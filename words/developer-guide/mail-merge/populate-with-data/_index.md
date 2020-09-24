---
title: "Populate Template with Data"
second_title: "Mail Merge"
type: docs
url: /mail-merge/populate-with-data/
aliases: [/populate-mailmerge-template-with-data/]
keywords: "Populate, Mail Merge, Word, Microsoft Word, Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "In this article you will learn that how to populate mail merge in various languages. You can download the SDK of your favorite language and start programming in a smartest way. The Cloud SDKs are available in Python, C#, Java, C++, Ruby, PHP, Node.js, Swift and Go programming languages."
weight: 30
---

In this article you will learn that how to populate mail merge or mustache template with data in various languages. You can download an SDK of your favorite language and start programming in a smartest way. The Cloud SDKs are available in Python, C#, Java, C++, Ruby, PHP, Node.js, Swift and Go programming languages.

[This API](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMerge) represents a controller for executing the mail merge.

The following is a description of the most important parameters:

|Parameter Name|Description|
| :- | :- |
|withRegions|<p>Merge with regions or not. False by default.</p><p>Flag 'withRegions' can be omitted, in this case, a simple mail merge will be executed. If the flag is present and value is 'true' - mail merge with regions will be executed.</p>|
|mailMergeDataFile|If mailMergeDataFile parameter exists, the data is taken from the server path (the parameter must contain the full path to the server file). However, if the mailMergeDataFile parameter is omitted, the data is expected in the requested content.|
|cleanup|<p>If the cleanup parameter is omitted, cleanup options will be None.</p><p> </p>|
|useWholeParagraphAsRegion|Specifies a value indicating whether paragraphs with TableStart or TableEnd field should be fully included in the mail merge region or particular range between TableStart and TableEnd fields. The default value is true.|
| | |

The cleanup options parameter can contain a list of values from below, separated by ",":

|Value|Description|
| :- | :- |
|None|Without any cleanup.|
|EmptyParagraphs|Specifies whether paragraphs that contained mail merge fields with no data should be removed from the document.|
|UnusedRegions|Specifies whether unused mail merge regions should be removed from the document.|
|UnusedFields|Specifies whether unused merge fields should be removed from the document.|
|ContainingFields|Specifies whether fields that contain merge fields (for example, IFs) should be removed from the document if the nested merge fields are removed.|
|RemoveTitleRow|Removes title row of the table if this table doesn't contain any rows except title row. It does not remove title rows in nested tables.|
|RemoveTitleRowInInnerTables|Enable "RemoveTitleRow " for nested tables.|
|RemoveStaticFields|Specifies whether static fields should be removed from the document. Static fields are fields, which results remain the same upon any document change. Fields, which do not store their results in a document and are calculated on the fly (like Aspose.Words.Fields.FieldType.FieldListNum, Aspose.Words.Fields.FieldType.FieldSymbol, etc.) are not considered to be static.|

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMerge) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL.

**Case 1**: MailMerge Template

You can use a sample **Input Document** [SampleMailMergeTemplate.docx](/words/attachments/884946/1180099.docx) and a sample **Mail Merge Data** [SampleMailMergeTemplateData.txt](/words/attachments/884946/1180097.txt). The **Output Document** would be as follows: [TestPostDocumentExecuteMailMerge.docx](/words/attachments/884946/8028164.docx).

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to populate MailMerge template with Data
curl -v "https://api.aspose.cloud/v4.0/words/SampleMailMergeTemplate.docx/MailMerge?withRegions=false&destFileName=TestPostDocumentExecuteMailMerge.docx" \
-X PUT \
-F data=@SampleMailMergeTemplateData.txt \
-H "Content-Type: multipart/form-data" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Document": {
    "Links": [
      {
        "Href": "TestPostDocumentExecuteMailMerge.docx",
        "Rel": "self"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=doc",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=dot",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=docx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as DOCX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=docm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.document.macroEnabled.12",
        "Title": "Download as DOCM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=dotx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",
        "Title": "Download as DOTX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=dotm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.template.macroEnabled.12",
        "Title": "Download as DOTM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=flatopc",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as FLATOPC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=rtf",
        "Rel": "alternate",
        "Type": "application/rtf",
        "Title": "Download as RTF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=wml",
        "Rel": "alternate",
        "Type": "text/xml",
        "Title": "Download as WML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=odt",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text",
        "Title": "Download as ODT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=ott",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text-template",
        "Title": "Download as OTT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=txt",
        "Rel": "alternate",
        "Type": "text/plain",
        "Title": "Download as TXT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=mhtml",
        "Rel": "alternate",
        "Type": "multipart/related",
        "Title": "Download as MHTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=epub",
        "Rel": "alternate",
        "Type": "application/epub+zip",
        "Title": "Download as EPUB"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=pdf",
        "Rel": "alternate",
        "Type": "application/pdf",
        "Title": "Download as PDF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=xps",
        "Rel": "alternate",
        "Type": "application/vnd.ms-xpsdocument",
        "Title": "Download as XPS"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=tiff",
        "Rel": "alternate",
        "Type": "image/tiff",
        "Title": "Download as TIFF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=png",
        "Rel": "alternate",
        "Type": "image/png",
        "Title": "Download as PNG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=jpeg",
        "Rel": "alternate",
        "Type": "image/jpeg",
        "Title": "Download as JPEG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=bmp",
        "Rel": "alternate",
        "Type": "image/bmp",
        "Title": "Download as BMP"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=gif",
        "Rel": "alternate",
        "Type": "image/gif",
        "Title": "Download as GIF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=svg",
        "Rel": "alternate",
        "Type": "image/svg+xml",
        "Title": "Download as SVG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=html",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=htmlfixed",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTMLFIXED"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx?format=pcl",
        "Rel": "alternate",
        "Type": "application/x-pcl",
        "Title": "Download as PCL"
      }
    ],
    "FileName": "TestPostDocumentExecuteMailMerge.docx",
    "SourceFormat": "Docx",
    "IsEncrypted": false,
    "IsSigned": false,
    "DocumentProperties": {
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostDocumentExecuteMailMerge.docx/documentProperties",
        "Rel": "self"
      }
    }
  },
}
```

{{< /tab >}}
{{< /tabs >}}

**Case 2**: Mustache Template

You can use a sample **Input Document** [TestExecuteTemplate.doc](/words/attachments/884946/8028161.doc) and a sample **Mail Merge Data** [TestExecuteTemplateData.txt](/words/attachments/884946/8028162.txt). The **Output Document** would be as follows: [TestPostExecuteTemplate.docx](/words/attachments/884946/8028165.docx).

{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to populate Mustache template with Data
curl -v "https://api.aspose.cloud/v4.0/words/TestExecuteTemplate.doc/MailMerge?destFileName=TestPostExecuteTemplate.docx" \
-X PUT \
-F data=@TestExecuteTemplateData.txt \
-H "Content-Type: multipart/form-data" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
{
  "Document": {
    "Links": [
      {
        "Href": "TestPostExecuteTemplate.docx",
        "Rel": "self"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=doc",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=dot",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=docx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as DOCX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=docm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.document.macroEnabled.12",
        "Title": "Download as DOCM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=dotx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",
        "Title": "Download as DOTX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=dotm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.template.macroEnabled.12",
        "Title": "Download as DOTM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=flatopc",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as FLATOPC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=rtf",
        "Rel": "alternate",
        "Type": "application/rtf",
        "Title": "Download as RTF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=wml",
        "Rel": "alternate",
        "Type": "text/xml",
        "Title": "Download as WML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=odt",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text",
        "Title": "Download as ODT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=ott",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text-template",
        "Title": "Download as OTT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=txt",
        "Rel": "alternate",
        "Type": "text/plain",
        "Title": "Download as TXT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=mhtml",
        "Rel": "alternate",
        "Type": "multipart/related",
        "Title": "Download as MHTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=epub",
        "Rel": "alternate",
        "Type": "application/epub+zip",
        "Title": "Download as EPUB"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=pdf",
        "Rel": "alternate",
        "Type": "application/pdf",
        "Title": "Download as PDF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=xps",
        "Rel": "alternate",
        "Type": "application/vnd.ms-xpsdocument",
        "Title": "Download as XPS"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=tiff",
        "Rel": "alternate",
        "Type": "image/tiff",
        "Title": "Download as TIFF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=png",
        "Rel": "alternate",
        "Type": "image/png",
        "Title": "Download as PNG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=jpeg",
        "Rel": "alternate",
        "Type": "image/jpeg",
        "Title": "Download as JPEG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=bmp",
        "Rel": "alternate",
        "Type": "image/bmp",
        "Title": "Download as BMP"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=gif",
        "Rel": "alternate",
        "Type": "image/gif",
        "Title": "Download as GIF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=svg",
        "Rel": "alternate",
        "Type": "image/svg+xml",
        "Title": "Download as SVG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=html",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=htmlfixed",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTMLFIXED"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx?format=pcl",
        "Rel": "alternate",
        "Type": "application/x-pcl",
        "Title": "Download as PCL"
      }
    ],
    "FileName": "TestPostExecuteTemplate.docx",
    "SourceFormat": "Doc",
    "IsEncrypted": false,
    "IsSigned": false,
    "DocumentProperties": {
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestPostExecuteTemplate.docx/documentProperties",
        "Rel": "self"
      }
    }
  },
}
```

{{< /tab >}}
{{< /tabs >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples.

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="9" tabID="7" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "PostDocumentExecuteMailMerge.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostDocumentExecuteMailMerge.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "PostDocumentExecuteMailMerge.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "PostDocumentExecuteMailMerge.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "PostDocumentExecuteMailMerge.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "PostDocumentExecuteMailMerge.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostDocumentExecuteMailMerge.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostDocumentExecuteMailMerge.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "PostDocumentExecuteMailMerge.go" >}}
{{< /tab >}}
{{< /tabs >}}
