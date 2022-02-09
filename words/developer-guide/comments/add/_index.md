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

You can use **cURL** and **Postman** to access Aspose.Words Cloud API. The following examples demonstate how to do it. Please refer to the <a href="/words/getting-started/quickstart/">instructions</a> to get a 'JWT_TOKEN' for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "InsertCommentOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "InsertCommentOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "Comment": {
    "RangeStart": {
      "Node": {
        "Text": "Page 1",
        "NodeId": "0.0.4",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0/runs/1",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0/runs/1",
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
            "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0/paragraphs/0",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        }
      ]
    },
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0",
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
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "InsertCommentOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "InsertCommentOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "InsertCommentOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "InsertCommentOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "InsertCommentOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "InsertCommentOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "InsertCommentOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "InsertCommentOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "InsertCommentOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "InsertCommentOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
