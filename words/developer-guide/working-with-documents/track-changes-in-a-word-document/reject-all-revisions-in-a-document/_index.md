---
title: "Reject all Revisions in a Document"
type: docs
url: /reject-all-revisions-in-a-document/
keywords: "word revision tracking, track changes, track changes in word"
description: "This REST API allows you to reject word revision tracking."
weight: 20
---




# **Introduction**
This REST API allows you to reject all revisions in a document. The request parameters are the following:

|**Parameter Name**|**Type**|**Query String/HTTP Body**|**Description**|
| :- | :- | :- | :- |
|destFileName|string|Query string: destFileName=AfterAcceptAll.doc|Result path of the document after the operation. If this parameter is omitted then the result of the operation will be saved as the source document.|
|folder|string|Query string: folder=MyFolder|Original document folder.|
|storage|string|Query string: storage=MyAmazonS3Storage|Original document storage.|
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Revisions/RejectAllRevisions) lets you call this REST API directly from the browser.  
## **cURL Example**
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \

-X POST \

-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"

// cURL example to reject all revisions in a document

curl -v "https://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/revisions/rejectAll" \

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

      "Href": "test\_multi\_pages.docx",

      "Rel": "self",

      "Type": null,

      "Title": null

    },

    "Dest": {

      "Href": "test\_multi\_pages.docx",

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
# **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "RejectAllRevisions.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "RejectAllRevisions.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "reject\_all\_revisions.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "reject\_all\_revisions.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "rejectAllRevisions.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_RejectAllRevisions.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_RejectAllRevisions.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "RejectAllRevisions.go" >}}

{{< /tab >}}

{{< /tabs >}}
