---
title: "Create a New Word Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /documents/create/
aliases: [/create-a-new-word-document/]
description: "Create a new word document"
weight: 10
---

This REST API creates a new `Document` with a format, specified by file extension.

The supported formats are:

|Format|Extension|Description|
| :- | :- | :- |
|[Doc](https://docs.fileformat.com/word-processing/doc/)|".doc"|Microsoft Word 97 - 2007 Document format|
|[Docx](https://docs.fileformat.com/word-processing/docx/)|".docx"|Office Open XML WordprocessingML Document (macro-free)|
|[Docm](https://docs.fileformat.com/word-processing/docm/)|".docm"|Office Open XML WordprocessingML Macro-Enabled Document|
|[Dot](https://docs.fileformat.com/word-processing/dot/)|".dot"|Microsoft Word 97 - 2007 Template format|
|[Dotm](https://docs.fileformat.com/word-processing/dotm/)|".dotm"|Office Open XML WordprocessingML Macro-Enabled Template|
|[Dotx](https://docs.fileformat.com/word-processing/dotx/)|".dotx"|Office Open XML WordprocessingML Template (macro-free)|
|[FlatOpc](#)|".flatopc", ".fopc"|Office Open XML WordprocessingML stored in a flat XML file instead of a ZIP package|
|[FlatOpcMacroEnabled](#)|".flatopc_macro", ".fopc_macro"|Office Open XML WordprocessingML Macro-Enabled Document stored in a flat XML file instead of a ZIP package.|
|[FlatOpcTemplate](#)|".flatopc_template", ".fopc_template"|Office Open XML WordprocessingML Template (macro-free) stored in a flat XML file instead of a ZIP package.|
|[FlatOpcTemplateMacroEnabled](#)|".flatopc_template_macro", ".fopc_template_macro"|Office Open XML WordprocessingML Macro-Enabled Template stored in a flat XML file instead of a ZIP package.|
|[WordML](#)|".wordml", ".wml"|Microsoft Word 2003 WordprocessingML format.|
|[Rtf](https://docs.fileformat.com/word-processing/rtf/)|".rtf"|RTF format. All characters above 7-bits are escaped as hexadecimal or Unicode characters|

and Request parameters are the following:

|Parameter Name|Query String/HTTPBody|Description|
| :- | :- | :- |
|fileName|Query String: fileName=documentName.docx|The file name.|

## Usage examples with cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "CreateDocument.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "CreateDocument.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "Document": {
    "Links": [
      {
        "Href": "TestDocument.docx",
        "Rel": "self",
        "Type": null,
        "Title": null
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=doc",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=dot",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=docx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as DOCX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=docm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.document.macroEnabled.12",
        "Title": "Download as DOCM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=dotx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",
        "Title": "Download as DOTX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=dotm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.template.macroEnabled.12",
        "Title": "Download as DOTM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=flatopc",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as FLATOPC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=rtf",
        "Rel": "alternate",
        "Type": "application/rtf",
        "Title": "Download as RTF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=wml",
        "Rel": "alternate",
        "Type": "text/xml",
        "Title": "Download as WML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=odt",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text",
        "Title": "Download as ODT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=ott",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text-template",
        "Title": "Download as OTT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=txt",
        "Rel": "alternate",
        "Type": "text/plain",
        "Title": "Download as TXT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=mhtml",
        "Rel": "alternate",
        "Type": "multipart/related",
        "Title": "Download as MHTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=epub",
        "Rel": "alternate",
        "Type": "application/epub+zip",
        "Title": "Download as EPUB"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=pdf",
        "Rel": "alternate",
        "Type": "application/pdf",
        "Title": "Download as PDF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=xps",
        "Rel": "alternate",
        "Type": "application/vnd.ms-xpsdocument",
        "Title": "Download as XPS"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=tiff",
        "Rel": "alternate",
        "Type": "image/tiff",
        "Title": "Download as TIFF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=png",
        "Rel": "alternate",
        "Type": "image/png",
        "Title": "Download as PNG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=jpeg",
        "Rel": "alternate",
        "Type": "image/jpeg",
        "Title": "Download as JPEG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=bmp",
        "Rel": "alternate",
        "Type": "image/bmp",
        "Title": "Download as BMP"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=gif",
        "Rel": "alternate",
        "Type": "image/gif",
        "Title": "Download as GIF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=svg",
        "Rel": "alternate",
        "Type": "image/svg+xml",
        "Title": "Download as SVG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=html",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=htmlfixed",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTMLFIXED"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx?format=pcl",
        "Rel": "alternate",
        "Type": "application/x-pcl",
        "Title": "Download as PCL"
      }
    ],
    "FileName": "TestDocument.docx",
    "SourceFormat": 4,
    "IsEncrypted": false,
    "IsSigned": false,
    "DocumentProperties": {
      "List": null,
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestDocument.docx/documentProperties",
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
{{< /nosnippet >}}

## Aspose.Words Cloud SDK Family

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Usage examples in Python, Java, C#, etc.

The following code samples show how to interact with the REST API using almost any mainstream programming language.

You can find a lot of other examples in [Python](https://gist.github.com/aspose-words-cloud-gists/e26813ced70692c544820cd8011ee7e0), [Java](https://gist.github.com/aspose-words-cloud-gists/caede439bfd2e57c3010befe504faff4), [C#](https://gist.github.com/aspose-words-cloud-gists/374e1e3dd4bca8f696f29d913645f549), [JavaScript](https://gist.github.com/aspose-words-cloud-gists/a9510e4b51613f1138e7c1ec09634c4a), [PHP](https://gist.github.com/aspose-words-cloud-gists/e2a72445b96362dc0117f06ab54bb94a), [C++](https://gist.github.com/aspose-words-cloud-gists/49aa5151a094849179bae8672c887a0e), [Golang](https://gist.github.com/aspose-words-cloud-gists/625ca80adffd779e8f6e3611551e14d5), [Ruby](https://gist.github.com/aspose-words-cloud-gists/339f3835a4c0a536c81ec941de29baf7), [Swift](https://gist.github.com/aspose-words-cloud-gists/790dbd2edd5d36f170732366f52cac4c), [Dart](https://gist.github.com/aspose-words-cloud-gists/6aae628cf2b878b78fea177c3171c6bf) on GitHub. All codes are thoroughly tested and ready for production use.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "CreateDocument.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "CreateDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "CreateDocument.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "CreateDocument.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "CreateDocument.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "CreateDocument.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "CreateDocument.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "CreateDocument.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "CreateDocument.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "CreateDocument.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
