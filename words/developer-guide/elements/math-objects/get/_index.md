---
title: "Get an OfficeMath object in a Word document online"
articleTitle: "Get an OfficeMath object"
linktitle: "Get an OfficeMath object"
type: docs
url: /math-objects/get/
description: "Get an OfficeMath object in a Word document programmatically via Cloud API."
weight: 10
---

Returns an `OfficeMath` object in a Word document.

## Get an OfficeMath object in a Word document REST API

Server: `https://api.aspose.cloud/v4.0`

| Method   | Endpoint                                                 |
|:---------|:---------------------------------------------------------|
| PUT      | `/words/online/get/{nodePath}/OfficeMathObjects/{index}` |

| Parameter Name       | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `loadEncoding`       | string    | Optional           | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| `password`           | string    | Optional           | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| `encryptedPassword`  | string    | Optional           | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |

{{% alert style="info" %}}
**Note**: Requires Client Id and Secret. See [Quick Start](/words/getting-started/quickstart/) to obtain credentials.
{{% /alert %}}

### Response

**Response model**: [OfficeMathObjectResponse](/spec/mathobject/#officemathobjectresponse)

| Field   | Type                                                                   | Description                                 |
|:--------|:-----------------------------------------------------------------------|:--------------------------------------------|
| Model   | [OfficeMathObjectResponse](/spec/mathobject/#officemathobjectresponse) | The REST response with a OfficeMath object. |

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
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetOfficeMathObjectOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetOfficeMathObjectOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

### SDK

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="2" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetOfficeMathObjectOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetOfficeMathObjectOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetOfficeMathObjectOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetOfficeMathObjectOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetOfficeMathObjectOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetOfficeMathObjectOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetOfficeMathObjectOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetOfficeMathObjectOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetOfficeMathObjectOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetOfficeMathObjectOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See Also

 * [Cloud SDKs](https://github.com/aspose-words-cloud) — Create, Edit, Convert and Render Word documents via REST API.

