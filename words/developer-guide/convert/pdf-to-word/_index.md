---
title: "PDF to Word"
second_title: "Convert"
type: docs
url: /convert/pdf-to-word/
aliases: [/convert-pdf-document-to-word/]
keywords: "convert PDF to Word, PDF to Word conversion, PDF to DOC, PDF to DOCX in Python, C#, Java, C++, Ruby, PHP, NodeJS, Go, Android, Swift, Dart"
description: "Cloud API to programmatically convert PDF to Word documents. Robust conversion engine to save PDF in DOC, DOCX and other formats with Python, C#, Java, C++, Ruby, PHP, NodeJS, Go, Android, Swift, Dart"
weight: 20
---

Aspose provides a high fidelity API to programmatically convert PDF to Word document formats and in the opposite directions with professional quality. The combined use of Adobe and Microsoft Office technologies has a lot to offer to the end-user.

These major document formats, including DOCX, DOC, RTF, ОDT and PDF, are capable of encapsulating almost any type of data including text, tables, raster and vector graphics, video, audio, and also support a wide range of formatting features.

Despite similarities, PDF and Word documents have considerable differences in the operational capabilities.

PDF documents support multilevel security options and are difficult to extract information. PDF format is the best choice when the document’s author allows others to read and print document copies only. Word document formats, in contrast, are great for collaborative development, but they aren't always the best choice for distributing as they can be easily modified without author's permission.

You may require to convert an immutable PDF to an editable DOCX or DOC document and it is also a fine solution if you need to extract text from a PDF file easily.

Aspose conversion engine transforms a PDF to Word-based document format, that can be naturally edited with any mainstream word processor. However, some complex formatting might appear slightly different from the original document. PDF to Word conversion supports detecting headers and footers. Sections of PDF pages containing page numbers, document names, etc. will be converted as Word's headers and footers. These headers and footers do not affect the rest of the page layout and are not moved while the document is being edited.

Aspose PDF to Word conversion engine currently supports the following features:

- Text and paragraphs
- Text formatting (font, size, foreground/background, options like bold, italic, underline)
- Bulleted and numbered lists (including nested lists)
- Tables (bordered and non-bordered, without nested tables)
- Images conversion
  - Semi-transparent images
  - Rotated images
  - Inline images (images that go "inside" the text, being a logical part of text paragraph)
- Encrypted PDF files
- Properly converts style and destination of hyperlinks, both to URLs and local files
- Headers/footers detection for PDF conversion
- Bookmarks
- Basic vector graphics

{{% alert style="info" %}}

There is a restriction on the usage of multi-column text that will be addressed in future API versions. Multi-column text is currently not supported by PDF to Word conversion API.

{{% /alert %}}

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Convert/SaveAs) defines a publicly accessible programming interface and lets you run PDF to Word conversions directly from a web browser.

You can also use cURL command-line utility to convert PDF to Word document. The following code demonstrates how to convert PDF to DOCX with cURL. Feel free to download and explore both input [demo.pdf](demo.pdf) and output [demo.docx](demo.docx) sample documents to figure things out.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to convert PDF document to Word
curl -v "https://api.aspose.cloud/v4.0/words/demo.pdf/saveAs" \
-X PUT \
-d "{'SaveFormat':'docx', 'FileName': 'demo.docx'}" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "SaveResult": {
    "SourceDocument": {
      "Href": "http://api.aspose.cloud/v4.0/words/demo.pdf",
      "Rel": "self",
      "Type": null,
      "Title": null
    },
    "DestDocument": {
      "Href": "demo.docx",
      "Rel": "saved",
      "Type": null,
      "Title": null
    },
    "AdditionalItems": [
    ]
  },
  "Code": 200,
  "Status": "OK"
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs.

The following code examples demonstrate how to convert PDF to Word programmatically using various Aspose.Words SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "ConvertPDFDocumentToWord.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "ConvertPDFDocumentToWord.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "ConvertPDFDocumentToWord.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "ConvertPDFDocumentToWord.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "ConvertPDFDocumentToWord.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "ConvertPDFDocumentToWord.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_ConvertPDFDocumentToWord.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_ConvertPDFDocumentToWord.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "ConvertPDFDocumentToWord.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See also

- Product page description: <a href="https://products.aspose.cloud/words/python/convert" target="_blank">Python</a>, <a href="https://products.aspose.cloud/words/net/convert" target="_blank">C#</a>, <a href="https://products.aspose.cloud/words/java/convert" target="_blank">Java</a>, <a href="https://products.aspose.cloud/words/nodejs/convert" target="_blank">Node.js</a>, <a href="https://products.aspose.cloud/words/php/convert" target="_blank">PHP</a>, <a href="https://products.aspose.cloud/words/go/convert" target="_blank">Go</a>,
"https://products.aspose.cloud/words/go/dart" target="_blank">Dart</a>
- <a href="https://products.aspose.app/words/conversion/pdf-to-word" target="_blank">Free online PDF to Word Converter app</a>
