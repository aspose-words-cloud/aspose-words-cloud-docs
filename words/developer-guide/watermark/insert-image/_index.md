---
title: "Insert a Watermark Image into a Word Document"
type: docs
url: /watermark/insert-image/
aliases: [/insert-a-watermark-image-into-a-word-document/]
weight: 20
---

This REST API allows you to insert a watermark image into a document. This is a high-level operation that allows inserting an image into headers/footers in a document. The image will appear as a watermark throughout the document. The most important request parameters are the following:

|Parameter Name|Type|Query String/HTTP Body|Description|
| :- | :- | :- | :- |
|image|string|Query string: imageFile=ImagesFolder/watermark.jpg|The image file server full name. If the name is empty the image is expected in request content.|
|rotationAngle|double|Query string: rotationAngle = -42.5|The watermark rotation angle.|

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Watermarks/InsertWatermarkImage) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to insert a watermark image into a document.
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/watermarks/images?destFileName=InsertDocumentWatermarkImage.docx&rotationAngle=0F&image=aspose-cloud.png" \
-X POST \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Content-Length: 0" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
{
  "Document": {
    "Links": [
      {
        "Href": "InsertDocumentWatermarkImage.docx",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=doc",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOC"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=dot",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOT"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=docx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as DOCX"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=docm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.document.macroEnabled.12",
        "Title": "Download as DOCM"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=dotx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",
        "Title": "Download as DOTX"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=dotm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.template.macroEnabled.12",
        "Title": "Download as DOTM"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=flatopc",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as FLATOPC"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=rtf",
        "Rel": "alternate",
        "Type": "application/rtf",
        "Title": "Download as RTF"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=wml",
        "Rel": "alternate",
        "Type": "text/xml",
        "Title": "Download as WML"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=odt",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text",
        "Title": "Download as ODT"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=ott",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text-template",
        "Title": "Download as OTT"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=txt",
        "Rel": "alternate",
        "Type": "text/plain",
        "Title": "Download as TXT"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=mhtml",
        "Rel": "alternate",
        "Type": "multipart/related",
        "Title": "Download as MHTML"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=epub",
        "Rel": "alternate",
        "Type": "application/epub+zip",
        "Title": "Download as EPUB"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=pdf",
        "Rel": "alternate",
        "Type": "application/pdf",
        "Title": "Download as PDF"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=xps",
        "Rel": "alternate",
        "Type": "application/vnd.ms-xpsdocument",
        "Title": "Download as XPS"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=tiff",
        "Rel": "alternate",
        "Type": "image/tiff",
        "Title": "Download as TIFF"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=png",
        "Rel": "alternate",
        "Type": "image/png",
        "Title": "Download as PNG"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=jpeg",
        "Rel": "alternate",
        "Type": "image/jpeg",
        "Title": "Download as JPEG"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=bmp",
        "Rel": "alternate",
        "Type": "image/bmp",
        "Title": "Download as BMP"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=gif",
        "Rel": "alternate",
        "Type": "image/gif",
        "Title": "Download as GIF"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=svg",
        "Rel": "alternate",
        "Type": "image/svg+xml",
        "Title": "Download as SVG"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=html",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTML"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=htmlfixed",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTMLFIXED"
      },
      {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx?format=pcl",
        "Rel": "alternate",
        "Type": "application/x-pcl",
        "Title": "Download as PCL"
      }
    ],
    "FileName": "InsertDocumentWatermarkImage.docx",
    "SourceFormat": 4,
    "IsEncrypted": false,
    "IsSigned": false,
    "DocumentProperties": {
      "List": null,
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/InsertDocumentWatermarkImage.docx/documentProperties",
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

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "InsertWatermarkImage.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostInsertDocumentWatermarkImage.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "post_insert_document_watermark_image.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "insert_document_watermark_image.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postInsertDocumentWatermarkImage.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostInsertDocumentWatermarkImage.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostInsertDocumentWatermarkImage.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "InsertDocumentWatermarkImage.go" >}}
{{< /tab >}}
{{< /tabs >}}