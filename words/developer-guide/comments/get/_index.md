---
title: "Get"
second_title: "Comments in a Word Document"
type: docs
url: /comments/get/
aliases: [/get-comment-from-word-document/]
weight: 30
---

This REST API retrieves a `Comment`.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|RangeStart|link|Link to comment range start.|
|RangeEnd|link|Link to comment range end.|
|Author|string|Specifies the author's name for comment. It cannot be null.|
|Initial|string|Specifies the initials of the user associated with a specific comment. It cannot be null.|
|DateTime|DateTime|Gets the date and time that the comment was made.|
|Text|string|This is a convenience property that allows you to easily specify the text of the comment.|
|Content|list of child nodes|List of child nodes.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Comments/GetComment) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a comment from word document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Comment": {
    "RangeStart": {
      "Node": {
        "Text": "Testing ",
        "NodeId": "0.0.1",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0/runs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    },
    "RangeEnd": {
      "Node": {
        "Text": "Testing ",
        "NodeId": "0.0.1",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0/runs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    },
    "Author": "Евгений Иванов",
    "Initial": "ЕИ",
    "DateTime": "\/Date(1502450580000)\/",
    "Text": "Comment 1\r\n\r\n",
    "Content": {
      "ChildNodes": [
        {
          "Text": "Comment 1",
          "NodeId": "6.0",
          "link": {
            "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0/paragraphs/0",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        },
        {
          "Text": "",
          "NodeId": "6.1",
          "link": {
            "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0/paragraphs/1",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        }
      ]
    },
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0",
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

## Cloud SDK Family

Using an SDK is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetComment.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetComment.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_comment.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_comment.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getComment.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetComment.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetComment.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetComment.go" >}}
{{< /tab >}}
{{< /tabs >}}
