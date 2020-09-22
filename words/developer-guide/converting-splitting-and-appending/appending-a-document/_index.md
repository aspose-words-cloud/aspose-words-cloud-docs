---
title: "Appending a Document"
type: docs
url: /appending-a-document/
aliases: [/appending-a-document/]
keywords: "document append, convert word doc to html, save word file as pdf, go sdk, Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift"
description: "Append Word documents in Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift using Aspose.Words Cloud. Recently we have introduced Go SDK for our Golang customers.Basically, appending documents is a very common task and is fully supported in Aspose.Words Cloud. The API allows you to append a document or documents, specified in the documentList parameter, to the original resource document. The changes are saved in the original resource document if the destFileName parameter is missing."
weight: 10
---

Appending documents is a very common task and is fully supported in Aspose.Words Cloud. The API allows you to append a document or documents, specified in the **documentList** parameter, to the original resource document. The changes are saved in the original resource document if the **destFileName** parameter is missing.

The description of the important API parameters is given below:

|Name|Type|Description|
| :- | :- | :- |
|Href|string|Path of the document to append.|
|ImportFormatMode|string|Defines which formatting will be used: appended or destination document. Possible values are **KeepSourceFormatting** or **UseDestinationStyles**. |

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Append/AppendDocument) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there.

## cURL Example

**Input Documents: [**test_doc.docx](attachments/885186/1180117.docx), [**test_multi_pages.docx](attachments/885186/1180118.docx)**

**Output Document: [**test_doc_output.docx](attachments/885186/1180114.docx)**

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to append a document

curl -v "https://api.aspose.cloud/v4.0/words/test_doc.docx/appendDocument" \
-X PUT \
-d "{'DocumentEntries':[{'Href':'test_multi_pages.docx', 'ImportFormatMode':'KeepSourceFormatting'}]}" \
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
        "Href": "test_doc.docx",
        "Rel": "self"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=doc",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOC"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=dot",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOT"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=docx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as DOCX"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=docm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.document.macroEnabled.12",
        "Title": "Download as DOCM"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=dotx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",
        "Title": "Download as DOTX"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=dotm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.template.macroEnabled.12",
        "Title": "Download as DOTM"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=flatopc",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as FLATOPC"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=rtf",
        "Rel": "alternate",
        "Type": "application/rtf",
        "Title": "Download as RTF"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=wml",
        "Rel": "alternate",
        "Type": "text/xml",
        "Title": "Download as WML"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=odt",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text",
        "Title": "Download as ODT"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=ott",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text-template",
        "Title": "Download as OTT"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=txt",
        "Rel": "alternate",
        "Type": "text/plain",
        "Title": "Download as TXT"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=mhtml",
        "Rel": "alternate",
        "Type": "multipart/related",
        "Title": "Download as MHTML"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=epub",
        "Rel": "alternate",
        "Type": "application/epub+zip",
        "Title": "Download as EPUB"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=pdf",
        "Rel": "alternate",
        "Type": "application/pdf",
        "Title": "Download as PDF"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=xps",
        "Rel": "alternate",
        "Type": "application/vnd.ms-xpsdocument",
        "Title": "Download as XPS"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=tiff",
        "Rel": "alternate",
        "Type": "image/tiff",
        "Title": "Download as TIFF"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=png",
        "Rel": "alternate",
        "Type": "image/png",
        "Title": "Download as PNG"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=jpeg",
        "Rel": "alternate",
        "Type": "image/jpeg",
        "Title": "Download as JPEG"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=bmp",
        "Rel": "alternate",
        "Type": "image/bmp",
        "Title": "Download as BMP"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=gif",
        "Rel": "alternate",
        "Type": "image/gif",
        "Title": "Download as GIF"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=svg",
        "Rel": "alternate",
        "Type": "image/svg+xml",
        "Title": "Download as SVG"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=html",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTML"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=htmlfixed",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTMLFIXED"

      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx?format=pcl",
        "Rel": "alternate",
        "Type": "application/x-pcl",
        "Title": "Download as PCL"

      }
    ],
    "FileName": "test_doc.docx",
    "SourceFormat": "Docx",
    "IsEncrypted": false,
    "IsSigned": false,
    "DocumentProperties": {
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/test_doc.docx/documentProperties",
        "Rel": "self"

      }
    }
  }
}
```

{{< /tab >}}
{{< /tabs >}}
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "AppendaDocument.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "AppendaDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "AppendaDocument.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "AppendaDocument.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "" "3f3f4f7033ae386af05042ee2ad3aa06" "AppendaDocument.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "AppendaDocument.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_AppendaDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_AppendaDocument.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "Aspose_Cloud_Words_AppendaDocument.go" >}}
{{< /tab >}}
{{< /tabs >}}
