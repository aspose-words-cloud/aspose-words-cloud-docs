---
title: "Get Image Data"
second_title: "Drawing Objects in a Word Document"
type: docs
url: /drawing-objects/get-image-data/
aliases: [/get-image-data-from-a-drawing-object/]
description: "Get image data from a drawing object in a Word document"
weight: 50
---

This REST API retrieves image data from a `DrawingObject`.

## REST API

```JAVA
~/{file-name}/drawingObjects/{index}/imageData

~/{file-name}/{nodePath}/drawingObjects/{index}/imageData
```
, where:

- *{file-name}* is a filename of a document.
- *{nodePath}* is a path to a node in a document. If this parameter is used, elements contained within a specified node will be processed:
  - *sections/{sectionIndex}* - references a section.
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.
- *{index}* is an index of a specific drawing object.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DrawingObjects/GetDocumentDrawingObjectImageData) lets you call this REST API directly from a browser. 

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get image data from a drawing object
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/drawingObjects/0/imageData" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o image.png
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
image.png file
```

{{< /tab >}}
{{< /tabs >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetDocumentDrawingObjectImageData.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentDrawingObjectImageData.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_document_drawing_object_image_data.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_document_drawing_object_image_data.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getDocumentDrawingObjectImageData.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentDrawingObjectImageData.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentDrawingObjectImageData.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentDrawingObjectImageData.go" >}}
{{< /tab >}}
{{< /tabs >}}
