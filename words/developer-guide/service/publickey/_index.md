---
title: "Working with asymmetric public key"
type: docs
url: /publickey/
description: "Get asymmetric public key programmatically via Cloud API."
weight: 7
---

Aspose.Words REST API includes a `GetPublicKey` method that allows developers to retrieve the public key for an asymmetric encryption algorithm. The public key is returned in the form of a string, which can then be used to encrypt data.

Asymmetric encryption uses two different keys, a public key and a private key. The public key can be shared with anyone and is used to encrypt data, while the private key is kept secret and is used to decrypt data.

## Get asymmetric public key REST API

Server: `https://api.aspose.cloud/v4.0`

| Method   | Endpoint                      |
|:---------|:------------------------------|
| GET      | `/words/encryption/publickey` |

{{% alert style="info" %}}
**Note**: Requires Client Id and Secret. See [Quick Start](/words/getting-started/quickstart/) to obtain credentials.
{{% /alert %}}

### Response

**Response model**: [PublicKeyResponse](/spec/other/#publickeyresponse)

| Field   | Type                                                | Description                            |
|:--------|:----------------------------------------------------|:---------------------------------------|
| Model   | [PublicKeyResponse](/spec/other/#publickeyresponse) | REST response for RSA public key info. |

### Error reference

|   Status | Code             | Description                                | Resolution                                                                   |
|---------:|:-----------------|:-------------------------------------------|:-----------------------------------------------------------------------------|
|      401 | `unauthorized`   | Missing or invalid access token            | Obtain a new access token via the authentication endpoint                    |
|      403 | `forbidden`      | Access to the requested resource is denied | Verify that the access token has the required permissions                    |
|      404 | `not_found`      | The requested resource does not exist      | Check the resource ID or path for typos                                      |
|      429 | `rate_limited`   | Too many requests — rate limit exceeded    | Wait for the Retry-After period before making another request                |
|      500 | `internal_error` | An unexpected server error occurred        | Retry the request after a short delay; contact support if the issue persists |

## Usage examples

### REST API

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="cURL Request" tabName2="Postman Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetPublicKey.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetPublicKey.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

### SDK

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="2" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetPublicKey.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetPublicKey.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetPublicKey.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetPublicKey.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetPublicKey.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetPublicKey.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetPublicKey.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetPublicKey.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetPublicKey.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetPublicKey.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See Also

 * [Cloud SDKs](https://github.com/aspose-words-cloud) — Create, Edit, Convert and Render Word documents via REST API.

