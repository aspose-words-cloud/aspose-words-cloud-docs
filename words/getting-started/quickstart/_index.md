---
title: "Quickstart"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /getting-started/quickstart/
aliases: [/quickstart/]
description: "Make your first Aspose.Words Cloud API call in 5 minutes. Create an account, get credentials, install an SDK, and process a Word document."
weight: 30
---

Follow these five steps to make your first Words Cloud API call.

## 1. Create an Account

Sign up for a free Aspose Cloud account — no credit card required.

1. Go to the [Aspose Dashboard](https://dashboard.aspose.cloud/)
2. Click **Sign In with GitHub** or **Sign In with Google**, or create an account with your email
3. Verify your email address

Your account includes **150 free API calls per month**.

## 2. Create a Storage

Words Cloud processes documents from cloud storage. Create a storage container for your files:

1. In the dashboard sidebar, open **Files**
2. Click the storage dropdown and select **Create New Storage**
3. Choose **Internal Storage** (Aspose-managed) — simplest for getting started
4. Name it (e.g., `my-documents`)

For Azure, AWS S3, or other storage backends, see the [deployment guides](/words/getting-started/how-to-run-docker-container/).

You can upload test documents through the **Files** page in the dashboard sidebar.

## 3. Create an API Client App

1. In the dashboard sidebar, open **Applications**
2. Click **Create New Application**
3. Enter a name (e.g., `My Words App`) and a description
4. Select your storage as the default
5. Click **Save**

Copy your **Client Id** and **Client Secret** — these are separate from your dashboard login. You will use them to authenticate API requests.

## 4. Install an SDK

{{< tabs tabTotal="4" tabID="1" tabName1="Python" tabName2=".NET" tabName3="Java" tabName4="Node.js">}}

{{< tab tabNum="1" >}}
```bash
pip install aspose-words-cloud
```
{{< /tab >}}

{{< tab tabNum="2" >}}
```bash
dotnet add package Aspose.Words-Cloud
```
{{< /tab >}}

{{< tab tabNum="3" >}}
Add the Aspose Maven repository (`https://releases.aspose.cloud/java/repo/`) and dependency `com.aspose:aspose-words-cloud`.
{{< /tab >}}

{{< tab tabNum="4" >}}
```bash
npm install asposewordscloud
```
{{< /tab >}}

{{< /tabs >}}

→ [All 10 SDKs with install commands](/words/getting-started/available-sdks/)

## 5. Make an API Request

Replace `CLIENT_ID` and `CLIENT_SECRET` with your credentials.

{{< tabs tabTotal="4" tabID="2" tabName1="Python" tabName2=".NET" tabName3="Java" tabName4="cURL">}}

{{< tab tabNum="1" >}}
```python
import asposewordscloud

api = asposewordscloud.WordsApi("CLIENT_ID", "CLIENT_SECRET")
result = api.get_info()
print(f"Words Cloud version: {result.version}")
```
{{< /tab >}}

{{< tab tabNum="2" >}}
```csharp
using Aspose.Words.Cloud.Sdk;

var config = new Configuration
{
    ClientId = "CLIENT_ID",
    ClientSecret = "CLIENT_SECRET"
};
var api = new WordsApi(config);
var result = await api.GetInfo();
Console.WriteLine($"Version: {result.Version}");
```
{{< /tab >}}

{{< tab tabNum="3" >}}
```java
import com.aspose.words.cloud.*;

WordsApi api = new WordsApi(
    "CLIENT_ID", "CLIENT_SECRET", "https://api.aspose.cloud"
);
InfoResponse result = api.getInfo();
System.out.println("Version: " + result.getVersion());
```
{{< /tab >}}

{{< tab tabNum="4" >}}
```bash
# Get access token
TOKEN=$(curl -s -X POST "https://api.aspose.cloud/connect/token" \
  -d "grant_type=client_credentials&client_id=CLIENT_ID&client_secret=CLIENT_SECRET" \
  -H "Content-Type: application/x-www-form-urlencoded" \
  | grep -o '"access_token":"[^"]*"' | cut -d'"' -f4)

# Call the API
curl -s "https://api.aspose.cloud/v4.0/words/info" \
  -H "Authorization: Bearer $TOKEN"
```
{{< /tab >}}

{{< /tabs >}}

## Next Steps

- [Developer Guide](/words/developer-guide/) — all API operations
- [API Reference](https://apireference.aspose.cloud/words/) — interactive API explorer
- [Authentication Guide](/words/getting-started/authentication/) — token details and best practices
- [Rate Limits](/words/getting-started/rate-limits/) — understand usage limits
