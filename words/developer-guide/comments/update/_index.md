---
title: "Update Comments"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /comments/update/
aliases: [/update-the-comment-in-a-word-document/]
description: "Update a comment in a Word document"
weight: 50
---

This REST API updates a `Comment`.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|RangeStart|link|Link to comment range start.|
|RangeEnd|link|Link to comment range end.|
|Author|string|Specifies the author's name for comment. It cannot be null.|
|Initial|string|Specifies the initials of the user associated with a specific comment. It cannot be null.|
|DateTime|DateTime|Gets the date and time that the comment was made.|
|Text|string|This is a convenience property that allows you to easily get or set the text of the comment.|
|Content|list of child nodes|List of child nodes.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Comments/UpdateComment) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to update the comment
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0" \
-X PUT \
-d "{ 'RangeStart': { 'Node': { 'nodeId': '0.0.3' }, 'Offset': 0}, 'RangeEnd': { 'Node': { 'nodeId': '0.0.3' }, 'Offset': 0}, 'Initial': 'IA', 'Author': 'Sohail', 'Text': 'A new Comment' }" \
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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="5" tabID="4" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "PostComment.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "PostComment.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateComment.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_PostComment.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_PostComment.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
