﻿---
title: "Get a Header/Footer of a Section online"
articleTitle: "Get a Header/Footer of a Section"
linktitle: "Get a Header/Footer of a Section"
type: docs
url: /headers-and-footers/get-of-section/
description: "Get a Header/Footer of a Section programmatically via Cloud API."
weight: 41
---

Returns a HeaderFooter object from the document section.


## Get a Header/Footer of a Section REST API

| Server                         | Method | Endpoint             |
|--------------------------------|--------|----------------------|
| `https://api.aspose.cloud/v4.0`  | PUT    | `/words/online/get/sections/{sectionIndex}/headersfooters/{headerFooterIndex}` |

, where:

* **`headerFooterIndex`** (required) — the index of the HeaderFooter object.
* **`sectionIndex`** (required) — the index of the section.

You can use the following parameters in a REST request:

| Parameter Name       | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `loadEncoding`       | string    | Optional           | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| `password`           | string    | Optional           | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| `encryptedPassword`  | string    | Optional           | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| `filterByType`       | string    | Optional           | The list of HeaderFooter types.                              |


Use `$multipart/form-data` request to combine one or more properties into a single body:

| Property Name        | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `document`           | string(binary) | Required           | The document.                                                |

{{% alert style="info" %}}
**Note**: to access this REST API, you need to register and get personal credentials. Use the '[Quick Start](/words/getting-started/quickstart/)' guide to go through the procedure in a couple of minutes.
{{% /alert %}}


## Get a Header/Footer of a Section usage examples

Let's look at practical examples of using the web service. You can do this both with cURL and Postman utilities, and from your code in various programming languages: Python, Java, JavaScript, C#, PHP, C++, Go, Ruby, Swift, Dart.

### How to get a Header/Footer of a Section with cURL or Postman

One of the easiest and fastest ways to call a REST API is to use cURL or Postman:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="cURL Request" tabName2="Postman Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetHeaderFooterOfSectionOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetHeaderFooterOfSectionOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


### How to get a Header/Footer of a Section in Python, Java, C#, C++, JavaScript and other programming languages

Using SDK is the quickest way to speed up the development. Please take a look at the provided code examples to quickly call this web service from your favourite programming language:

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="2" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetHeaderFooterOfSectionOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetHeaderFooterOfSectionOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetHeaderFooterOfSectionOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetHeaderFooterOfSectionOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetHeaderFooterOfSectionOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetHeaderFooterOfSectionOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetHeaderFooterOfSectionOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetHeaderFooterOfSectionOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetHeaderFooterOfSectionOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetHeaderFooterOfSectionOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


## See Also

 * [GitHub repository](https://github.com/aspose-words-cloud) — explore Aspose.Words Cloud SDK Family. These software libraries take care of all low-level document-processing details.


