---
title: "Update"
second_title: "Comments in a Word Document"
type: docs
url: /comments/update/
aliases: [/update-the-comment-in-a-word-document/]
weight: 40
---

The REST API allows you to update the comment in a Word Document. The API returns updated comment data in XML/JSON format. Moreover, resource properties are given below:

|Property Name|Type|Description|
| :- | :- | :- |
|RangeStart|link|Link to comment range start.|
|RangeEnd|link|Link to comment range end.|
|Author|string|Specifies the author's name for comment. It cannot be null.|
|Initial|string|Specifies the initials of the user associated with a specific comment. It cannot be null.|
|DateTime|DateTime|Gets the date and time that the comment was made.|
|Text|string|This is a convenience property that allows you to easily get or set the text of the comment.|
|Content|list of child nodes|List of child nodes.|

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Comments/UpdateComment) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to update the comment
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0" \
-X PUT \
-d "{ 'RangeStart': { 'Node': { 'nodeId': '0.0.3' }, 'Offset': 0}, 'RangeEnd': { 'Node': { 'nodeId': '0.0.3' }, 'Offset': 0}, 'Initial': 'IA', 'Author': 'Sohail', 'Text': 'A new Comment' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
{
  "Comment": {
    "RangeStart": null,
    "RangeEnd": null,
    "Author": "Sohail",
    "Initial": "IA",
    "DateTime": "\/Date(-62135596800000)\/",
    "Text": "A new Comment\r\n",
    "Content": {
      "ChildNodes": [
        {
          "Text": "A new Comment",
          "NodeId": "2.0",
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

Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "PostComment.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostComment.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "update_comment.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "post_comment.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postComment.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostComment.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostComment.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "UpdateComment.go" >}}
{{< /tab >}}
{{< /tabs >}}