---
title: "Apply Style from Document Element"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /styles/apply/
aliases: [/apply-style-from-document-element/]
keywords: ""
description: "Apply a style from an element in a Word document"
weight: 10
---

This REST API applies a style from a document element.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Styles/GetStyles) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X PUT "https://api.aspose.cloud/v4.0/words/TestApplyStyleToDocumentElement.docx/paragraphs%2F1%2FparagraphFormat/style?storage=First%20Storage" 

-H  "Content-Type: application/json" -d "{\"StyleName\":\"Heading 1\"}"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "RequestId": "Root=1-5ee50c87-0df701e079e69dfc36890778"
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
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "ApplyStyleToDocumentElement.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "ApplyStyleToDocumentElement.php" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "style-to-element.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

