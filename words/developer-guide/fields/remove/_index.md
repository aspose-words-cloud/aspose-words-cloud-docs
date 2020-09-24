---
title: "Remove Fields from a Document"
type: docs
url: /fields/remove/
aliases: [/remove-fields-from-a-document/]
weight: 30
---

This REST API allows you to remove all fields from a document, section or paragraph.  

## REST API’s Resources

The following URIs are used to address REST resources:

```HTML
~/{file-name}/fields
~/{file-name}/{nodePath}/fields
```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to specific node in the document. If this URI is used, only elements contained within specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

The resource properties are:

|Property Name|Type|Description|
| :- | :- | :- |
|FieldCode|string|Returns field code.|
|LocaleId|int|Gets or sets LCID of the field.|
|Result|string|Returns field result.|

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Fields/DeleteFields) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

**Input Document**: [GetField.docx](attachments/885406/1180126.docx)

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to delete fields from a Document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/fields" \
-X DELETE \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
{
  "Code": 200,
  "Status": "OK"
}
```

{{< /tab >}}
{{< /tabs >}}

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

**Case 1: Delete Fields from a Document**

{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "DeleteDocumentFields.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "DeleteFields.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "delete_fields.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "delete_fields.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "deleteFields.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_DeleteFields.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_DeleteFields.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "DeleteFields.go" >}}
{{< /tab >}}
{{< /tabs >}}

**Case 2: Delete Fields from a Section**

{{< tabs tabTotal="4" tabID="6" tabName1="C#" tabName2="Android" tabName3="Swift" tabName4="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "DeleteSectionFields.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_DeleteSectionFields.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_DeleteSectionFields.swift" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "DeleteFields.go" >}}
{{< /tab >}}
{{< /tabs >}}

**Case 3: Delete Fields from a Paragraph**

{{< tabs tabTotal="3" tabID="7" tabName1="C#" tabName2="Android" tabName3="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "DeleteParagraphFields.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_DeleteParagraphFields.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_DeleteParagraphFields.swift" >}}
{{< /tab >}}
{{< /tabs >}}
