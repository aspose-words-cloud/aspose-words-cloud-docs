---
title: "Updating the Boorkmark Text in a document"
type: docs
url: /updating-the-boorkmark-text-in-a-document/
aliases: [/updating-the-boorkmark-text-in-a-document/]
weight: 30
---

## Introduction
This REST API allows you to update the bookmark text and returns updated bookmark data in XML/JSON format. The description of the important parameters of the API is given below:

|**Property Name**|**Type**|**Description**|
| :- | :- | :- |
|Name|string|Name of the selected bookmark |
|Text|string|The text contained within this bookmark|
## Resource URI
[Aspose.Words Cloud APIs Swagger UI](https://apireference.aspose.cloud/words/#/Bookmarks/UpdateBookmark) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there. 
## cURL Example
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to update bookmark text in a document

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/bookmarks/aspose" \
-X PUT \
-d "{'Name': 'aspose', 'Text': 'This will be the text for Aspose'}" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Bookmark": {

    "Name": "aspose",

    "Text": "This will be the text for Aspose",

    "link": {

      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/bookmarks/aspose",

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
## SDK Source
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## SDK Examples
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "PostUpdateDocumentBookmark.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostUpdateDocumentBookmark.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "update_document_bookmark.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "post_update_document_bookmark.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postUpdateDocumentBookmark.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostUpdateDocumentBookmark.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostUpdateDocumentBookmark.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "UpdateDocumentBookmark.go" >}}

{{< /tab >}}

{{< /tabs >}}
