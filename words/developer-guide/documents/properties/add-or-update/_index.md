---
title: "Add New or Update Existing Document Property"
type: docs
url: /documents/properties/add-or-update/
aliases: [/add-new-or-update-existing-document-property/]
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

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DocumentProperties/CreateOrUpdateDocumentProperty) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

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

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

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

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "CreateOrUpdateDocumentProperty.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "CreateOrUpdateDocumentProperty.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "CreateOrUpdateDocumentProperty.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "CreateOrUpdateDocumentProperty.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "CreateOrUpdateDocumentProperty.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "CreateOrUpdateDocumentProperty.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_CreateOrUpdateDocumentProperty.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_CreateOrUpdateDocumentProperty.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "CreateOrUpdateDocumentProperty.go" >}}
{{< /tab >}}
{{< /tabs >}}
