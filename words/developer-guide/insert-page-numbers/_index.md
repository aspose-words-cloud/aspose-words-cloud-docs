---
title: "Page Numbers"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /insert-page-numbers/
aliases: [/insert-page-numbers-in-a-document/]
keywords: "page numbers in word, Microsoft Word page numbers, how to add page numbers in Word, add page numbers to Word"
description: "Insert page numbers into a Word document"
weight: 190
---

This REST API inserts page numbers into a document.

## REST API

```JAVA
~/{file-name}/insertPageNumbers

or

~/{file-name}/insertPageNumbers?destFileName={DestDocumentName}
```

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/PageNumbers/InsertPageNumbers) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to insert page numbers into a document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/insertPageNumbers" \
-X PUT \
-d "{ 'Format': '{PAGE} of {NUMPAGES}', 'Alignment': 'right', 'IsTop': true, 'SetPageNumberOnFirstPage': true }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Document": {
    "Links": [
      {
        "Href": "test_multi_pages.docx",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=doc",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOC"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=dot",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOT"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=docx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as DOCX"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=docm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.document.macroEnabled.12",
        "Title": "Download as DOCM"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=dotx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",
        "Title": "Download as DOTX"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=dotm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.template.macroEnabled.12",
        "Title": "Download as DOTM"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=flatopc",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as FLATOPC"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=rtf",
        "Rel": "alternate",
        "Type": "application/rtf",
        "Title": "Download as RTF"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=wml",
        "Rel": "alternate",
        "Type": "text/xml",
        "Title": "Download as WML"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=odt",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text",
        "Title": "Download as ODT"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=ott",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text-template",
        "Title": "Download as OTT"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=txt",
        "Rel": "alternate",
        "Type": "text/plain",
        "Title": "Download as TXT"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=mhtml",
        "Rel": "alternate",
        "Type": "multipart/related",
        "Title": "Download as MHTML"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=epub",
        "Rel": "alternate",
        "Type": "application/epub+zip",
        "Title": "Download as EPUB"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=pdf",
        "Rel": "alternate",
        "Type": "application/pdf",
        "Title": "Download as PDF"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=xps",
        "Rel": "alternate",
        "Type": "application/vnd.ms-xpsdocument",
        "Title": "Download as XPS"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=tiff",
        "Rel": "alternate",
        "Type": "image/tiff",
        "Title": "Download as TIFF"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=png",
        "Rel": "alternate",
        "Type": "image/png",
        "Title": "Download as PNG"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=jpeg",
        "Rel": "alternate",
        "Type": "image/jpeg",
        "Title": "Download as JPEG"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=bmp",
        "Rel": "alternate",
        "Type": "image/bmp",
        "Title": "Download as BMP"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=gif",
        "Rel": "alternate",
        "Type": "image/gif",
        "Title": "Download as GIF"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=svg",
        "Rel": "alternate",
        "Type": "image/svg+xml",
        "Title": "Download as SVG"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=html",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTML"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=htmlfixed",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTMLFIXED"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=pcl",
        "Rel": "alternate",
        "Type": "application/x-pcl",
        "Title": "Download as PCL"
      }
    ],
    "FileName": "test_multi_pages.docx",
    "SourceFormat": 4,
    "IsEncrypted": false,
    "IsSigned": false,
    "DocumentProperties": {
      "List": null,
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    }
  },
  "Code": 200,
  "Status": "OK"
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< nosnippet >}}
{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "InsertPageNumbers.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostInsertPageNumbers.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "post_insert_page_numbers.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "insert_page_numbers.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postInsertPageNumbers.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostInsertPageNumbers.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostInsertPageNumbers.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "InsertPageNumbers.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
