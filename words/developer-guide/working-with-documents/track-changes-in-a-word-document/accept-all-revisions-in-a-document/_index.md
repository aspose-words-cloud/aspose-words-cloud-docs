---
title: "Accept all Revisions in a Document"
type: docs
url: /accept-all-revisions-in-a-document/
aliases: [/accept-all-revisions-in-a-document/]
keywords: "word revision tracking, track changes, track changes in word"
description: "This REST API allows you to accept word revision tracking."
weight: 10
---

This REST API allows you to accept all revisions in a document. The request parameters are the following:

|Parameter Name|Type|Query String/HTTP Body|Description|
| :- | :- | :- | :- |
|destFileName|string|Query string: destFileName=AfterAcceptAll.doc|Result path of the document after the operation. If this parameter is omitted then the result of the operation will be saved as the source document.|
|folder|string|Query string: folder=MyFolder|Original document folder.|
|storage|string|Query string: storage=MyAmazonS3Storage|Original document storage.|

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Revisions/AcceptAllRevisions) lets you call this REST API directly from the browser.  

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

// cURL example to accept all revisions in a document

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/revisions/acceptAll" \
-X PUT \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Content-Length: 0" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Result": {

    "Source": {

      "Href": "test_multi_pages.docx",

      "Rel": "self",

      "Type": null,

      "Title": null

    },

    "Dest": {

      "Href": "test_multi_pages.docx",

      "Rel": "result",

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

## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "AcceptAllRevisions.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "AcceptAllRevisions.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "accept_all_revisions.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "accept_all_revisions.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "acceptAllRevisions.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_AcceptAllRevisions.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_AcceptAllRevisions.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "RevisionsAll.go" >}}

{{< /tab >}}

{{< /tabs >}}
