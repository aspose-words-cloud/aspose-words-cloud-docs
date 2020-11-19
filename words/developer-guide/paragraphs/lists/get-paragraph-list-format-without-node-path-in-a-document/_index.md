---
title: "Get Paragraph List Format Without Node Path in a Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /paragraphs/lists/get-paragraph-list-format-without-node-path-in-a-document/
aliases: [/get-paragraph-list-format-without-node-path-in-a-document/]
keywords: ""
description: "Get paragraph's list formatting without node path in a Word document"
weight: 30
---

This REST API gets paragraph's list formatting without node path.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/GetParagraphListFormat) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use `cURL` command-line tool to easily interact with Aspose.Words web services. The following example demonstrates how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X GET "https://api.aspose.cloud/v4.0/words/ParagraphGetListFormat.doc/paragraphs/1/listFormat?storage=First%20Storage"

-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "ListFormat": {
    "ListLevelNumber": 1,
    "ListId": 1,
    "IsListItem": true,
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/ParagraphGetListFormat.doc/sections/0/body/paragraphs/1/listFormat",
      "Rel": "self"
    }
  },
  "RequestId": "Root=1-5ee5003c-cb9aaf6c22084586e37c7428"
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "GetParagraphListFormatWithoutNodePath.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetParagraphListFormatWithoutNodePath.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetParagraphListFormatWithoutNodePath.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetParagraphListFormatWithoutNodePath.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "GetParagraphListFormatWithoutNodePath.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "GetParagraphListFormatWithoutNodePath.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "GetParagraphListFormatWithoutNodePath.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "GetParagraphListFormatWithoutNodePath.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "get_paragraph_list_format_without_path.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

