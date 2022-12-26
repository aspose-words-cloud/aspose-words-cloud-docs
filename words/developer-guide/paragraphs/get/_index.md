---
title: "Get"
second_title: "Paragraphs in a Document"
type: docs
url: /paragraphs/get/
aliases: [/get-a-particular-paragraph-from-a-word-document/]
description: "Get a paragraph in a Word document"
weight: 30
---

Reads a paragraph from the document node.

## REST API

| Server                         | Method | Endpoint             |
|--------------------------------|--------|----------------------|
| https://api.aspose.cloud/v4.0  | PUT    | /words/online/get/{nodePath}/paragraphs/{index} |

, where:

* **`nodePath`** (required) - the path to the node in the document tree.
* **`index`** (required) - object index.

You can use the following parameters in a REST request:

| Parameter Name       | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `loadEncoding`       | string    | Optional           | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| `password`           | string    | Optional           | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| `encryptedPassword`  | string    | Optional           | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |


Use `$multipart/form-data` request to combine one or more properties into a single body:

| Property Name        | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `document`           | string(binary) | Required           | The document.                                                |

{{% alert style="info" %}}
**Note**: to access this REST API, you need to register and get personal credentials. Use the '[Quick Start](/getting-started/quickstart/)' guide to go through the procedure in a couple of minutes.
{{% /alert %}}


## Usage Examples

Let's look at practical examples of using the web service. You can do this both with cURL and Postman utilities, and from your code in various programming languages: Python, Java, JavaScript, C#, PHP, C++, Go, Ruby, Swift, Dart.

### How to get a paragraph in a Word document using cURL or Postman

One of the easiest and fastest ways to call a REST API is to use cURL or Postman:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="cURL Request" tabName2="Postman Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetParagraphOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetParagraphOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


### How to get a paragraph in a Word document using Python, Java, C#, C++, JavaScript and other programming languages

Using SDK is the quickest way to speed up the development. Please take a look at the provided code examples to quickly call this web service from your favourite programming language:

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="2" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetParagraphOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetParagraphOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetParagraphOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetParagraphOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetParagraphOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetParagraphOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetParagraphOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetParagraphOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetParagraphOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetParagraphOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


## See Also

 * [GitHub repository](https://github.com/aspose-words-cloud) - explore Aspose.Words Cloud SDK Family. These software libraries take care of all low-level document-processing details.


