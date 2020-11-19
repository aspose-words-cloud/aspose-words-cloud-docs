---
title: "Add comments"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /comments/add/
aliases: [/add-comment-to-a-word-document/]
description: "Add a comment to a Word document"
weight: 10
---

This REST API adds a `Comment`.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|RangeStart|link|Link to comment range start.|
|RangeEnd|link|Link to comment range end.|
|Author|string|Specifies the author's name for comment. It cannot be null.|
|Initial|string|Specifies the initials of the user associated with a specific comment. It cannot be null.|
|DateTime|DateTime|Gets the date and time that the comment was made.|
|Text|string|This is a convenience property that allows you to easily get or set the text of the comment.|
|Content|list of child nodes|List of child nodes.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Comments/InsertComment) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use `cURL` command-line tool to easily interact with Aspose.Words web services. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get add comment to a Word document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments" \
-X POST \
-d "{ 'RangeStart': { 'Node': { 'nodeId': '0.0.3' },  'Offset': 0}, 'RangeEnd': { 'Node': { 'nodeId': '0.0.3' }, 'Offset': 0}, 'Initial': 'IA', 'Author': 'Sohail', 'Text': 'A new Comment' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Comment": {
    "RangeStart": {
      "Node": {
        "Text": "Page 1",
        "NodeId": "0.0.4",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0/runs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    },
    "RangeEnd": {
      "Node": {
        "Text": "Page 1",
        "NodeId": "0.0.4",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0/runs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    },
    "Author": "Sohail",
    "Initial": "IA",
    "DateTime": "\/Date(-62135596800000)\/",
    "Text": "A new Comment\r\n",
    "Content": {
      "ChildNodes": [
        {
          "Text": "A new Comment",
          "NodeId": "6.0",
          "link": {
            "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0/paragraphs/0",
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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "PutComment.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PutComment.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "add_comment_to_document.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "put_comment.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "putComment.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PutComment.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PutComment.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "PutComment.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
