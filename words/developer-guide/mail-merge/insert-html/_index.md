---
title: "Insert HTML"
second_title: "Mail Merge"
type: docs
url: /mail-merge/insert-html/
aliases: [/insert-html-during-mail-merge/]
description: "Insert HTML into a MERGEFIELD in a Word document"
weight: 10
---

This example explains how to insert [HTML](https://docs.fileformat.com/web/html/) on a MERGEFIELD. [executeMailMerge](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMerge) API lets you insert [HTML](https://docs.fileformat.com/web/html/) on a merge field. The mail merges data string can be either in XML or JSON format.

Please escape HTML characters in data source string and use "format"="html" attribute.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMerge) lets you call the REST API directly from the browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [template.doc](template.doc) and [TestExecuteMailMergeData.txt](TestExecuteMailMergeData.txt) files designed to act as a demonstration and let you figure out the details quickly. The output document would be as follows: [TestPostDocumentExecuteMailMerge.docx](TestPostDocumentExecuteMailMerge.docx).

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to populate MailMerge template with HTML Data
curl -v "https://api.aspose.cloud/v4.0/words/template.doc/MailMerge?destFileName=TestPostDocumentExecuteMailMerge.docx" \
-X PUT \
-F data=@TestExecuteMailMergeData.txt \
-H "Content-Type: multipart/form-data" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs. Please check [Available SDKs](/words/getting-started/available-sdks/) article to learn how to add an SDK to your project.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="3" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "PopulateMailMergeTemplateWithHTMLData.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "PopulateMailMergeTemplateWithHTMLData.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "PopulateMailMergeTemplateWithHTMLData.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "PopulateMailMergeTemplateWithHTMLData.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "PopulateMailMergeTemplateWithHTMLData.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "PopulateMailMergeTemplateWithHTMLData.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "PopulateMailMergeTemplateWithHTMLData.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_PopulateMailMergeTemplateWithHTMLData.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_PopulateMailMergeTemplateWithHTMLData.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

PopulateMailMergeTemplateWithHTMLData
