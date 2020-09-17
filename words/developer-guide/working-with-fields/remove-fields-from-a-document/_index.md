---
title: "Remove Fields from a Document"
type: docs
url: /remove-fields-from-a-document/
weight: 30
---

# **Introduction**
This REST API allows you to remove all fields from a document, section or paragraph.  
## **Resource URI**
```html

~/{file-name}/fields

~/{file-name}/{nodePath}/fields

```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to specific node in the document. If this URI is used, only elements contained within specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

The resource properties are:

|**Property Name**|**Type**|**Description**|
| :- | :- | :- |
|FieldCode|string|Returns field code.|
|LocaleId|int|Gets or sets LCID of the field.|
|Result|string|Returns field result.|
[Swagger UI](https://apireference.aspose.cloud/words/#/Fields/DeleteFields) lets you call this REST API directly from the browser.  
## **cURL Example**
**Input Document:** [GetField.docx](attachments/885406/1180126.docx)

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to delete fields from a Document

curl -v "https://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/fields" \
-X DELETE \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Code": 200,

  "Status": "OK"

}

```

{{< /tab >}}

{{< /tabs >}}
# **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
**Case 1: Delete Fields from a Document**

{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "DeleteDocumentFields.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "DeleteFields.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "delete\_fields.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "delete\_fields.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "deleteFields.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_DeleteFields.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_DeleteFields.swift" >}}

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

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_DeleteSectionFields.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_DeleteSectionFields.swift" >}}

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

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_DeleteParagraphFields.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_DeleteParagraphFields.swift" >}}

{{< /tab >}}

{{< /tabs >}}

