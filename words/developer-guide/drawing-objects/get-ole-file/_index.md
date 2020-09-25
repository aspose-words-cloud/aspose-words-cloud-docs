---
title: "Get OLE file"
second_title: "Drawing Objects in a Word Document"
type: docs
url: /drawing-objects/get-ole-file/
aliases: [/get-ole-file-from-a-drawing-object/]
weight: 60
---

This REST API allows you to get an embedded OLE file from a drawing object. The API response contains an embedded OLE file of the first drawing object of the document. However, returns an error if the drawing object does not have an embedded OLE file.

## REST API’s Resources

```JAVA
~/{file-name}/drawingObjects/{index}/oleData

~/{file-name}/{nodePath}/drawingObjects/{index}/oleData
```
, where:
- *{file-name}* is a filename of a document.
- *{nodePath}* is a path to a node in a document. If this parameter is used, elements contained within a specified node will be processed:
  - *sections/{sectionIndex}* - references a section.
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.
- *{index}* is an index of a drawing object.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DrawingObjects/GetDocumentDrawingObjectOleData) lets you call this REST API directly from a browser. 

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get OLE file from a drawing object
curl -v "https://api.aspose.cloud/v4.0/words/sample_EmbeddedOLE.docx/drawingObjects/0/oleData" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o Object.ole
```

To get a JWT-token, please, follow these [instructions](/words/getting-started/available-sdks/#curl).

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
OLE file
```

{{< /tab >}}
{{< /tabs >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetDocumentDrawingObjectOleData.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentDrawingObjectOleData.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_document_drawing_object_ole_data.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_document_drawing_object_ole_data.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getDocumentDrawingObjectOleData.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentDrawingObjectOleData.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentDrawingObjectOleData.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentDrawingObjectOleData.go" >}}
{{< /tab >}}
{{< /tabs >}}
