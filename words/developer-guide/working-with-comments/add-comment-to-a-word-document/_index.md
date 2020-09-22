---
title: "Add Comment to a Word Document"
type: docs
url: /add-comment-to-a-word-document/
aliases: [/add-comment-to-a-word-document/]
weight: 30
---

The REST API allows you to add a comment to a Word Document. The API return added comment data in XML/JSON format. The resource properties are given below:

|Property Name|Type|Description|
| :- | :- | :- |
|RangeStart|link|Link to comment range start.|
|RangeEnd|link|Link to comment range end.|
|Author|string|Specifies the author's name for comment. It cannot be null.|
|Initial|string|Specifies the initials of the user associated with a specific comment. It cannot be null.|
|DateTime|DateTime|Gets the date and time that the comment was made.|
|Text|string|This is a convenience property that allows you to easily get or set the text of the comment.|
|Content|list of child nodes|List of child nodes.|

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Comments/InsertComment) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there.

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

// cURL example to get add comment to a word document

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments" \
-X POST \
-d "{ 'RangeStart': { 'Node': { 'nodeId': '0.0.3' },  'Offset': 0}, 'RangeEnd': { 'Node': { 'nodeId': '0.0.3' }, 'Offset': 0}, 'Initial': 'IA', 'Author': 'Sohail', 'Text': 'A new Comment' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

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

## SDK Source

Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.

## SDK Examples

Code examples for various SDKs are presented below:
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
