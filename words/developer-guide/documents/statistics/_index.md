---
title: "Get Document Statistics"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /documents/statistics/
aliases: [/get-document-statistics/]
description: "Get statistical information from a Word document."
weight: 40
---

This REST API retrieves statistical information from a document.

The request parameters are the following:

|Parameter Name|Type|Query String/HTTPBody|Description|
| :- | :- | :- | :- |
|includeComments|bool|Query String: includeComments=true|Support including/excluding comments from the WordCount. The default value is "false".|
|includeFootnotes|bool|Query String: includeFootnotes=true|Support including/excluding footnotes from the WordCount. The default value is "false".|
|includeTextInShapes|bool|Query String: includeTextInShapes=true|Support including/excluding shape's text from the WordCount. The default value is "false".|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Statistics/GetDocumentStatistics) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get the statistical data of the document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/statistics" \
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
  "StatData": {
    "WordCount": 24,
    "ParagraphCount": 5,
    "PageCount": 3,
    "FootnotesStatData": {
      "WordCount": 0,
      "ParagraphCount": 0
    },
    "PageStatData": [
      {
        "PageNumber": 1,
        "WordCount": 4,
        "ParagraphCount": 2,
        "FootnotesStatData": null
      },
      {
        "PageNumber": 2,
        "WordCount": 9,
        "ParagraphCount": 1,
        "FootnotesStatData": null
      },
      {
        "PageNumber": 3,
        "WordCount": 11,
        "ParagraphCount": 2,
        "FootnotesStatData": null
      }
    ]
  },
  "DocumentLink": {
    "Href": "test_multi_pages.docx",
    "Rel": "self",
    "Type": null,
    "Title": null
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
{{< tabs tabTotal="5" tabID="4" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetDocumentStatistics.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetDocumentStatistics.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetDocumentStatistics.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetDocumentStatistics.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetDocumentStatistics.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
