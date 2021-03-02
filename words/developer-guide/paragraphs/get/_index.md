---
title: "Get"
second_title: "Paragraphs in a Document"
type: docs
url: /paragraphs/get/
aliases: [/get-a-particular-paragraph-from-a-word-document/]
description: "Get a paragraph in a Word document"
weight: 30
---

This REST API retrieves a `Paragraph`.

## REST API

```JAVA
~/{file-name}/paragraph/{index}
~/{file-name}/sections/{sectionIndex}/paragraphs/{index}
~/{file-name}/sections/{sectionIndex}/headersFooters/{headerFooterIndex}/paragraphs/{index}
```
, where:

- *{file-name}* is a filename of a document.
- *{sectionIndex}* is an index of a section.
- *{headerFooterIndex}* is an index of a section, that contains headers and footers.
- *{index}* is an index of a specific paragraph.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/GetParagraph) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser. 

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get one of the paragraphs contained in the document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Paragraph": {
    "ChildNodes": [
      {
        "Text": "Testing ",
        "NodeId": "0.0.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0/runs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "Page 1",
        "NodeId": "0.0.1",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0/runs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "NodeId": "0.0",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0",
      "Rel": "self",
      "Type": null,
      "Title": null
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

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="5" tabID="5" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetDocumentParagraph.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetDocumentParagraphByIndex.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetDocumentParagraph.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetDocumentParagraph.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetDocumentParagraph.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
