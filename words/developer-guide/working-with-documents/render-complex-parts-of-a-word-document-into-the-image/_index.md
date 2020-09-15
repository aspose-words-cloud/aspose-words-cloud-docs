---
title: "Render Complex Parts of a Word Document Into the Image"
type: docs
url: /render-complex-parts-of-a-word-document-into-the-image/
weight: 90
---

## **Introduction**
This REST API allows you to render complex portions of a document to any supported format. The following elements can be rendered: 

- page
- paragraph
- table
- drawingObject
- officeMathObject

The request parameters are the following:

|**Parameter Name**|**Type**|**Query String/HTTPBody**|**Description**|
| :- | :- | :- | :- |
|format|string|Query String: format=jpeg|Return the document in the specified format. Valid values for this parameter are given below.|
The following formats are supported:

|**format parameter value**|**Format of the returned Presentation**|
| :- | :- |
|bmp|Bitmap image file|
|gif|Gif Image|
|jpeg|JPEG Image|
|png|Portable Network Graphic|
|svg|Scalable Vector Graphics File|
|tiff|Tagged Image File Format|
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Render) lets you call following REST APIs directly from the browser:

- [Renders page to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderPage)
- [Renders paragraph to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderParagraph)
- [Renders table to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderTable)
- [Renders drawing object to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderDrawingObject)
- [Renders math object to a specified format](https://apireference.aspose.cloud/words/#/Render/RenderMathObject)
## **cURL Example**
**Case 1: Render a page of the document in BMP format:**

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \

-X POST \

-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"

// cURL example to render a page of the document in BMP format

curl -v "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/pages/1/render?format=bmp" \

-X GET \

-H "Content-Type: application/json" \

-H "Accept: application/json" \

-H "Authorization: Bearer <jwt token>" \

-o SampleWordDocument.bmp

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

BMP File

```

{{< /tab >}}

{{< /tabs >}}

**Case 2: Render a paragraph in PNG format:**

{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \

-X POST \

-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"

// cURL example to render a paragraph in PNG format

curl -v "https://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/paragraphs/0/render?format=png" \

-X GET \

-H "Content-Type: application/json" \

-H "Accept: application/json" \

-H "Authorization: Bearer <jwt token>" \

-o Paragraph.png

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

PNG File

```

{{< /tab >}}

{{< /tabs >}}

**Case 3: Render a table in PNG format:**

{{< tabs tabTotal="2" tabID="7" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \

-X POST \

-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"

// cURL example to render a table in PNG format

curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/0/render?format=png" \

-X GET \

-H "Content-Type: application/json" \

-H "Accept: application/json" \

-H "Authorization: Bearer <jwt token>" \

-o Table.png

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

PNG File

```

{{< /tab >}}

{{< /tabs >}}

**Case 4: Render a drawingObject in PDF format:**

{{< tabs tabTotal="2" tabID="10" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \

-X POST \

-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"

// cURL example to render a DrawingObject to PDF format

curl -v "https://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/drawingObjects/0/render?format=pdf" \

-X GET \

-H "Content-Type: application/json" \

-H "Accept: application/json" \

-H "Authorization: Bearer <jwt token>" \

-o DrawingObject.pdf

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

PDF File

```

{{< /tab >}}

{{< /tabs >}}

**Case 5: Render an OfficeMathObject in PNG format:**

{{< tabs tabTotal="2" tabID="13" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \

-X POST \

-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"

// cURL example to render a OfficeMathObject to PNG format

curl -v "https://api.aspose.cloud/v4.0/words/MathObjects.docx/OfficeMathObjects/0/render?format=png" \

-X GET \

-H "Content-Type: application/json" \

-H "Accept: application/json" \

-H "Authorization: Bearer <jwt token>" \

-o OfficeMathObject.png

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

PNG File

```

{{< /tab >}}

{{< /tabs >}}
## **SDK Examples**
**Case 1: Renders Page to Specified Format**

{{< tabs tabTotal="7" tabID="16" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "RendersPageToSpecifiedFormat.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "RenderPage.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "render\_page\_to\_specified\_format.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "render\_page.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "renderPage.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_RenderPage.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_RenderPage.swift" >}}

{{< /tab >}}

{{< /tabs >}}

**Case 2: Renders Paragraph to Specified Format**

{{< tabs tabTotal="7" tabID="17" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "RenderParagraph.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "RenderParagraph.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "render\_paragraph\_to\_specified\_format.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "render\_paragraph.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "renderParagraph.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_RenderParagraph.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_RenderParagraph.swift" >}}

{{< /tab >}}

{{< /tabs >}}

**Case 3: Renders Table to Specified Format**

{{< tabs tabTotal="7" tabID="18" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "RenderTable.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "RenderTable.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "render\_table\_to\_specified\_format.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "render\_table.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "renderTable.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_RenderTable.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_RenderTable.swift" >}}

{{< /tab >}}

{{< /tabs >}}

**Case 4: Renders Drawing Object to Specified Format**

{{< tabs tabTotal="7" tabID="19" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "RenderDrawingObjectToSpecifiedFormat.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "RenderDrawingObject.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "render\_drawing\_object\_to\_specified\_format.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "render\_drawing\_object.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "renderDrawingObject.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_RenderDrawingObject.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_RenderDrawingObject.swift" >}}

{{< /tab >}}

{{< /tabs >}}

**Case 5: Renders Math Object to Specified Format**

{{< tabs tabTotal="7" tabID="20" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "RenderMathObject.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "RenderMathObject.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "render\_math\_object\_to\_specified\_format.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "render\_math\_object.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "renderMathObject.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_RenderMathObject.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_RenderMathObject.swift" >}}

{{< /tab >}}

{{< /tabs >}}

