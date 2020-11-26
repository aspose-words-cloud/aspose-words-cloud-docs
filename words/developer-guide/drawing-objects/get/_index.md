---
title: "Get"
second_title: "Drawing Objects in a Word Document"
type: docs
url: /drawing-objects/get/
aliases: [/get-a-particular-drawing-object/]
description: "Get a drawing object from a Word document"
weight: 30
---

This REST API retrieves a `DrawingObject`. You can also convert a `DrawingObject` to a required format.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|Width|double|Width of drawing object.|
|Height|double|Height of drawing object.|
|Left|double|Position of the left edge of the containing block of the drawing object.|
|RelativeHorizontalPosition|RelativeHorizontalPosition|Specifies what the horizontal position of a shape or text frame is relative. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.drawing/relativehorizontalposition)|
|Top|double|Position of the top edge of the containing block of the drawing object.|
|RelativeVerticalPosition|RelativeVerticalPosition|Specifies what the vertical position of a shape or text frame is relative. See possible values and more info at [.NET API Reference.](https://apireference.aspose.com/net/words/aspose.words.drawing/relativeverticalposition)|
|WrapType|WrapType|Specifies how text is wrapped around a shape or picture. See possible values and more info at [.NET API Reference](https://apireference.aspose.com/net/words/aspose.words.drawing/wraptype).|
|imageDataLink|link|Link to embedded image resource, if present.|
|oleDataLink|link|Link to embedded OLE resource, if present.|

## REST API

The following URIs are used to address REST resources:

```HTML
~/{file-name}/drawingObjects/{index}
~/{file-name}/{nodePath}/drawingObjects/{index}
```
, where:

- *{file-name}* is a filename of a document.
- *{nodePath}* is a path to a node in a document. If this parameter is used, elements contained within a specified node will be processed:
  - *sections/{sectionIndex}* - references a section.
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.
- *{index}* is an index of a drawing object.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DrawingObjects/GetDocumentDrawingObjectByIndex) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser. 

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [test_multi_pages.docx](test_multi_pages.docx) and output [drawingObject.png](drawingObject.png) files designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a particular drawing object in a PNG format
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/drawingObjects/0?format=png" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o drawingObject.png
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
drawingObject.png file
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
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetDocumentDrawingObjectByIndex.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetDocumentDrawingObjectByIndexWithFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetDocumentDrawingObjectByIndex.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetDocumentDrawingObjectByIndex.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetDocumentDrawingObjectByIndex.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
