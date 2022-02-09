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

## cURL and Postman

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

You can carry out REST API interactions using **cURL** and **Postman**. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="2" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "UpdateDrawingObjectOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "UpdateDrawingObjectOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "DrawingObject": {
    "RenderLinks": [
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0?format=jpeg",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0?format=tiff",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0?format=png",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0?format=bmp",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    ],
    "Width": 100.0,
    "Height": 100.0,
    "OleDataLink": null,
    "ImageDataLink": {
      "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0/ImageData",
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
      "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7/drawingObjects/0",
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
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "UpdateDrawingObjectOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "UpdateDrawingObjectOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "UpdateDrawingObjectOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateDrawingObjectOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "UpdateDrawingObjectOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "UpdateDrawingObjectOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateDrawingObjectOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "UpdateDrawingObjectOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "UpdateDrawingObjectOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "UpdateDrawingObjectOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
