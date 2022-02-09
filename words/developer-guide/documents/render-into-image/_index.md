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

Request parameters are the following:

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

## Usage examples with cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

**Case 1**: Render a page of the document in BMP format:

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "RenderMathObjectOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "RenderMathObjectOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
BMP File
```
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 2**: Render a paragraph in PNG format:

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="4" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
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
{{< tabs tabTotal="3" tabID="7" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
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
{{< tabs tabTotal="3" tabID="10" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
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
{{< tabs tabTotal="3" tabID="13" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
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

## Usage examples in Python, Java, C#, etc.

The following code samples show how to interact with the REST API using almost any mainstream programming language.

You can find a lot of other examples in [Python](https://gist.github.com/aspose-words-cloud-gists/e26813ced70692c544820cd8011ee7e0), [Java](https://gist.github.com/aspose-words-cloud-gists/caede439bfd2e57c3010befe504faff4), [C#](https://gist.github.com/aspose-words-cloud-gists/374e1e3dd4bca8f696f29d913645f549), [JavaScript](https://gist.github.com/aspose-words-cloud-gists/a9510e4b51613f1138e7c1ec09634c4a), [PHP](https://gist.github.com/aspose-words-cloud-gists/e2a72445b96362dc0117f06ab54bb94a), [C++](https://gist.github.com/aspose-words-cloud-gists/49aa5151a094849179bae8672c887a0e), [Golang](https://gist.github.com/aspose-words-cloud-gists/625ca80adffd779e8f6e3611551e14d5), [Ruby](https://gist.github.com/aspose-words-cloud-gists/339f3835a4c0a536c81ec941de29baf7), [Swift](https://gist.github.com/aspose-words-cloud-gists/790dbd2edd5d36f170732366f52cac4c), [Dart](https://gist.github.com/aspose-words-cloud-gists/6aae628cf2b878b78fea177c3171c6bf) on GitHub. All codes are thoroughly tested and ready for production use.

**Case 1**: Renders Page to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="16" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "RenderPageOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderPageOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "RenderPageOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderPageOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "RenderPageOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "RenderPageOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "RenderPageOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "RenderPageOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderPageOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "RenderPageOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 2**: Renders Paragraph to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="17" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "RenderParagraphOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderParagraphOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "RenderParagraphOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderParagraphOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "RenderParagraphOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "RenderParagraphOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "RenderParagraphOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "RenderParagraphOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderParagraphOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "RenderParagraphOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 3**: Renders Table to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="18" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "RenderTableOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderTableOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "RenderTableOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderTableOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "RenderTableOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "RenderTableOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "RenderTableOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "RenderTableOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderTableOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "RenderTableOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 4**: Renders Drawing Object to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="19" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "RenderDrawingObjectOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderDrawingObjectOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "RenderDrawingObjectOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderDrawingObjectOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "RenderDrawingObjectOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "RenderDrawingObjectOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "RenderDrawingObjectOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "RenderDrawingObjectOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderDrawingObjectOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "RenderDrawingObjectOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 5**: Renders Math Object to Specified Format

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="20" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "RenderMathObjectOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "RenderMathObjectOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "RenderMathObjectOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "RenderMathObjectOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "RenderMathObjectOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "RenderMathObjectOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "RenderMathObjectOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "RenderMathObjectOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "RenderMathObjectOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "RenderMathObjectOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

