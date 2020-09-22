---
title: "Get a Particular Drawing Object"
type: docs
url: /get-a-particular-drawing-object/
aliases: [/get-a-particular-drawing-object/]
weight: 20
---

This REST API allows you to get a particular drawing object from the document. You can also convert a drawing object to a specified format. Moreover, the detail of resource properties are given below:

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

## Resource URI

```html

~/{file-name}/drawingObjects/{index}
~/{file-name}/{nodePath}/drawingObjects/{index}
```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to a specific node in the document. If this URI is used, only elements contained within a specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

*{index}* is the index of the specific drawing object.

[Swagger UI](https://apireference.aspose.cloud/words/#/DrawingObjects/GetDocumentDrawingObjectByIndex) lets you call this REST API directly from the browser. 

## cURL Example

**Input Document:** [test_multi_pages.docx](attachments/885442/1180124.docx)

**Output File:** [drawingObject.png](attachments/885442/1180123.png)

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// First get Access Token
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/oauth2/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get a particular drawing object in a PNG format

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/drawingObjects/0?format=png" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o drawingObject.png
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
drawingObject.png file
```

{{< /tab >}}
{{< /tabs >}}
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetDocumentDrawingObjectByIndexWithFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentDrawingObjectByIndex.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_document_drawing_object_by_index.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_document_drawing_object_by_index.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getDocumentDrawingObjectByIndex.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentDrawingObjectByIndex.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentDrawingObjectByIndex.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentDrawingObjectByIndex.go" >}}
{{< /tab >}}
{{< /tabs >}}
