---
title: "Error Handling"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /getting-started/error-handling/
aliases: [/error-handling/]
description: "Standard HTTP error codes for Aspose.Words Cloud API: 400, 401, 403, 404, 429, 500. Error response format, retry strategies, and troubleshooting."
weight: 90
---

The Words Cloud API returns standard HTTP status codes. Each API operation page includes detailed error tables for operation-specific errors.

## Standard Error Codes

| Status | Code | Meaning | Action |
|--------|------|---------|--------|
| 400 | `bad_request` | Invalid parameter or missing required field | Check parameter format and required fields |
| 401 | `unauthorized` | Missing or invalid access token | Obtain a new token — see [Authentication](/words/getting-started/authentication/) |
| 403 | `forbidden` | Access denied to the requested resource | Verify the token has the required permissions |
| 404 | `not_found` | Resource does not exist | Check the resource ID or path for typos |
| 429 | `rate_limited` | Too many requests | Wait for the `Retry-After` period — see [Rate Limits](/words/getting-started/rate-limits/) |
| 500 | `internal_error` | Unexpected server error | Retry after a short delay; contact [support](https://forum.aspose.cloud/c/words) if the issue persists |

## Error Response Format

Errors are returned as JSON:

```json
{
  "requestId": "38a90f3ae7c6c6eca4daca26de3cd154",
  "error": {
    "code": "errorAuthorization",
    "message": "Unauthorized",
    "description": "Operation Failed. The authorization data is incorrect.",
    "dateTime": "2026-07-01T12:03:52.4820502Z",
    "innerError": null
  }
}
```

The `code` field contains the specific error type. The `message` and `description` fields provide human-readable details.

## Retry Strategy

Implement exponential backoff for transient errors (429, 500):

```python
import time
import requests

def call_with_retry(url, headers, max_retries=3):
    for attempt in range(max_retries):
        response = requests.get(url, headers=headers)

        if response.status_code == 429:
            wait = int(response.headers.get("Retry-After", 5))
            time.sleep(wait)
            continue

        if response.status_code >= 500:
            time.sleep(2 ** attempt)  # 1s, 2s, 4s
            continue

        return response

    raise Exception(f"Request failed after {max_retries} retries")
```

→ [Rate Limits](/words/getting-started/rate-limits/)  |  → [Authentication](/words/getting-started/authentication/)
