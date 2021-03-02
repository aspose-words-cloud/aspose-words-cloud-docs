---
title: "Merge"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /merge/
aliases: [/appending-a-document/]
keywords: "document append, merge"
description: "Merge Word documents. Merge DOCX, PDF, RTF into one with a single request."
weight: 180
---

Aspose provides a powerful API to merge and combine multiple documents into one. It's a common document automation task with several practical applications, that may enable greater consistency, streamline document workflows and reduce paper usage.

With this API you can join several Word documents into one, that is easier to review, print and share. For example, you can merge DOCX files and save them into a single consolidated [PDF](https://docs.fileformat.com/pdf/).

The API supports a variety of input and output formats and allows you to combine multiple [DOC](https://docs.fileformat.com/word-processing/doc/), [DOT](https://docs.fileformat.com/word-processing/dot/), [DOCX](https://docs.fileformat.com/word-processing/docx/), [DOTX](https://docs.fileformat.com/word-processing/dotx/), [RTF](https://docs.fileformat.com/word-processing/rtf/), [ODT](https://docs.fileformat.com/word-processing/odt/), [OTT](https://docs.fileformat.com/word-processing/ott/), [TXT](https://docs.fileformat.com/word-processing/txt/), [HTML](https://docs.fileformat.com/web/html/) files and download the result in [DOCX](https://docs.fileformat.com/word-processing/docx/), [PDF](https://docs.fileformat.com/pdf/), [HTML](https://docs.fileformat.com/web/html/), [EPUB](https://docs.fileformat.com/ebook/epub/), [PNG](https://docs.fileformat.com/Image/png/), [JPEG](https://docs.fileformat.com/image/jpeg/) and other formats. 
 
To append Word documents to the source document,  you need to specify their names in the `documentList` parameter. The resulting changes are saved in the source document if the `destFileName` parameter is missing.

The description of the important API parameters is given below:

|Name|Type|Description|
| :- | :- | :- |
|Href|string|Path of the document to append.|
|ImportFormatMode|string|Defines which formatting will be used: appended or destination document. Possible values are **KeepSourceFormatting** or **UseDestinationStyles**. |

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Append/AppendDocument) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [test_doc.docx](test_doc.docx), [test_multi_pages.docx](test_multi_pages.docx) and output [test_doc_output.docx](test_doc_output.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to append a document
curl -v "https://api.aspose.cloud/v4.0/words/test_doc.docx/appendDocument" \
-X PUT \
-d "{'DocumentEntries':[{'Href':'test_multi_pages.docx', 'ImportFormatMode':'KeepSourceFormatting'}]}" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Document": {
    "Links": [
      {
        "Href": "test_doc.docx",
        "Rel": "self"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=doc",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=dot",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=docx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as DOCX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=docm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.document.macroEnabled.12",
        "Title": "Download as DOCM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=dotx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",
        "Title": "Download as DOTX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=dotm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.template.macroEnabled.12",
        "Title": "Download as DOTM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=flatopc",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as FLATOPC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=rtf",
        "Rel": "alternate",
        "Type": "application/rtf",
        "Title": "Download as RTF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=wml",
        "Rel": "alternate",
        "Type": "text/xml",
        "Title": "Download as WML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=odt",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text",
        "Title": "Download as ODT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=ott",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text-template",
        "Title": "Download as OTT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=txt",
        "Rel": "alternate",
        "Type": "text/plain",
        "Title": "Download as TXT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=mhtml",
        "Rel": "alternate",
        "Type": "multipart/related",
        "Title": "Download as MHTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=epub",
        "Rel": "alternate",
        "Type": "application/epub+zip",
        "Title": "Download as EPUB"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=pdf",
        "Rel": "alternate",
        "Type": "application/pdf",
        "Title": "Download as PDF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=xps",
        "Rel": "alternate",
        "Type": "application/vnd.ms-xpsdocument",
        "Title": "Download as XPS"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=tiff",
        "Rel": "alternate",
        "Type": "image/tiff",
        "Title": "Download as TIFF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=png",
        "Rel": "alternate",
        "Type": "image/png",
        "Title": "Download as PNG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=jpeg",
        "Rel": "alternate",
        "Type": "image/jpeg",
        "Title": "Download as JPEG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=bmp",
        "Rel": "alternate",
        "Type": "image/bmp",
        "Title": "Download as BMP"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=gif",
        "Rel": "alternate",
        "Type": "image/gif",
        "Title": "Download as GIF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=svg",
        "Rel": "alternate",
        "Type": "image/svg+xml",
        "Title": "Download as SVG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=html",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=htmlfixed",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTMLFIXED"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=pcl",
        "Rel": "alternate",
        "Type": "application/x-pcl",
        "Title": "Download as PCL"
      }
    ],
    "FileName": "test_doc.docx",
    "SourceFormat": "Docx",
    "IsEncrypted": false,
    "IsSigned": false,
    "DocumentProperties": {
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx/documentProperties",
        "Rel": "self"
      }
    }
  }
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "AppendaDocument.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "AppendaDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "AppendaDocument.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "AppendaDocument.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "AppendaDocument.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "Aspose_Cloud_Words_AppendaDocument.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "AppendaDocument.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_AppendaDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_AppendaDocument.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See also

- Product page description: <a href="https://products.aspose.cloud/words/python/merge" target="_blank">Python</a>, <a href="https://products.aspose.cloud/words/net/merge" target="_blank">C#</a>, <a href="https://products.aspose.cloud/words/java/merge" target="_blank">Java</a>, <a href="https://products.aspose.cloud/words/nodejs/merge" target="_blank">Node.js</a>, <a href="https://products.aspose.cloud/words/php/merge" target="_blank">PHP</a>, <a href="https://products.aspose.cloud/words/go/merge" target="_blank">Go</a>
- <a href="https://products.aspose.app/words/merger" target="_blank">Free online merger app
