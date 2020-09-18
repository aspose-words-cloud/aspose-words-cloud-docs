---
title: "Update Fields in a Document"
type: docs
url: /update-fields-in-a-document/
aliases: [/update-fields-in-a-document/]
weight: 20
---

This REST API allows you to update (reevaluate) fields in a document. 
## Resource URI
```html

~/{file-name}/updateFields

or

~/{file-name}/updateFields?filename={DestDocumentName}

```

[Swagger UI](https://apireference.aspose.cloud/words/#/Fields/UpdateFields) lets you call this REST API directly from the browser.  
## cURL Example
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to update Fields in a Document

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/updateFields" \
-X PUT \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Content-Length: 0" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Document": {

    "Links": [

      {

        "Href": "test_multi_pages.docx",

        "Rel": "self",

        "Type": null,

        "Title": null

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=doc",

        "Rel": "alternate",

        "Type": "application/msword",

        "Title": "Download as DOC"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=dot",

        "Rel": "alternate",

        "Type": "application/msword",

        "Title": "Download as DOT"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=docx",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",

        "Title": "Download as DOCX"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=docm",

        "Rel": "alternate",

        "Type": "application/vnd.ms-word.document.macroEnabled.12",

        "Title": "Download as DOCM"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=dotx",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",

        "Title": "Download as DOTX"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=dotm",

        "Rel": "alternate",

        "Type": "application/vnd.ms-word.template.macroEnabled.12",

        "Title": "Download as DOTM"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=flatopc",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",

        "Title": "Download as FLATOPC"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=rtf",

        "Rel": "alternate",

        "Type": "application/rtf",

        "Title": "Download as RTF"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=wml",

        "Rel": "alternate",

        "Type": "text/xml",

        "Title": "Download as WML"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=odt",

        "Rel": "alternate",

        "Type": "application/vnd.oasis.opendocument.text",

        "Title": "Download as ODT"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=ott",

        "Rel": "alternate",

        "Type": "application/vnd.oasis.opendocument.text-template",

        "Title": "Download as OTT"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=txt",

        "Rel": "alternate",

        "Type": "text/plain",

        "Title": "Download as TXT"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=mhtml",

        "Rel": "alternate",

        "Type": "multipart/related",

        "Title": "Download as MHTML"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=epub",

        "Rel": "alternate",

        "Type": "application/epub+zip",

        "Title": "Download as EPUB"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=pdf",

        "Rel": "alternate",

        "Type": "application/pdf",

        "Title": "Download as PDF"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=xps",

        "Rel": "alternate",

        "Type": "application/vnd.ms-xpsdocument",

        "Title": "Download as XPS"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=tiff",

        "Rel": "alternate",

        "Type": "image/tiff",

        "Title": "Download as TIFF"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=png",

        "Rel": "alternate",

        "Type": "image/png",

        "Title": "Download as PNG"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=jpeg",

        "Rel": "alternate",

        "Type": "image/jpeg",

        "Title": "Download as JPEG"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=bmp",

        "Rel": "alternate",

        "Type": "image/bmp",

        "Title": "Download as BMP"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=gif",

        "Rel": "alternate",

        "Type": "image/gif",

        "Title": "Download as GIF"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=svg",

        "Rel": "alternate",

        "Type": "image/svg+xml",

        "Title": "Download as SVG"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=html",

        "Rel": "alternate",

        "Type": "text/html",

        "Title": "Download as HTML"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=htmlfixed",

        "Rel": "alternate",

        "Type": "text/html",

        "Title": "Download as HTMLFIXED"

      },

      {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=pcl",

        "Rel": "alternate",

        "Type": "application/x-pcl",

        "Title": "Download as PC\* Connection #0 to host api.aspose.cloud left intact L"

      }

    ],

    "FileName": "test_multi_pages.docx",

    "SourceFormat": 4,

    "IsEncrypted": false,

    "IsSigned": false,

    "DocumentProperties": {

      "List": null,

      "link": {

        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties",

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
## SDKs
Using an SDK is the best way to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## SDK Examples
{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "UpdateDocumentFields.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostUpdateDocumentFields.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "post_update_document_fields.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "update_document_fields.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postUpdateDocumentFields.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostUpdateDocumentFields.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostUpdateDocumentFields.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "UpdateDocumentFields.go" >}}

{{< /tab >}}

{{< /tabs >}}
