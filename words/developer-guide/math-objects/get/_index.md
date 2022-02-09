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

Important properties are the following:

|Property Name|Type|Description|
| :- | :- | :- |
|Content| |Content of OfficeMath object.|
|DisplayType|OfficeMathDisplayType|Specifies the display format type of the equation. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.math/officemathdisplaytype)|
|Justification|OfficeMathJustification|Specifies the justification of the equation. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.math/officemathjustification)|
|MathObjectType|MathObjectType|Specifies type of an Office Math object. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.math/mathobjecttype)|

## cURL and Postman

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

You can carry out REST API interactions using **cURL** and **Postman**. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="2" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetOfficeMathObjectOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetOfficeMathObjectOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "OfficeMathObject": {
    "Content": {
      "ChildNodes": [
        {
          "NodeId": "0.0.0.0",
          "link": {
            "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/0/OfficeMathObjects/0/OfficeMathObjects/0",
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
      "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/0/OfficeMathObjects/0",
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

## Code samples in Python, Java, C#, JavaScript, PHP, C++, Golang, Ruby, Swift, Dart

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of low-level programming details and let you focus on your primary tasks.

The following code samples show how to interact with REST API using almost any mainstream programming language:

{{< nosnippet >}}
{{< tabs tabTotal="11" tabID="5" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" tabName11="Curl" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetOfficeMathObjectOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetOfficeMathObjectOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetOfficeMathObjectOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetOfficeMathObjectOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetOfficeMathObjectOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetOfficeMathObjectOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetOfficeMathObjectOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetOfficeMathObjectOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetOfficeMathObjectOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetOfficeMathObjectOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
