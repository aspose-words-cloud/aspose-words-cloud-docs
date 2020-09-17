---
title: "Get Hyperlink from a Document"
type: docs
url: /get-hyperlink-from-a-document/
weight: 10
---

# **Introduction**
This REST API allows you to get a hyperlink from a document. The resource properties are:

|**Property Name**|**Type**|**Description**|
| :- | :- | :- |
|Id|int|Hyperlink identifier.|
|DisplayText|string|Text of the hyperlink as it is presented in a Word document.|
|Value|string|Destination of the hyperlink.|
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Hyperlinks/GetDocumentHyperlinkByIndex) lets you call this REST API directly from the browser.  
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

// cURL example to get hyperlink from the document

curl -v "https://api.aspose.cloud/v4.0/words/test\_doc.docx/hyperlinks/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Hyperlink": {

    "DisplayText": "Aspose",

    "Value": "http://www.aspose.com/",

    "link": {

      "Href": "http://api.aspose.cloud/v4.0/words/test\_doc.docx/hyperlinks/0",

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
# **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetDocumentHyperlinkByIndex.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentHyperlinkByIndex.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get\_document\_hyperlink\_by\_index.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get\_document\_hyperlink\_by\_index.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getDocumentHyperlinkByIndex.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_GetDocumentHyperlinkByIndex.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_GetDocumentHyperlinkByIndex.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentHyperlinkByIndex.go" >}}

{{< /tab >}}

{{< /tabs >}}
