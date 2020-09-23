---
title: "Get a OfficeMath Object from Document"
type: docs
url: /get-a-officemath-object-from-document/
aliases: [/get-a-officemath-object-from-document/]
weight: 20
---

This REST API allows you to get one of the OfficeMath objects that are defined in the document. The Resource Properties are:

|Property Name|Type|Description|
| :- | :- | :- |
|Content| |Content of OfficeMath object.|
|DisplayType|OfficeMathDisplayType|Specifies the display format type of the equation. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.math/officemathdisplaytype)|
|Justification|OfficeMathJustification|Specifies the justification of the equation. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.math/officemathjustification)|
|MathObjectType|MathObjectType|Specifies type of an Office Math object. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.math/mathobjecttype)|

## REST API’s Resources

```JAVA
~/{file-name}/officeMathObjects/{index}
~/{file-name}/{nodePath}/officeMathObjects/{index}
```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to a specific node in the document. If this URI is used, only elements contained within a specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

*{index}* is the index of specific office math object.
The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/OfficeMathObjects/GetOfficeMathObject) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

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

# cURL example to get one of the OfficeMath objects defined in the document
curl -v "https://api.aspose.cloud/v4.0/words/MathObjects.docx/OfficeMathObjects/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
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

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

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
