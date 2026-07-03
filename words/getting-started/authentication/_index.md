---
title: "Authentication"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /getting-started/authentication/
aliases: [/authentication/]
description: "Authenticate with Aspose.Words Cloud API using OAuth 2.0 Client Credentials and JWT Bearer tokens. Obtain access tokens via POST /connect/token."
weight: 40
---

Aspose.Words Cloud uses [OAuth 2.0 Client Credentials](https://docs.aspose.cloud/total/getting-started/rest-api-overview/authenticating-api-requests/) flow with JWT Bearer tokens. All API requests require an `Authorization: Bearer <token>` header.

## Get Credentials

API authentication uses a **Client Id** (a UUID) and **Client Secret** (a hex string) — separate from your dashboard login. Create them in the [Aspose Dashboard](https://dashboard.aspose.cloud/):

1. Go to [Applications](https://dashboard.aspose.cloud/#/applications) and click **Create New Application**
2. Enter a name and description for your app. Select a default storage — create one first via [Storages](https://dashboard.aspose.cloud/#/storages) if needed
3. Click **Save**. The app appears in your applications list
4. Click on the app card to view its details. Both **Client Id** and **Client Secret** are displayed with copy buttons. To replace a compromised secret, use **Regenerate Client Secret**

The application details page also lets you configure:

- **Application Limits** — set optional daily or monthly caps on API calls for this app. Useful for controlling usage per client or environment
- **CORS Origin** — optional. Only needed if you call the Words Cloud API directly from browser JavaScript (`fetch`, `XMLHttpRequest`). Server-side applications (SDKs, curl, backend code) do not require CORS configuration. Add each allowed domain on a separate line (e.g., `https://myapp.com`)

The same credentials work across all [Aspose Cloud products](https://products.aspose.cloud/) — Words, PDF, Cells, and more.

## Obtain an Access Token

Send your credentials to the authentication endpoint:

{{< tabs tabTotal="4" tabID="1" tabName1="cURL" tabName2="Python" tabName3="C#" tabName4="Java">}}

{{< tab tabNum="1" >}}
```bash
curl -X POST "https://api.aspose.cloud/connect/token" \
  -H "Content-Type: application/x-www-form-urlencoded" \
  -H "Accept: application/json" \
  -d "grant_type=client_credentials&client_id=YOUR_CLIENT_ID&client_secret=YOUR_CLIENT_SECRET"
```
{{< /tab >}}

{{< tab tabNum="2" >}}
```python
import requests

response = requests.post(
    "https://api.aspose.cloud/connect/token",
    data={
        "grant_type": "client_credentials",
        "client_id": "YOUR_CLIENT_ID",
        "client_secret": "YOUR_CLIENT_SECRET"
    },
    headers={"Content-Type": "application/x-www-form-urlencoded"}
)
token = response.json()["access_token"]
```
{{< /tab >}}

{{< tab tabNum="3" >}}
```csharp
using Aspose.Words.Cloud.Sdk;

var config = new Configuration
{
    ClientId = "YOUR_CLIENT_ID",
    ClientSecret = "YOUR_CLIENT_SECRET"
};
var api = new WordsApi(config);
// Token is obtained and managed automatically by the SDK
```
{{< /tab >}}

{{< tab tabNum="4" >}}
```java
import com.aspose.words.cloud.*;

WordsApi api = new WordsApi(
    "YOUR_CLIENT_ID",
    "YOUR_CLIENT_SECRET",
    "https://api.aspose.cloud"
);
// Token is obtained and managed automatically by the SDK
```
{{< /tab >}}

{{< /tabs >}}

**Response** — a JSON object with your access token:

```json
{
  "access_token": "eyJhbGciOiJSUzI1NiIs...",
  "token_type": "Bearer"
}
```

## Use the Token

Include the token in the `Authorization` header of every API request:

```bash
curl -X GET "https://api.aspose.cloud/v4.0/words/info" \
  -H "Authorization: Bearer YOUR_TOKEN"
```

SDKs handle authentication automatically — pass your credentials once when creating the API client, and the SDK manages token acquisition and renewal.

## Token Lifetime

- Cache the token and reuse it until expiration — do not request a new token for each API call
- On HTTP 401, request a fresh token and retry
- The `expires_in` field in the token response indicates the remaining validity period

## Security Best Practices

- Store credentials in environment variables, not in source code:
  ```bash
  export ASPOSE_CLIENT_ID="your_client_id"
  export ASPOSE_CLIENT_SECRET="your_client_secret"
  ```
- Rotate credentials periodically via the [Aspose Dashboard](https://dashboard.aspose.cloud/#/applications) — use **Regenerate Client Secret** on your application details page
- All API communication is encrypted via HTTPS

→ [Quickstart: Make your first API call](/words/getting-started/quickstart/)
→ [Full OAuth2 details (Aspose.Total)](https://docs.aspose.cloud/total/getting-started/rest-api-overview/authenticating-api-requests/)
