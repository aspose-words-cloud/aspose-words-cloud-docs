---
title: "Add New or Update Existing Document Property"
type: docs
url: /add-new-or-update-existing-document-property/
aliases: [/add-new-or-update-existing-document-property/]
weight: 30
---

This REST API allows you to add new or update existing document property. The details of resource properties are given below:

|Property Name|Description|
| :- | :- |
|Name|The name of the property.  <br>Two properties cannot have the same name; attempts to create one would return a 400 BadRequest.  <br>BuiltIn property names cannot be changed; attempts to create one would return a 400 BadRequest|
|Value|The value of the property.|
|BuiltIn|A value indicating whether the property is a built-in type. Values - 1 = True, 0 = No.|

## Resource URI

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DocumentProperties/CreateOrUpdateDocumentProperty) lets you call this REST API directly from a browser.

## cURL Example

cUrl is a popular command-line utility for transferring data and a perfect tool for testing REST APIs. The following are a few examples of using cURL.

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to update an existing document property
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/AsposeAuthor?destFileName=updated_document.docx" \
-X PUT \
-d "{ 'Name': 'Author', 'Value': 'Sohail', 'BuiltIn': false, 'link': null }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
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
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

The code examples of using this REST API with various SDKs are presented below:

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
