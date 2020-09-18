---
title: "Convert PDF Document to Word"
type: docs
url: /convert-pdf-document-to-word/
keywords: "convert pdf to word, dotm file, go sdk, Python, Ruby, Java, C#, Node.js, PHP, Android, Swift and Go"
description: "Our conversion APIs let you convert PDF to Word document. The APIs even supports encrypted PDF file to Word document conversion. The converter turns a document into a &amp;quot;flow&amp;quot; format - merges multiple paragraphs into one section, converts tables and lists into native Word tables and lists, etc. so that document can then be naturally edited in Word editing application (such as Microsoft Word). Currently, we support Python, C#, Java, Ruby, PHP, Node.JS, Go, Android, Swift"
weight: 40
---

# **Introduction**
Our conversion APIs let you *convert PDF to Word* document. The APIs even supports encrypted PDF file to Word document conversion. The converter turns a document into a "flow" format - merges multiple paragraphs into one section, converts tables and lists into native Word tables and lists, etc. so that document can then be naturally edited in Word editing application (such as Microsoft Word).

{{% alert color="primary" %}} 

Aspose.Words conversion engine is deliberately focused on conversion document structure into a "flow" format. The resulting document will be "editable" but some complex formatting might appear different from the original document.

{{% /alert %}} 

PDF to Word conversion supports detecting headers and footers. Sections of PDF pages containing page numbers, document names, etc. will be converted as headers and footers in Word document that do not affect the rest of the page layout and are not moved while the document is being edited.

Converter currently supports the following features:

- Text and paragraphs
- Text formatting (font, size, foreground/background, options like bold, italic, underline)
- Bulleted and numbered lists (including nested lists)
- Tables (bordered and non-bordered, without nested tables)
- Images conversion
  - Semi-transparent images
  - Rotated images
  - Inline images (images that go “inside” the text, being a logical part of text paragraph)
- Encrypted PDF files
- Properly converts style and destination of hyperlinks, both to URLs and local files
- Headers/footers detection for PDF conversion
- Bookmarks
- Basic vector graphics

The following limitations apply and will be addressed in future versions:

- Multi-column text is not supported
- Password-protected PDF documents are not supported

**Note:** We support Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift so far you can find the sample code below in this page:
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Convert/SaveAs) lets you call this REST API directly from the browser. The description of the API and its parameters is also given there.
## **cURL Example**
**Input Document:** [2019_new_demo.pdf](attachments/885287/8028167.pdf)

**Output Document:** [2019_new_demo Out.docx](attachments/885287/8028168.docx)

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"



// cURL example to convert PDF Document to Word

curl -v "https://api.aspose.cloud/v4.0/words/2019_new_demo.pdf/saveAs" \
-X PUT \
-d "{'SaveFormat':'docx', 'FileName': '2019_new_demo Out.docx'}" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "SaveResult": {

    "SourceDocument": {

      "Href": "http://api.aspose.cloud/v4.0/words/2019_new_demo.pdf",

      "Rel": "self",

      "Type": null,

      "Title": null

    },

    "DestDocument": {

      "Href": "2019_new_demo Out.docx",

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
# **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
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
