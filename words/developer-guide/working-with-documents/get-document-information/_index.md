---
title: "Get Document Information"
type: docs
url: /get-document-information/
weight: 30
---

# **Introduction**
This REST API allows you to get information about the document. The API returns a JSON/XML representation of the document unless a specific Accept header is provided in which case it will return the document in the specified format. The different representations of a document are basically the formats to which the document can be converted. So to achieve a conversion, all a user has to do is to use one of these links.
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/WordsDocument/GetDocument) lets you call this REST API directly from the browser.  
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

// cURL example to get document information

curl -v "https://api.aspose.cloud/v4.0/words/test\_multi\_pages.docx" \
-X GET \
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

        "Title": "Download as PC\* Connection #0 to host api.aspose.cloud left intact L"

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
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "GetDocumentInfo.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentInfo.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetDocumentInfo.php" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetDocumentInfo.py" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetDocumentInfo.rb" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetDocumentInfo.js" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_GetDocumentInfo.java" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_GetDocumentInfo.swift" >}}

{{< /tab >}}

{{< tab tabNum="9" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentInfo.go" >}}

{{< /tab >}}

{{< /tabs >}}
