---
title: "Get a OfficeMath Object from Document"
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

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/OfficeMathObjects/GetOfficeMathObject) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

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

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

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

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< nosnippet >}}
{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetOfficeMathObject.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetOfficeMathObject.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_office_math_object.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_office_math_object.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getOfficeMathObject.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetOfficeMathObject.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetOfficeMathObject.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetOfficeMathObject.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
