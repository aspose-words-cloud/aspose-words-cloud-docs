---
title: "Get Document Protection Info"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /documents/protection/get/
aliases: [/get-document-protection-info/]
description: "Get word document protection info"
weight: 10
---

This REST API retrieves protection information.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|ProtectionType|string|Document protection type, one from: AllowOnlyComments, AllowOnlyFormFields, AllowOnlyRevisions, ReadOnly, NoProtection.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Protection/GetDocumentProtection) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser. 

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get current document protection info
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/protection" \
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
  "ProtectionData": {
    "ProtectionType": "NoProtection"
  },
  "DocumentLink": null,
  "Code": 200,
  "Status": "OK"
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="5" tabID="4" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetDocumentProtection.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetDocumentProtection.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetDocumentProtection.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "GetDocumentProtection.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetDocumentProtection.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
