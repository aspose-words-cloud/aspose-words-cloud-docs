---
title: "Get a particular Paragraph from a Word Document"
type: docs
url: /paragraphs/get/
aliases: [/get-a-particular-paragraph-from-a-word-document/]
weight: 20
---

This REST API allows you to get a particular paragraph from a word document. The API returns a JSON/XML representation of one of the paragraphs.

## REST API’s Resources

```JAVA
~/{file-name}/paragraph/{index}
~/{file-name}/sections/{sectionIndex}/paragraphs/{index}
~/{file-name}/sections/{sectionIndex}/headersFooters/{headerFooterIndex}/paragraphs/{index}
```

*{file-name}* is the name of the Word document containing elements.
*{sectionIndex}* is the index of a section that contains paragraphs. 
*{headerFooterIndex}* is the index of a section that contains headers and footers. 
*{index}* is the index of a specific paragraph.
The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/GetParagraph) lets you call this REST API directly from a browser. 

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to get one of the paragraphs contained in the document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
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

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetDocumentParagraphByIndex.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentParagraph.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_document_paragraph.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_document_paragraph.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getDocumentParagraph.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentParagraph.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentParagraph.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentParagraph.go" >}}
{{< /tab >}}
{{< /tabs >}}