---
title: "Get OLE file from a Drawing Object"
type: docs
url: /get-ole-file-from-a-drawing-object/
aliases: [/get-ole-file-from-a-drawing-object/]
weight: 70
---

This REST API allows you to get an embedded OLE file from a drawing object. The API response contains an embedded OLE file of the first drawing object of the document. However, returns an error if the drawing object does not have an embedded OLE file.

## Resource URI

```java

~/{file-name}/drawingObjects/{index}/oleData

~/{file-name}/{nodePath}/drawingObjects/{index}/oleData

```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to specific node in the document. If this URI is used, only elements contained within specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

*{index}* is the index of specific drawing object.

[Swagger UI](https://apireference.aspose.cloud/words/#/DrawingObjects/GetDocumentDrawingObjectOleData) lets you call this REST API directly from the browser. 

## cURL Example

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```java

// Please get your App_Key and App_SID from https://dashboard.aspose.cloud/#/apps. Place your App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get OLE file from a drawing object

curl -v "https://api.aspose.cloud/v4.0/words/sample_EmbeddedOLE.docx/drawingObjects/0/oleData" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o Object.ole

```

{{< /tab >}}
{{< tab tabNum="2" >}}

```java

OLE file

```

{{< /tab >}}
{{< /tabs >}}

## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.

## SDK Examples

Code examples for various SDKs are presented below:
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
