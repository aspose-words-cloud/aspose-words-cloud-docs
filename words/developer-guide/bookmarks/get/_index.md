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

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Bookmarks/GetBookmarks) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [test_multi_pages.docx](test_multi_pages.docx) to figure out the details.

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
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

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

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="5" tabID="4" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetDocumentBookmarks.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetDocumentBookmarks.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetDocumentBookmarks.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetDocumentBookmarks.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetDocumentBookmarks.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
