---
title: "Get all"
second_title: "Fields in a Document"
type: docs
url: /fields/get-all/
aliases: [/get-all-fields-from-a-document/]
description: "Get all fields from a Word document"
weight: 40
---

This REST API retrieves a collection of `Field` items from a document.

## REST API

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

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|FieldCode|string|Returns field code.|
|LocaleId|int|Gets or sets LCID of the field.|
|Result|string|Returns field result.|

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Fields/GetFields) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [GetField.docx](/words/fields/GetField.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
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
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="5" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetFieldsOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetFieldsOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetFieldsOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetFieldsOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetFieldsOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetFieldsOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetFieldsOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetFieldsOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetFieldsOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetFieldsOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
