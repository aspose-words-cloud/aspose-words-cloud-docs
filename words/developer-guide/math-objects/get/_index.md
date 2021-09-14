---
title: "Get a OfficeMath Object from Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /math-objects/get/
aliases: [/get-a-officemath-object-from-document/]
description: "Get an officemath object from a Word document"
weight: 10
---

This REST API retrieves an `OfficeMath` object.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|Content| |Content of OfficeMath object.|
|DisplayType|OfficeMathDisplayType|Specifies the display format type of the equation. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.math/officemathdisplaytype)|
|Justification|OfficeMathJustification|Specifies the justification of the equation. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.math/officemathjustification)|
|MathObjectType|MathObjectType|Specifies type of an Office Math object. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.math/mathobjecttype)|

## REST API

```JAVA
~/{file-name}/officeMathObjects/{index}
~/{file-name}/{nodePath}/officeMathObjects/{index}
```
, where:

- *{file-name}* is a filename of a document.
- *{nodePath}* is a path to a node in a document. If this parameter is used, elements contained within a specified node will be processed:
  - *sections/{sectionIndex}* - references a section.
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.
- *{index}* is an index of a office math object.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/OfficeMathObjects/GetOfficeMathObject) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get one of the OfficeMath objects defined in the document
curl -v "https://api.aspose.cloud/v4.0/words/MathObjects.docx/OfficeMathObjects/0" \
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
  "OfficeMathObject": {
    "Content": {
      "ChildNodes": [
        {
          "NodeId": "0.0.0.0",
          "link": {
            "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/0/OfficeMathObjects/0/OfficeMathObjects/0",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        }
      ]
    },
    "DisplayType": "Display",
    "Justification": "CenterGroup",
    "MathObjectType": "OMathPara",
    "NodeId": "0.0.0",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/0/OfficeMathObjects/0",
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
{{< tabs tabTotal="5" tabID="5" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetOfficeMathObject.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetOfficeMathObject.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetOfficeMathObject.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "GetOfficeMathObject.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetOfficeMathObject.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
