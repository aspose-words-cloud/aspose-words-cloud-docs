---
title: "Get"
second_title: "Bookmarks in a Word Document"
type: docs
url: /bookmarks/get/
aliases: [/getting-bookmarks-from-a-document/]
description: "Get bookmarks in a Word document"
weight: 10
---

Bookmarks identify in a Microsoft Word document the locations or fragments that you name and identify for future reference. For example, you might use a bookmark to identify text that you want to revise later. Instead of scrolling through the document to locate the text, you can go to it by using the Bookmark dialog box.

Aspose.Words Cloud API allows you to obtain a bookmark collection to iterate through bookmarks or for other purposes.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Bookmarks/GetBookmarks) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL, supplied with a sample document [test_multi_pages.docx](test_multi_pages.docx).

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to obtain bookmarks from a bookmark collection
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/bookmarks" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Bookmarks": {
    "BookmarkList": [
      {
        "Name": "_GoBack",
        "Text": "",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/bookmarks/_GoBack",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "aspose",
        "Text": "",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/bookmarks/aspose",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "page2",
        "Text": "",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/bookmarks/page2",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/bookmarks",
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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< nosnippet >}}
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetDocumentBookmarks.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentBookmarks.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_document_bookmarks.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_document_bookmarks.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getDocumentBookmarks.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentBookmarks.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentBookmarks.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentBookmarks.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
