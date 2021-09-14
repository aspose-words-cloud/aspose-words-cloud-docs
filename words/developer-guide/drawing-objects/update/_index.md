---
title: "Update"
second_title: "Drawing Objects in a Word Document"
type: docs
url: /drawing-objects/update/
aliases: [/update-a-drawing-object/]
description: "Update a drawing object in a Word document"
weight: 70
---

This REST API updates a `DrawingObject`.

The request is an HTTP request with multipart content (see [RFC 2046](http://tools.ietf.org/html/rfc2046#page-17) or [RFC 1341](http://www.w3.org/Protocols/rfc1341/7_2_Multipart.html)). The first part of the multipart content contains the drawing object data and the second contains a binary image.

The important parameters are described in the following table:

|Parameter Name|Type|Description|
| :- | :- | :- |
|RelativeHorizontalPosition|Aspose.Words.Drawing.ShapeBase.RelativeHorizontalPosition|Specifies where the distance to the image is measured.|
|RelativeVerticalPosition|Aspose.Words.Drawing.ShapeBase.RelativeVerticalPosition|Specifies where the distance to the image is measured.|
|Left|double|Distance in points from the origin to the left side of the image.|
|Top|double|Distance in points from the origin to the top side of the image.|
|Width|double|Width of the drawing objects in points.|
|Height|double|Height of the drawing object in points.|
|WrapType|Aspose.Words.Drawing.ShapeBase.WrapType|Specifies how to wrap text around the image.|

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

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DrawingObjects/UpdateDrawingObject) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser. 

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to update a Drawing Object in the Word Document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/drawingObjects/0" \
-X PUT \
-F "json={ 'Left': 0 };type=application/json" \
-F "aspose-cloud.png=@aspose-cloud.png;type=image/png" \
-H "Content-Type: multipart/form-data" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "DrawingObject": {
    "RenderLinks": [
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0?format=jpeg",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0?format=tiff",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0?format=png",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0?format=bmp",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    ],
    "Width": 100.0,
    "Height": 100.0,
    "OleDataLink": null,
    "ImageDataLink": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0/ImageData",
      "Rel": "self",
      "Type": null,
      "Title": null
    },
    "RelativeHorizontalPosition": "Margin",
    "Left": 0.0,
    "RelativeVerticalPosition": "TableDefault",
    "Top": 0.0,
    "WrapType": "Inline",
    "NodeId": "0.7.1",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0",
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
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "UpdateDrawingObject.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateDrawingObject.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateDrawingObject.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "UpdateDrawingObject.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "UpdateDrawingObject.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
