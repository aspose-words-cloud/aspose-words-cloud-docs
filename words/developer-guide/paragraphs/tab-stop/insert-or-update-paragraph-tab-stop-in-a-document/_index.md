---
title: "Insert OR Update Paragraph Tab Stop in a Document"
type: docs
url: /paragraphs/tab-stop/insert-or-update-paragraph-tab-stop-in-a-document/
aliases: [/insert-or-update-paragraph-tab-stop-in-a-document/]
keywords: "List of Sections,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents,Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "This REST API allows you to Insert OR Update Paragraph Tab Stop in a Document. Please note that the SDKs of this cloud API are available in Python, C#, Java, Ruby, PHP, Node.js, Android, Swift, and Go languages."
weight: 40
---

This REST API allows you to Insert or update the paragraph tab stop in a document. Please note that the SDKs of this cloud API are available in *Python, C#, Java, Ruby, PHP, Node.js, Android, Swift,* and *Go* languages. 

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/InsertOrUpdateParagraphTabStop) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X POST "https://api.aspose.cloud/v4.0/words/ParagraphTabStops.docx/sections%2F0/paragraphs/0/tabstops?storage=First%20Storage"

-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
  {
  "TabStops": [
    {
      "Alignment": "Left",
      "Leader": "None",
      "Position": 72,
      "IsClear": false
    },
    {
      "Alignment": "Right",
      "Leader": "Dots",
      "Position": 288,
      "IsClear": false
    }
  ],
  "RequestId": "Root=1-5ee502ba-b203480859050d704d4b91d9"
}
```

{{< /tab >}}
{{< /tabs >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "InsertOrUpdateParagraphTabStop.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "InsertOrUpdateParagraphTabStop.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "InsertOrUpdateParagraphTabStop.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "InsertOrUpdateParagraphTabStop.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "InsertOrUpdateParagraphTabStop.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "InsertOrUpdateParagraphTabStop.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "InsertOrUpdateParagraphTabStop.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "InsertOrUpdateParagraphTabStop.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "insert_or_update_paragraph_tab_stops.go" >}}
{{< /tab >}}
{{< /tabs >}}
