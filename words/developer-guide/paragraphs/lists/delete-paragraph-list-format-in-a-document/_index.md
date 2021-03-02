---
title: "Delete Paragraph List Format in a Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /paragraphs/lists/delete-paragraph-list-format-in-a-document/
aliases: [/delete-paragraph-list-format-in-a-document/]
keywords: ""
description: "Delete paragraph's list formatting in a Word document"
weight: 10
---

This REST API deletes paragraph's list formatting.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/DeleteParagraph) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X DELETE "https://api.aspose.cloud/v4.0/words/ParagraphGetListFormat.doc/sections%2F0/paragraphs/1/listFormat?storage=First%20Storage"

-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
  "ListFormat": {
    "ListLevelNumber": 0,
    "IsListItem": false,
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/ParagraphGetListFormat.doc/sections/0/body/paragraphs/1/listFormat",
      "Rel": "self"
    }
  },
  "RequestId": "Root=1-5ee500ee-74375c8e592911e28d0c7ec5"
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="4" tabName1="C#" tabName2="PHP" tabName3="Golang" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "DeleteParagraphListFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "DeleteParagraphListFormat.php" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "delete_paragraph_list_format.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
