﻿---
title: "Insert watermark image into a Word document online"
articleTitle: "Insert watermark image"
linktitle: "Insert watermark image"
type: docs
url: /watermark/insert-image/
description: "Insert watermark image into a Word document programmatically via Cloud API."
weight: 20
---

Inserts watermark image into a Word document.


## Insert watermark image into a Word document REST API

| Server                         | Method | Endpoint             |
|--------------------------------|--------|----------------------|
| `https://api.aspose.cloud/v4.0`  | PUT    | `/words/online/post/watermarks/images` |

You can use the following parameters in a REST request:

| Parameter Name       | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `loadEncoding`       | string    | Optional           | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| `password`           | string    | Optional           | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| `encryptedPassword`  | string    | Optional           | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| `destFileName`       | string    | Optional           | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| `revisionAuthor`     | string    | Optional           | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| `revisionDateTime`   | string    | Optional           | The date and time to use for revisions.                      |
| `rotationAngle`      | number(double) | Optional           | The rotation angle of the watermark.                         |
| `image`              | string    | Optional           | The filename of the image. If the parameter value is missing — the image data is expected in the request content. |


Use `$multipart/form-data` request to combine one or more properties into a single body:

| Property Name        | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `document`           | string(binary) | Required           | The document.                                                |
| `multipartbody`      | #/paths//words/{name}/watermarks/images/post/requestBody/content/application/json/schema | Required           |                                                              |

{{% alert style="info" %}}
**Note**: to access this REST API, you need to register and get personal credentials. Use the '[Quick Start](/words/getting-started/quickstart/)' guide to go through the procedure in a couple of minutes.
{{% /alert %}}


## Insert watermark image into a Word document usage examples

Let's look at practical examples of using the web service. You can do this both with cURL and Postman utilities, and from your code in various programming languages: Python, Java, JavaScript, C#, PHP, C++, Go, Ruby, Swift, Dart.

### How to insert watermark image into a Word document with cURL or Postman

One of the easiest and fastest ways to call a REST API is to use cURL or Postman:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="cURL Request" tabName2="Postman Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "InsertWatermarkImageOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "InsertWatermarkImageOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


### How to insert watermark image into a Word document in Python, Java, C#, C++, JavaScript and other programming languages

Using SDK is the quickest way to speed up the development. Please take a look at the provided code examples to quickly call this web service from your favourite programming language:

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="2" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "InsertWatermarkImageOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "InsertWatermarkImageOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "InsertWatermarkImageOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "InsertWatermarkImageOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "InsertWatermarkImageOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "InsertWatermarkImageOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "InsertWatermarkImageOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "InsertWatermarkImageOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "InsertWatermarkImageOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "InsertWatermarkImageOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


## See Also

 * [GitHub repository](https://github.com/aspose-words-cloud) — explore Aspose.Words Cloud SDK Family. These software libraries take care of all low-level document-processing details.


