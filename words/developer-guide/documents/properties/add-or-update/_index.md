---
title: "Add New or Update Existing Document Property"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /documents/properties/add-or-update/
aliases: [/add-new-or-update-existing-document-property/]
description: "Add a new or update an existing document property"
weight: 10
---

This REST API adds a new or updates an existing document property.

A document property is described by the following format:

|Property Name|Description|
| :- | :- |
|Name|The name of the property.|
|Value|The value of the property.|
|BuiltIn|A value indicating whether the property is a built-in type. Values - 1 = True, 0 = False.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DocumentProperties/CreateOrUpdateDocumentProperty) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to update an existing document property
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/AsposeAuthor?destFileName=updated_document.docx" \
-X PUT \
-d "{ 'Name': 'Author', 'Value': 'Sohail', 'BuiltIn': false, 'link': null }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "DocumentProperty": {
    "Name": "AsposeAuthor",
    "Value": "Sohail",
    "BuiltIn": false,
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/updated_document.docx/documentProperties/AsposeAuthor",
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

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "CreateOrUpdateDocumentProperty.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "CreateOrUpdateDocumentProperty.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "CreateOrUpdateDocumentProperty.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "CreateOrUpdateDocumentProperty.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "CreateOrUpdateDocumentProperty.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "CreateOrUpdateDocumentProperty.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "CreateOrUpdateDocumentProperty.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_CreateOrUpdateDocumentProperty.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_CreateOrUpdateDocumentProperty.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
