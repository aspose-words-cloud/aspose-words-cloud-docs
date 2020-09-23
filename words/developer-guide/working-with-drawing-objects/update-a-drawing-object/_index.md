---
title: "Update a Drawing Object"
type: docs
url: /update-a-drawing-object/
aliases: [/update-a-drawing-object/]
weight: 40
---

This REST API allows you to update a drawing object in the Word document. The API returns updated object data in the XML/JSON format.

The request is an HTTP request with multipart content (see [RFC 2046](http://tools.ietf.org/html/rfc2046#page-17) or [RFC 1341](http://www.w3.org/Protocols/rfc1341/7_2_Multipart.html)). The first part of the multipart content contains the drawing object data and the second contains a binary image. Moreover, the detail of resource properties are given below:

|Parameter Name|Type|Description|
| :- | :- | :- |
|RelativeHorizontalPosition|Aspose.Words.Drawing.ShapeBase.RelativeHorizontalPosition|Specifies where the distance to the image is measured.|
|RelativeVerticalPosition|Aspose.Words.Drawing.ShapeBase.RelativeVerticalPosition|Specifies where the distance to the image is measured.|
|Left|double|Distance in points from the origin to the left side of the image.|
|Top|double|Distance in points from the origin to the top side of the image.|
|Width|double|Width of the drawing objects in points.|
|Height|double|Height of the drawing object in points.|
|WrapType|Aspose.Words.Drawing.ShapeBase.WrapType|Specifies how to wrap text around the image.|

## REST API’s Resources

The following URIs are used to address REST resources:

```HTML
~/{file-name}/drawingObjects/{index}
~/{file-name}/{nodePath}/drawingObjects/{index}
```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to a specific node in the document. If this URI is used, only elements contained within a specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

*{index}* is the index of the specific drawing object.
The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DrawingObjects/UpdateDrawingObject) lets you call this REST API directly from a browser. 

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

# cURL example to update a Drawing Object in the Word Document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/drawingObjects/0" \
-X PUT \
-F "json={ 'Left': 0 };type=application/json" \
-F "aspose-cloud.png=@aspose-cloud.png;type=image/png" \
-H "Content-Type: multipart/form-data" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
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

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "UpdateDrawingObject.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostDrawingObject.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "post_drawing_object.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "post_drawing_object.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postDrawingObject.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostDrawingObject.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostDrawingObject.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "PostDrawingObject.go" >}}
{{< /tab >}}
{{< /tabs >}}
