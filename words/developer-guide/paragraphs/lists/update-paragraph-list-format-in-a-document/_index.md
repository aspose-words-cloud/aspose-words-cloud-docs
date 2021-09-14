---
title: "Update Paragraph List Format in a Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /paragraphs/lists/update-paragraph-list-format-in-a-document/
aliases: [/update-paragraph-list-format-in-a-document/]
keywords: ""
description: "Update a paragraph's list format in a Word document"
weight: 40
---

This REST API updates a paragraph's list format.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/UpdateParagraphListFormat) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X PUT "https://api.aspose.cloud/v4.0/words/ParagraphUpdateListFormat.doc/sections%2F0/paragraphs/0/listFormat?storage=First%20Storage"

-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "ListFormat": {
    "ListLevelNumber": 0,
    "ListId": 2,
    "IsListItem": true,
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/ParagraphUpdateListFormat.doc/sections/0/body/paragraphs/0/listFormat",
      "Rel": "self"
    }
  },
  "RequestId": "Root=1-5ee4ff3c-2e50ac699016b63751afbeab"
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
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateParagraphListFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "UpdateParagraphListFormat.php" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateParagraphListFormat.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
