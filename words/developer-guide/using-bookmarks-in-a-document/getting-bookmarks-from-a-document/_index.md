---
title: "Getting Bookmarks from a Document"
type: docs
url: /getting-bookmarks-from-a-document/
weight: 10
---

## **Introduction**
Bookmarks identify in a Microsoft Word document the locations or fragments that you name and identify for future reference. For example, you might use a bookmark to identify text that you want to revise later. Instead of scrolling through the document to locate the text, you can go to it by using the Bookmark dialog box.

Aspose.Words Cloud API allows you to obtain a bookmark collection to iterate through bookmarks or for other purposes.
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Bookmarks/GetBookmarks) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there. 
## **cURL Example**
Below cURL example shows how to obtain bookmarks from a bookmark collection. You can download a template file of this example from [here](attachments/885272/1180120.docx).

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

// cURL example to obtain bookmarks from a bookmark collection

curl -v "https://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/bookmarks" \

-X GET \

-H "Content-Type: application/json" \

-H "Accept: application/json" \

-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Bookmarks": {

    "BookmarkList": [

      {

        "Name": "\_GoBack",

        "Text": "",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/bookmarks/\_GoBack",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Name": "aspose",

        "Text": "",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/bookmarks/aspose",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Name": "page2",

        "Text": "",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/bookmarks/page2",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      }

    ],

    "link": {

      "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/bookmarks",

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
## **SDK Source**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetDocumentBookmarks.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentBookmarks.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get\_document\_bookmarks.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get\_document\_bookmarks.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getDocumentBookmarks.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_GetDocumentBookmarks.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_GetDocumentBookmarks.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentBookmarks.go" >}}

{{< /tab >}}

{{< /tabs >}}
