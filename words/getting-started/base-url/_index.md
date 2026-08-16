---
title: "Base URL & Environments"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /getting-started/base-url/
aliases: [/base-url/]
description: "Aspose.Words Cloud API base URL is https://api.aspose.cloud/v4.0/words. Learn about API versioning, environments, and custom base URL configuration."
weight: 50
---

All Aspose.Words Cloud API requests are sent to a single base URL.

## REST API

```
https://api.aspose.cloud/v4.0/words
```

All API operations are relative to this base. For example:

```bash
GET  https://api.aspose.cloud/v4.0/words/info
PUT  https://api.aspose.cloud/v4.0/words/{filename}/saveAs
```

## Authentication Endpoint

```
POST https://api.aspose.cloud/connect/token
```

The authentication service runs on the same domain but is separate from the Words API. See the [Authentication Guide](/words/getting-started/authentication/) for details.

## API Version

Current version: **v4.0**. The version is part of the URL path: `/v4.0/words/...`

There is no separate staging or sandbox environment. Use the [free trial](/words/getting-started/evaluate-aspose-words/) for testing — it provides full API access with a monthly call limit.

## Self-Hosted (Docker)

When running [Aspose.Words Cloud as a Docker container](/words/getting-started/how-to-run-docker-container/), the base URL changes to:

```
http://localhost/v4.0/words
```

### SDK Configuration

All SDKs default to the production URL. To use a custom base URL:

```python
import asposewordscloud

api = asposewordscloud.WordsApi(
    "YOUR_CLIENT_ID",
    "YOUR_CLIENT_SECRET",
    base_url="http://localhost/v4.0/words"
)
```

The same pattern applies to all [available SDKs](/words/getting-started/available-sdks/) — pass the base URL as the third constructor argument.

→ [Deployment Guides](/words/getting-started/how-to-run-docker-container/)
