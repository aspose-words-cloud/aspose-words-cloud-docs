---
title: "Delete all Paragraph Tab Stops in a Document"
type: docs
url: /delete-all-paragraph-tab-stops-in-a-document/
aliases: [/delete-all-paragraph-tab-stops-in-a-document/]
keywords: "List of Sections,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents,Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "This REST API allows you to Delete all Paragraph Tab Stops in a Document. Please note that the SDKs of this cloud API are available in Python, C#, Java, Ruby, PHP, Node.js, Android, Swift, and Go languages."
weight: 10
---

This REST API allows you to delete all Paragraph Tab Stops in a Document. Please note that the SDKs of this cloud API are available in *Python, C#, Java, Ruby, PHP, Node.js, Android, Swift,* and *Go* languages. 

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Paragraphs/DeleteAllParagraphTabStops) lets you call this REST API directly from the browser.  

## cURL Example

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java

// Please get your App_Key and App_SID from https://dashboard.aspose.cloud/#/apps. Place your App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get a list of sections

curl -X DELETE "https://api.aspose.cloud/v4.0/words/ParagraphTabStops.docx/sections%2F0/paragraphs/0/tabstops?storage=First%20Storage"

-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java

 {
  "TabStops": [],
  "RequestId": "Root=1-5ee5043a-efea5b92b280c903d2788739"

}
```

{{< /tab >}}
{{< /tabs >}}
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "DeleteAllParagraphTabStops.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "DeleteAllParagraphTabStops.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "DeleteAllParagraphTabStops.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "DeleteAllParagraphTabStops.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "DeleteAllParagraphTabStops.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "DeleteAllParagraphTabStops.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "DeleteAllParagraphTabStops.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "DeleteAllParagraphTabStops.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "delete_all_paragraph_tab_stops.go" >}}
{{< /tab >}}
{{< /tabs >}}
