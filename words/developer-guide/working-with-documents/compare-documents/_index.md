---
title: "Compare Documents"
type: docs
url: /compare-documents/
aliases: [/compare-documents/]
weight: 80
---

{{% alert color="primary" %}} 

Try Online

You can try this functionality and view the results online at this link:

<https://products.aspose.app/words/comparison> {{% /alert %}} 
## Introduction
The REST API compares the input document with another document producing changes as a number of edit and format revisions. The changes are saved in the original resource document.

The description of the important parameters of the API is given below:

|Name|Type|Description|
| :- | :- | :- |
|ComparingWithDocument|string|Path to document to compare at the server.|
|Author|string|Initials of the author to use for revisions.|
|DateTime|string|The date and time to use for revisions. Default is the current server time.|
## Resource URI
[Swagger UI](https://apireference.aspose.cloud/words/#/Compare/CompareDocument) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there.
## cURL Example
**Input Documents: [**compareTestDoc1.doc](attachments/885441/1180122.doc)**, [compareTestDoc2.doc](attachments/885441/1180121.doc)

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to compare documents

curl -v "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc/compareDocument" \
-X PUT \
-d "{ 'Author': 'author', 'ComparingWithDocument': 'compareTestDoc2.doc' }" \
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

        "Href": "compareTestDoc1.doc",

        "Rel": "self"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=doc",

        "Rel": "alternate",

        "Type": "application/msword",

        "Title": "Download as DOC"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=dot",

        "Rel": "alternate",

        "Type": "application/msword",

        "Title": "Download as DOT"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=docx",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",

        "Title": "Download as DOCX"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=docm",

        "Rel": "alternate",

        "Type": "application/vnd.ms-word.document.macroEnabled.12",

        "Title": "Download as DOCM"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=dotx",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",

        "Title": "Download as DOTX"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=dotm",

        "Rel": "alternate",

        "Type": "application/vnd.ms-word.template.macroEnabled.12",

        "Title": "Download as DOTM"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=flatopc",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",

        "Title": "Download as FLATOPC"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=rtf",

        "Rel": "alternate",

        "Type": "application/rtf",

        "Title": "Download as RTF"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=wml",

        "Rel": "alternate",

        "Type": "text/xml",

        "Title": "Download as WML"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=odt",

        "Rel": "alternate",

        "Type": "application/vnd.oasis.opendocument.text",

        "Title": "Download as ODT"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=ott",

        "Rel": "alternate",

        "Type": "application/vnd.oasis.opendocument.text-template",

        "Title": "Download as OTT"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=txt",

        "Rel": "alternate",

        "Type": "text/plain",

        "Title": "Download as TXT"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=mhtml",

        "Rel": "alternate",

        "Type": "multipart/related",

        "Title": "Download as MHTML"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=epub",

        "Rel": "alternate",

        "Type": "application/epub+zip",

        "Title": "Download as EPUB"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=pdf",

        "Rel": "alternate",

        "Type": "application/pdf",

        "Title": "Download as PDF"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=xps",

        "Rel": "alternate",

        "Type": "application/vnd.ms-xpsdocument",

        "Title": "Download as XPS"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=tiff",

        "Rel": "alternate",

        "Type": "image/tiff",

        "Title": "Download as TIFF"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=png",

        "Rel": "alternate",

        "Type": "image/png",

        "Title": "Download as PNG"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=jpeg",

        "Rel": "alternate",

        "Type": "image/jpeg",

        "Title": "Download as JPEG"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=bmp",

        "Rel": "alternate",

        "Type": "image/bmp",

        "Title": "Download as BMP"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=gif",

        "Rel": "alternate",

        "Type": "image/gif",

        "Title": "Download as GIF"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=svg",

        "Rel": "alternate",

        "Type": "image/svg+xml",

        "Title": "Download as SVG"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=html",

        "Rel": "alternate",

        "Type": "text/html",

        "Title": "Download as HTML"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=htmlfixed",

        "Rel": "alternate",

        "Type": "text/html",

        "Title": "Download as HTMLFIXED"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc?format=pcl",

        "Rel": "alternate",

        "Type": "application/x-pcl",

        "Title": "Download as PCL"

      }

    ],

    "FileName": "compareTestDoc1.doc",

    "SourceFormat": "Doc",

    "IsEncrypted": false,

    "IsSigned": false,

    "DocumentProperties": {

      "link": {

        "Href": "https://api.aspose.cloud/v4.0/words/compareTestDoc1.doc/documentProperties",

        "Rel": "self"

      }

    }

  }

```

{{< /tab >}}

{{< /tabs >}}
## SDKs
Using an SDK is the best way to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## SDK Examples
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "CompareDocument.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "CompareDocument.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "compare_document.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "compare_document.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "compareDocument.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_CompareDocument.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_CompareDocument.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "CompareDocument.go" >}}

{{< /tab >}}

{{< /tabs >}}
