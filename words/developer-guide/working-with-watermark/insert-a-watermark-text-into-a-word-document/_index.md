---
title: "Insert a Watermark Text into a Word Document"
type: docs
url: /insert-a-watermark-text-into-a-word-document/
weight: 30
---

# **Introduction**
This REST API allows you to insert a watermark text into a document. This is a high-level operation that allows inserting a WordArt object into headers/footers in a document. The object will appear as a watermark throughout the document. The most important request parameters are the following:

|**Parameter Name**|**Type**|**Query String/HTTP Body**|**Description**|
| :- | :- | :- | :- |
|watermarkText |string|Query String/HTTP Body: text=DRAFT|Watermark text.|
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Watermarks/InsertWatermarkText) lets you call this REST API directly from the browser.  
## **cURL Example**
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

// cURL example to insert a WordArt text watermark into a document

curl -v "https://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/watermarks/texts" \
-X POST \
-d "{ 'Text': 'This is the text', 'RotationAngle': 90 }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Document": {

    "Links": [

      {

        "Href": "test\_multi\_pages.docx",

        "Rel": "self",

        "Type": null,

        "Title": null

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=doc",

        "Rel": "alternate",

        "Type": "application/msword",

        "Title": "Download as DOC"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=dot",

        "Rel": "alternate",

        "Type": "application/msword",

        "Title": "Download as DOT"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=docx",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",

        "Title": "Download as DOCX"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=docm",

        "Rel": "alternate",

        "Type": "application/vnd.ms-word.document.macroEnabled.12",

        "Title": "Download as DOCM"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=dotx",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",

        "Title": "Download as DOTX"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=dotm",

        "Rel": "alternate",

        "Type": "application/vnd.ms-word.template.macroEnabled.12",

        "Title": "Download as DOTM"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=flatopc",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",

        "Title": "Download as FLATOPC"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=rtf",

        "Rel": "alternate",

        "Type": "application/rtf",

        "Title": "Download as RTF"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=wml",

        "Rel": "alternate",

        "Type": "text/xml",

        "Title": "Download as WML"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=odt",

        "Rel": "alternate",

        "Type": "application/vnd.oasis.opendocument.text",

        "Title": "Download as ODT"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=ott",

        "Rel": "alternate",

        "Type": "application/vnd.oasis.opendocument.text-template",

        "Title": "Download as OTT"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=txt",

        "Rel": "alternate",

        "Type": "text/plain",

        "Title": "Download as TXT"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=mhtml",

        "Rel": "alternate",

        "Type": "multipart/related",

        "Title": "Download as MHTML"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=epub",

        "Rel": "alternate",

        "Type": "application/epub+zip",

        "Title": "Download as EPUB"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=pdf",

        "Rel": "alternate",

        "Type": "application/pdf",

        "Title": "Download as PDF"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=xps",

        "Rel": "alternate",

        "Type": "application/vnd.ms-xpsdocument",

        "Title": "Download as XPS"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=tiff",

        "Rel": "alternate",

        "Type": "image/tiff",

        "Title": "Download as TIFF"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=png",

        "Rel": "alternate",

        "Type": "image/png",

        "Title": "Download as PNG"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=jpeg",

        "Rel": "alternate",

        "Type": "image/jpeg",

        "Title": "Download as JPEG"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=bmp",

        "Rel": "alternate",

        "Type": "image/bmp",

        "Title": "Download as BMP"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=gif",

        "Rel": "alternate",

        "Type": "image/gif",

        "Title": "Download as GIF"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=svg",

        "Rel": "alternate",

        "Type": "image/svg+xml",

        "Title": "Download as SVG"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=html",

        "Rel": "alternate",

        "Type": "text/html",

        "Title": "Download as HTML"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=htmlfixed",

        "Rel": "alternate",

        "Type": "text/html",

        "Title": "Download as HTMLFIXED"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx?format=pcl",

        "Rel": "alternate",

        "Type": "application/x-pcl",

        "Title": "Download as PCL"

      }

    ],

    "FileName": "test\_multi\_pages.docx",

    "SourceFormat": 4,

    "IsEncrypted": false,

    "IsSigned": false,

    "DocumentProperties": {

      "List": null,

      "link": {

        "Href": "http://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx/documentProperties",

        "Rel": "self",

        "Type": null,

        "Title": null

      }

    }

  },

  "Code": 200,

  "Status": "OK"

}

```

{{< /tab >}}

{{< /tabs >}}
# **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "InsertWatermarkText.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostInsertDocumentWatermarkText.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "post\_insert\_document\_watermark\_text.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "insert\_document\_watermark\_text.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postInsertDocumentWatermarkText.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_PostInsertDocumentWatermarkText.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_PostInsertDocumentWatermarkText.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "InsertDocumentWatermarkText.go" >}}

{{< /tab >}}

{{< /tabs >}}
