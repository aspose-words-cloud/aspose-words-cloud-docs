---
title: "Convert Documents"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /convert/specified-format/
aliases: [/convert-word-document-from-request-content-to-specified-format/]
keywords: "convert to, word to doc, save Word file as PDF, convert Word document to HTML, Word doc to HTML, convert PDF to Word, TIFF file"
description: "Convert Word document to another format"
weight: 10
---

Document conversion Cloud API lets you convert Word document to another format. The API request contains a document to convert and the response contains the conversion result, or if outPath parameter specified - the API saves the result to the Cloud storage and return OK status code. 

You can check the quality of Aspose.Words Cloud conversion and view the results online:

- [Conversion](https://products.aspose.app/words/conversion)
- [Viewer](https://products.aspose.app/words/viewer)

The list of supported formats is provided below:

|format Parameter Value|Format of the returned Presentation|
| :- | :- |
|[bmp](https://docs.fileformat.com/image/bmp/)|Bitmap image file|
|[doc](https://docs.fileformat.com/word-processing/doc/)|Word document|
|[docm](https://docs.fileformat.com/word-processing/docm/)|Word Open XML Macro-Enabled Document|
|[docx](https://docs.fileformat.com/word-processing/docx/)|Microsoft Word Open XML Document|
|[dot](https://docs.fileformat.com/word-processing/dot/)|Word Document Template|
|[dotm](https://docs.fileformat.com/word-processing/dotm/)|Word Open XML Macro-Enabled Document Template|
|[dotx](https://docs.fileformat.com/word-processing/dotx/)|Word Open XML Document Template|
|[emf](https://docs.fileformat.com/image/emf/)|Enhanced Windows Metafile|
|[epub](https://docs.fileformat.com/ebook/epub/)|Open eBook File|
|[flatopc](#)|Flat OPC format|
|[gif](https://docs.fileformat.com/image/gif/)|Gif Image|
|[html](https://docs.fileformat.com/web/html/)|Hypertext Markup Language File|
|[jpeg](https://docs.fileformat.com/image/jpeg/)|JPEG Image|
|[mhtml](https://docs.fileformat.com/web/mhtml/)|MIME HTML File|
|[odt](https://docs.fileformat.com/word-processing/odt/)|OpenDocument Text Document|
|[ott](https://docs.fileformat.com/word-processing/ott/)|OpenDocument Document Template|
|[pcl](https://docs.fileformat.com/page-description-language/pcl/)|Printer Command Language File|
|[pdf](https://docs.fileformat.com/pdf/)|Portable Document Format File|
|[png](https://docs.fileformat.com/Image/png/)|Portable Network Graphic|
|[rtf](https://docs.fileformat.com/word-processing/rtf/)|Rich Text Format File|
|[svg](https://docs.fileformat.com/page-description-language/svg/)|Scalable Vector Graphics File|
|[swf](https://docs.fileformat.com/page-description-language/swf/)|Shockwave Flash Movie(removed)|
|[txt](https://docs.fileformat.com/word-processing/txt/)|Plain Text File|
|[tiff](https://docs.fileformat.com/image/tiff/)|Tagged Image File Format|
|[wml](#)|Wireless Markup Language File|
|[xps](https://docs.fileformat.com/page-description-language/xps/)|XML Paper Specification File|

The important parameters are described in the following table:

|Parameter Name|Type|Query String|Description|
| :- | :- | :- | :- |
|format|string|format=jpeg|Return the document in the specified format. Valid values for this parameter are given above.|
|outPath|string|outPath=SomeFolder/result.jpeg|A path for saving operation results to Cloud storage.|

The format can also be specified by the request Accept header.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Convert/ConvertDocument) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [TableDocument.doc](TableDocument.doc) and output [TableDocument.pdf](TableDocument.pdf) files designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to convert MS Word Document to PDF
curl -v "https://api.aspose.cloud/v4.0/words/convert?format=pdf" \
-X PUT \
-F document=@TableDocument.doc \
-H "Content-Type: multipart/form-data" \
-H "Accept: multipart/form-data" \
-H "Authorization: Bearer <jwt token>" \
-o TableDocument.pdf
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
PDF Document 
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "ConvertWordDocumentToAnotherFormat.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "ConvertWordDocumentToAnotherFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "ConvertWordDocumentToAnotherFormat.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "ConvertWordDocumentToAnotherFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "ConvertWordDocumentToAnotherFormat.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "ConvertWordDocumentToAnotherFormat.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "ConvertWordDocumentToAnotherFormat.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_ConvertWordDocumentToAnotherFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_ConvertWordDocumentToAnotherFormat.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See also

- Product page description: <a href="https://products.aspose.cloud/words/python/convert" target="_blank">Python</a>, <a href="https://products.aspose.cloud/words/net/convert" target="_blank">C#</a>, <a href="https://products.aspose.cloud/words/java/convert" target="_blank">Java</a>, <a href="https://products.aspose.cloud/words/nodejs/convert" target="_blank">Node.js</a>, <a href="https://products.aspose.cloud/words/php/convert" target="_blank">PHP</a>, <a href="https://products.aspose.cloud/words/go/convert" target="_blank">Go</a>
- <a href="https://products.aspose.app/words/conversion" target="_blank">Free online conversion app</a>
