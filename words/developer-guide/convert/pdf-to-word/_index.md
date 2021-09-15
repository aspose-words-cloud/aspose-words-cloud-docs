---
title: "PDF to Word"
second_title: "Convert"
type: docs
url: /convert/pdf-to-word/
aliases: [/convert-pdf-document-to-word/]
keywords: "convert PDF to Word, PDF to Word conversion, PDF to DOC, PDF to DOCX in Python, C#, Java, C++, Ruby, PHP, NodeJS, Go, Swift, Dart"
description: "Cloud API to programmatically convert PDF to Word documents. Robust conversion engine to save PDF in DOC, DOCX and other formats with Python, C#, Java, C++, Ruby, PHP, NodeJS, Go, Android, Swift, Dart"
weight: 20
---

Aspose provides a high fidelity API to programmatically convert PDF documents to Word format and in the opposite directions with professional quality. The combined use of Adobe and Microsoft Office technologies has a lot to offer to the end-user.

These major document formats, including [DOCX](https://docs.fileformat.com/word-processing/docx/), [DOC](https://docs.fileformat.com/word-processing/doc/), [RTF](https://docs.fileformat.com/word-processing/rtf/), [ODT](https://docs.fileformat.com/word-processing/odt/) and [PDF](https://docs.fileformat.com/pdf/), are capable of encapsulating almost any type of data including text, tables, raster and vector graphics, video, audio, and also support a wide range of formatting features.

Despite similarities, [PDF](https://docs.fileformat.com/pdf/) and Word documents have considerable differences in the operational capabilities.

[PDF](https://docs.fileformat.com/pdf/) documents support multilevel security options and are difficult to extract information. [PDF](https://docs.fileformat.com/pdf/) format is the best choice when the document’s author allows others to read and print document copies only. Word document formats, in contrast, are great for collaborative development, but they aren't always the best choice for distributing as they can be easily modified without author's permission.

You may require to convert an immutable [PDF](https://docs.fileformat.com/pdf/) to an editable [DOCX](https://docs.fileformat.com/word-processing/docx/) or [DOC](https://docs.fileformat.com/word-processing/doc/) document and it is also a fine solution if you need to extract text from a [PDF](https://docs.fileformat.com/pdf/) file easily.

Aspose conversion engine transforms a [PDF](https://docs.fileformat.com/pdf/) to Word-based document format, that can be naturally edited with any mainstream word processor. However, some complex formatting might appear slightly different from the original document. [PDF](https://docs.fileformat.com/pdf/) to Word conversion supports detecting headers and footers. Sections of PDF pages containing page numbers, document names, etc. will be converted as Word's headers and footers. These headers and footers do not affect the rest of the page layout and are not moved while the document is being edited.

Aspose [PDF](https://docs.fileformat.com/pdf/) to Word conversion engine currently supports the following features:

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

You can use **cURL** command-line tool to access Aspose.Words web services and convert PDF documents to Word format easily. The following code demonstrates how to convert PDF to DOCX with cURL. Feel free to download and explore sample input [demo.pdf](demo.pdf) and output [demo.docx](demo.docx) files designed to act as a demonstration and let you figure out the details quickly.

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
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

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
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "SaveAsOnline_1.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "SaveAsOnline_1.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "SaveAsOnline_1.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "SaveAsOnline_1.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "SaveAsOnline_1.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "SaveAsOnline_1.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "SaveAsOnline_1.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "SaveAsOnline_1.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "SaveAsOnline_1.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "SaveAsOnline_1.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See also

- Product page description: <a href="https://products.aspose.cloud/words/python/convert" target="_blank">Python</a>, <a href="https://products.aspose.cloud/words/net/convert" target="_blank">C#</a>, <a href="https://products.aspose.cloud/words/java/convert" target="_blank">Java</a>, <a href="https://products.aspose.cloud/words/nodejs/convert" target="_blank">Node.js</a>, <a href="https://products.aspose.cloud/words/php/convert" target="_blank">PHP</a>, <a href="https://products.aspose.cloud/words/go/convert" target="_blank">Go</a>,
<a href="https://products.aspose.cloud/words/dart/convert" target="_blank">Dart</a>
- <a href="https://products.aspose.app/words/conversion/pdf-to-word" target="_blank">Free online PDF to Word Converter app</a>
