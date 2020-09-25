---
title: "Delete Paragraph List Format in a Document"
type: docs
url: /paragraphs/lists/delete-paragraph-list-format-in-a-document/
aliases: [/delete-paragraph-list-format-in-a-document/]
keywords: "List of Sections,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents,Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "This REST API allows you to Delete Paragraph List Format in a Document. Please note that the SDKs of this cloud API are available in Python, C#, Java, Ruby, PHP, Node.js, Android, Swift, and Go languages."
weight: 10
---

This REST API allows you to Delete Paragraph List Format in a Document. Please note that the SDKs of this cloud API are available in *Python, C#, Java, Ruby, PHP, Node.js, Android, Swift,* and *Go* languages. 

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/DeleteParagraph) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X DELETE "https://api.aspose.cloud/v4.0/words/ParagraphGetListFormat.doc/sections%2F0/paragraphs/1/listFormat?storage=First%20Storage"

-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

To get a **JWT** token, please, follow these [instructions](/words/getting-started/available-sdks/#curl).

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
  "ListFormat": {
    "ListLevelNumber": 0,
    "IsListItem": false,
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/ParagraphGetListFormat.doc/sections/0/body/paragraphs/1/listFormat",
      "Rel": "self"
    }
  },
  "RequestId": "Root=1-5ee500ee-74375c8e592911e28d0c7ec5"
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
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "DeleteParagraphListFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "DeleteParagraphListFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "DeleteParagraphListFormat.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "DeleteParagraphListFormat.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "DeleteParagraphListFormat.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "DeleteParagraphListFormat.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "DeleteParagraphListFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "DeleteParagraphListFormat.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "delete_paragraph_list_format.go" >}}
{{< /tab >}}
{{< /tabs >}}
