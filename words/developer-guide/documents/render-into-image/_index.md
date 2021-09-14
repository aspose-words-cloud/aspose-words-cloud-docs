---
title: "Render Complex Parts of a Word Document Into the Image"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /documents/render-into-image/
aliases: [/render-complex-parts-of-a-word-document-into-the-image/]
description: "Render complex parts of a Word document into an image."
weight: 70
---

This REST API renders complex parts of a document to a specified image format.

The following elements can be rendered:

- page
- paragraph
- table
- drawingObject
- officeMathObject

The request parameters are the following:

|Parameter Name|Type|Query String/HTTPBody|Description|
| :- | :- | :- | :- |
|format|string|Query String: format=jpeg|Return the document in the specified format. Valid values for this parameter are given below.|

The following formats are supported:

|format parameter value|Format of the returned Presentation|
| :- | :- |
|bmp|Bitmap image file|
|gif|Gif Image|
|jpeg|JPEG Image|
|png|Portable Network Graphic|
|svg|Scalable Vector Graphics File|
|tiff|Tagged Image File Format|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Render) lets you call the following REST APIs directly from a browser:

- [Renders page to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderPage).
- [Renders paragraph to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderParagraph).
- [Renders table to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderTable).
- [Renders drawing object to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderDrawingObject).
- [Renders math object to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderMathObject).

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

**Case 1**: Render a page of the document in BMP format:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to render a page of the document in BMP format
curl -v "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/pages/1/render?format=bmp" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o SampleWordDocument.bmp
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
BMP File
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 2**: Render a paragraph in PNG format:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your `Client Id` and `Secret` credentials from https://dashboard.aspose.cloud/applications.
# Place `Client Id` in client_id argument. Place `Secret` in client_secret argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to render a paragraph in PNG format
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/paragraphs/0/render?format=png" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o Paragraph.png
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
PNG File
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 3**: Render a table in PNG format:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="7" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your `Client Id` and `Secret` credentials from https://dashboard.aspose.cloud/applications.
# Place `Client Id` in client_id argument. Place `Secret` in client_secret argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to render a table in PNG format
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/0/render?format=png" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o Table.png
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
PNG File
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 4**: Render a drawingObject in PDF format:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="10" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your `Client Id` and `Secret` credentials from https://dashboard.aspose.cloud/applications.
# Place `Client Id` in client_id argument. Place `Secret` in client_secret argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to render a DrawingObject to PDF format
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/drawingObjects/0/render?format=pdf" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o DrawingObject.pdf
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
PDF File
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 5**: Render an OfficeMathObject in PNG format:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="13" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your `Client Id` and `Secret` credentials from https://dashboard.aspose.cloud/applications.
# Place `Client Id` in client_id argument. Place `Secret` in client_secret argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to render a OfficeMathObject to PNG format
curl -v "https://api.aspose.cloud/v4.0/words/MathObjects.docx/OfficeMathObjects/0/render?format=png" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o OfficeMathObject.png
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
PNG File
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

**Case 1**: Renders Page to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="4" tabID="16" tabName1="Java" tabName2="C#" tabName3="Android" tabName4="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderPage.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderPage.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "RenderPage.java" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderPage.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 2**: Renders Paragraph to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="4" tabID="17" tabName1="Java" tabName2="C#" tabName3="Android" tabName4="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderParagraph.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderParagraph.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "RenderParagraph.java" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderParagraph.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 3**: Renders Table to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="4" tabID="18" tabName1="Java" tabName2="C#" tabName3="Android" tabName4="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderTable.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderTable.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "RenderTable.java" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderTable.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 4**: Renders Drawing Object to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="4" tabID="19" tabName1="Java" tabName2="C#" tabName3="Android" tabName4="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderDrawingObject.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderDrawingObjectToSpecifiedFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "RenderDrawingObject.java" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderDrawingObject.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 5**: Renders Math Object to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="4" tabID="20" tabName1="Java" tabName2="C#" tabName3="Android" tabName4="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderMathObject.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderMathObject.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "RenderMathObject.java" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderMathObject.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
