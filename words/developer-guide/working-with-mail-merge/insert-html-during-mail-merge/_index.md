---
title: "Insert HTML During Mail Merge"
type: docs
url: /insert-html-during-mail-merge/
aliases: [/insert-html-during-mail-merge/]
weight: 50
---

This example explains how to insert HTML on a MERGEFIELD. [executeMailMerge](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMerge) API lets you insert HTML on a merge field. The mail merges data string can be either in XML or JSON format.

{{% alert color="primary" %}} 

Please escape HTML characters in data source string and use "format"="html" attribute.

{{% /alert %}} 

## Resource URI

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMerge) lets you call the REST API directly from the browser. The description of the APIs and its parameters are also given there.

## cURL Example

cUrl is a popular command-line utility for transferring data and a perfect tool for testing REST APIs. The following are a few examples of using cURL.Input Document: [template.doc](attachments/885367/1180109.doc)

Mail Merge Data: [TestExecuteMailMergeData.txt](attachments/885367/1180108.txt)

Output Document: [TestPostDocumentExecuteMailMerge.docx](attachments/885367/1180102.docx)

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

// cURL example to populate MailMerge template with HTML Data
curl -v "https://api.aspose.cloud/v4.0/words/template.doc/MailMerge?destFileName=TestPostDocumentExecuteMailMerge.docx" \
-X PUT \
-F data=@TestExecuteMailMergeData.txt \
-H "Content-Type: multipart/form-data" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
{
  "Document": {
    "Links": [
      {
        "Href": "TestPostDocumentExecuteMailMerge.docx",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=doc>",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOC"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=dot>",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOT"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=docx>",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as DOCX"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=docm>",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.document.macroEnabled.12",
        "Title": "Download as DOCM"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=dotx>",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",
        "Title": "Download as DOTX"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=dotm>",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.template.macroEnabled.12",
        "Title": "Download as DOTM"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=flatopc>",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as FLATOPC"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=rtf>",
        "Rel": "alternate",
        "Type": "application/rtf",
        "Title": "Download as RTF"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=wml>",
        "Rel": "alternate",
        "Type": "text/xml",
        "Title": "Download as WML"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=odt>",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text",
        "Title": "Download as ODT"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=ott>",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text-template",
        "Title": "Download as OTT"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=txt>",
        "Rel": "alternate",
        "Type": "text/plain",
        "Title": "Download as TXT"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=mhtml>",
        "Rel": "alternate",
        "Type": "multipart/related",
        "Title": "Download as MHTML"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=epub>",
        "Rel": "alternate",
        "Type": "application/epub+zip",
        "Title": "Download as EPUB"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=pdf>",
        "Rel": "alternate",
        "Type": "application/pdf",
        "Title": "Download as PDF"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=xps>",
        "Rel": "alternate",
        "Type": "application/vnd.ms-xpsdocument",
        "Title": "Download as XPS"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=tiff>",
        "Rel": "alternate",
        "Type": "image/tiff",
        "Title": "Download as TIFF"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=png>",
        "Rel": "alternate",
        "Type": "image/png",
        "Title": "Download as PNG"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=jpeg>",
        "Rel": "alternate",
        "Type": "image/jpeg",
        "Title": "Download as JPEG"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=bmp>",
        "Rel": "alternate",
        "Type": "image/bmp",
        "Title": "Download as BMP"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=gif>",
        "Rel": "alternate",
        "Type": "image/gif",
        "Title": "Download as GIF"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=svg>",
        "Rel": "alternate",
        "Type": "image/svg+xml",
        "Title": "Download as SVG"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge*> Connection #0 to host api.aspose.cloud left intact .docx?format=html",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTML"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=htmlfixed>",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTMLFIXED"
      },
      {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=pcl>",
        "Rel": "alternate",
        "Type": "application/x-pcl",
        "Title": "Download as PCL"
      }
    ],
    "FileName": "TestPostDocumentExecuteMailMerge.docx",
    "SourceFormat": 1,
    "IsEncrypted": false,
    "IsSigned": false,
    "DocumentProperties": {
      "List": null,
      "link": {
        "Href": "<http://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx/documentProperties>",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    }
  },
  "Code": 200,
  "Status": "OK"
}
{{< /tab >}}
{{< /tabs >}}
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.

## SDK Examples

The code examples of using this REST API with various SDKs are presented below:

{{< tabs tabTotal="9" tabID="3" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "PopulateMailMergeTemplateWithHTMLData.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PopulateMailMergeTemplateWithHTMLData.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "PopulateMailMergeTemplateWithHTMLData.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "PopulateMailMergeTemplateWithHTMLData.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "PopulateMailMergeTemplateWithHTMLData.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "PopulateMailMergeTemplateWithHTMLData.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PopulateMailMergeTemplateWithHTMLData.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PopulateMailMergeTemplateWithHTMLData.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "PopulateMailMergeTemplateWithHTMLData.go" >}}
{{< /tab >}}
{{< /tabs >}}
PopulateMailMergeTemplateWithHTMLData
