---
title: "Save a Webpage in a Word Document"
type: docs
url: /save-a-webpage-in-a-word-document/
aliases: [/save-a-webpage-in-a-word-document/]
weight: 20
---

This REST API allows you to load a new document from the web into the file with any supported format of data. The request parameters are given below:

|Parameter Name|Type|Description|
| :- | :- | :- |
|LoadingDocumentUrl|string|Web document URL|
|SaveOptions|SaveOptions|Save options|
Please check [Convert Document to Destination Format with Detailed Settings and Save Result to Storage](/convert-document-to-destination-format-with-detailed-settings-and-save-result-to-storage/) article to know the SaveOptions of different formats.

## Resource URI

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/WordsDocument/LoadWebDocument) lets you call this REST API directly from a browser.  

## cURL Example

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

// cURL example to load web page and save it to doc format
curl -v "https://api.aspose.cloud/v4.0/words/loadWebDocument" \
-X PUT \
-d "{ 'LoadingDocumentUrl': 'https://www.le.ac.uk/oerresources/bdra/html/page_09.htm', 'SaveOptions': { 'SaveFormat': 'docx', 'FileName': 'HTMLDocument.docx', 'SaveRoutingSlip': true } }" \
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

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "PostLoadWebDocument.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostLoadWebDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "PostLoadWebDocument.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "PostLoadWebDocument.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "PostLoadWebDocument.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "PostLoadWebDocument.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostLoadWebDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostLoadWebDocument.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "LoadWebDocument.go" >}}
{{< /tab >}}
{{< /tabs >}}
