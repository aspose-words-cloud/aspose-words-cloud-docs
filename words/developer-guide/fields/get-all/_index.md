---
title: "Get all"
second_title: "Fields in a Document"
type: docs
url: /fields/get-all/
aliases: [/get-all-fields-from-a-document/]
weight: 40
---

This REST API allows you to get all fields that are defined in the document, section or paragraph.  

## REST API’s Resources

The following URIs are used to address REST resources:

```HTML
~/{file-name}/fields
~/{file-name}/{nodePath}/fields
```
, where:
- *{file-name}* is a filename of a document.
- *{nodePath}* is a path to a node in a document. If this parameter is used, elements contained within a specified node will be processed:
  - *sections/{sectionIndex}* - references a section.
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.

The resource properties are:

|Property Name|Type|Description|
| :- | :- | :- |
|FieldCode|string|Returns field code.|
|LocaleId|int|Gets or sets LCID of the field.|
|Result|string|Returns field result.|

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Fields/GetFields) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL. You can use a sample **Input Document** [GetField.docx](/words/fields/GetField.docx).

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get all Fields from a Document
curl -v "https://api.aspose.cloud/v4.0/words/GetField.docx/sections/0/paragraphs/0/fields" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

To get a JWT-token, please, follow these [instructions](/words/getting-started/available-sdks/#curl).

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Fields": {
    "List": [
      {
        "Result": "1",
        "LocaleId": "1049",
        "FieldCode": "{ PAGE }",
        "NodeId": "0.0.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/GetField.docx/sections/0/paragraphs/0/fields/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/GetField.docx/sections/0/paragraphs/0/fields",
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

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetFieldsFromDocument.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetFields.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_fields.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_fields.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getFields.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetFields.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetFields.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetFields.go" >}}
{{< /tab >}}
{{< /tabs >}}
