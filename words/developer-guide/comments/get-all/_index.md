---
title: "Get all comments"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /comments/get-all/
aliases: [/get-all-comments-from-a-word-document/]
description: "Get all comments from a Word document"
weight: 40
---

This REST API retrieves a collection of `Comment` items from a document.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Comments/GetComments) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get all comments from a Word document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments" \
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
  "Comments": {
    "CommentList": [
      {
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
              "NodeId": "4.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            },
            {
              "Text": "",
              "NodeId": "4.1",
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
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments",
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
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetComments.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetComments.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetComments.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetComments.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetComments.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
