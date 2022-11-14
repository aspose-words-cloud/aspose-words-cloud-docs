---
title: "Update Paragraph List Format in a Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /paragraphs/lists/update-paragraph-list-format-in-a-document/
aliases: [/update-paragraph-list-format-in-a-document/]
description: "Update a paragraph's list format in a Word document"
weight: 40
---

Updates the formatting properties of a paragraph list in the document node.

## REST API

| Server                         | REST endpoint        | HTTP method  |
|--------------------------------|----------------------|--------------|
| https://api.aspose.cloud/v4.0  | [/words/online/put/{nodePath}/paragraphs/{index}/listFormat](https://api.aspose.cloud/v4.0/words/online/put/{nodePath}/paragraphs/{index}/listFormat) | PUT |

, where:

* `nodePath` - the path to the node in the document tree.
* `index` - object index.

You can use these parameters in a REST request:

| Name                 | Type   | Description                                                  |
|----------------------|--------|--------------------------------------------------------------|
| `loadEncoding`       | string | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| `password`           | string | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| `encryptedPassword`  | string | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| `destFileName`       | string | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| `revisionAuthor`     | string | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| `revisionDateTime`   | string | The date and time to use for revisions.                      |


{{% alert style="info" %}}
**Note**: to access this REST API, you need to register and get personal credentials. Use the '[Quick Start](/getting-started/quickstart/)' guide to go through the procedure in a couple of minutes.
{{% /alert %}}


## Supported File Formats

The following input file formats are supported: DOC, DOT, DOCX, DOCM, DOTX, DOTM, FlatOPC (with and without macros), RTF, WordML, HTML, MHTHML, MOBI, CHM, AZW3, EPUB, ODT, OTT, TXT, Markdown, PDF, XML.

The following output file formats are supported: DOC, DOT, DOCX, DOCM, DOTX, DOTM, FlatOPC (with and without macros), RTF, WordML, HTML, MTHML, AZW3, EPUB, ODT, OTT, TXT, Markdown, PDF, XPS, XAML (fixed and flow), SVG, OpenXPS, PS, PCL, TIFF, PNG, BMP, EMF, JPG, GIF.


## Usage Examples

Let's look at practical examples of using the web service. You can do this both with cURL and Postman utilities, and from your code in various programming languages: Python, Java, JavaScript, C#, PHP, C++, Go, Ruby, Swift, Dart.

### How to Update a paragraph's list format in a Word document using cURL or Postman

One of the easiest and fastest ways to call a REST API is to use cURL or Postman:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="cURL Request" tabName2="Postman Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "UpdateParagraphListFormatOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "UpdateParagraphListFormatOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


### How to Update a paragraph's list format in a Word document using Python, Java, C#, C++, JavaScript and other programming languages

Using SDK is the quickest way to speed up the development. Please take a look at the provided code examples to quickly call this web service from your favourite programming language:

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="2" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "UpdateParagraphListFormatOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "UpdateParagraphListFormatOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "UpdateParagraphListFormatOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateParagraphListFormatOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "UpdateParagraphListFormatOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "UpdateParagraphListFormatOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateParagraphListFormatOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "UpdateParagraphListFormatOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "UpdateParagraphListFormatOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "UpdateParagraphListFormatOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

You can also visit our [GitHub repository](https://github.com/aspose-words-cloud) to explore a wide family of Aspose.Words Cloud SDKs. These software libraries take care of all low-level document-processing details and let you focus on your primary tasks.


