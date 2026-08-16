---
title: "Move a folder to a new location in Cloud Storage online"
articleTitle: "Move a folder to a new location in Cloud Storage"
linktitle: "Move a folder to a new location in Cloud Storage"
type: docs
url: /files-and-storage/move-folder/
description: "Move a folder to a new location in Cloud Storage programmatically via Cloud API."
weight: 90
---

This REST API moves a folder to a new location in Cloud Storage.

## Move a folder to a new location in Cloud Storage REST API

Server: `https://api.aspose.cloud/v4.0`

| Method   | Endpoint                               |
|:---------|:---------------------------------------|
| PUT      | `/words/storage/folder/move/{srcPath}` |

| Parameter Name       | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `destPath`           | string    | Required           | Destination folder path to move to e.g '/dst'                |
| `srcStorageName`     | string    | Optional           | Source storage name                                          |
| `destStorageName`    | string    | Optional           | Destination storage name                                     |

{{% alert style="info" %}}
**Note**: Requires Client Id and Secret. See [Quick Start](/words/getting-started/quickstart/) to obtain credentials.
{{% /alert %}}

### Error reference

|   Status | Code             | Description                                       | Resolution                                                                   |
|---------:|:-----------------|:--------------------------------------------------|:-----------------------------------------------------------------------------|
|      400 | `bad_request`    | Invalid parameter value or missing required field | Check the parameter format and ensure all required fields are provided       |
|      401 | `unauthorized`   | Missing or invalid access token                   | Obtain a new access token via the authentication endpoint                    |
|      403 | `forbidden`      | Access to the requested resource is denied        | Verify that the access token has the required permissions                    |
|      404 | `not_found`      | The requested resource does not exist             | Check the resource ID or path for typos                                      |
|      429 | `rate_limited`   | Too many requests — rate limit exceeded           | Wait for the Retry-After period before making another request                |
|      500 | `internal_error` | An unexpected server error occurred               | Retry the request after a short delay; contact support if the issue persists |

## Usage examples

### REST API

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="cURL Request" tabName2="Postman Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "MoveFolder.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "MoveFolder.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

### SDK

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="2" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "MoveFolder.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "MoveFolder.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "MoveFolder.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "MoveFolder.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "MoveFolder.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "MoveFolder.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "MoveFolder.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "MoveFolder.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "MoveFolder.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "MoveFolder.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See Also

 * [Cloud SDKs](https://github.com/aspose-words-cloud) — Create, Edit, Convert and Render Word documents via REST API.

