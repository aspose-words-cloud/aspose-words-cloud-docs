---
title: "Rate Limits"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /getting-started/rate-limits/
aliases: [/rate-limits/]
description: "Aspose.Words Cloud rate limits: 5 failed auth attempts trigger a 10-minute cooldown. API operations are not currently rate-limited."
weight: 80
---

Aspose Cloud applies rate limiting to protect service stability.

## Current Limits

| Endpoint | Limit | Window | Response |
|----------|-------|--------|----------|
| `POST /connect/token` | 5 failed attempts | per credential pair | HTTP 429, `Retry-After: 600` |

Rate limits are based on the **Client Id + Client Secret** combination — not IP address. Successful authentication resets the counter. Changing either credential immediately lifts the limit.

## API Operations

Words Cloud API operations (`/v4.0/words/*`) are **not currently rate-limited**. This policy may change — monitor this page for updates.

## Handling Rate Limits

When the limit is hit, the API returns:

```http
HTTP/1.1 429 Too Many Requests
Retry-After: 600
```

Implement a retry strategy that respects the `Retry-After` header:

```python
import time
import requests

def call_with_backoff(url, headers, max_retries=3):
    for attempt in range(max_retries):
        response = requests.get(url, headers=headers)

        if response.status_code == 429:
            wait = int(response.headers.get("Retry-After", 60))
            time.sleep(wait)
            continue

        return response

    raise Exception(f"Max retries ({max_retries}) exceeded")
```

## Best Practices

- **Cache tokens** — reuse valid tokens. Do not re-authenticate for each API call
- **Validate credentials** — test credentials locally before deploying
- **Monitor 429 responses** — set up alerts for rate limit hits in production

→ [Error Handling](/words/getting-started/error-handling/)  |  → [Full rate limit policy (Aspose.Total)](https://docs.aspose.cloud/total/rate-limits/)
