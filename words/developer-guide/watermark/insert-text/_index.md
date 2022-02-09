---
title: "Insert a Watermark Text into a Word Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /watermark/insert-text/
aliases: [/insert-a-watermark-text-into-a-word-document/]
description: "Insert a watermark text into a Word document"
weight: 30
---

This REST API insert a `Watermark` text. The object will appear as a `Watermark` throughout the document. 

The important request parameters are the following:

|Parameter Name|Type|Query String/HTTP Body|Description|
| :- | :- | :- | :- |
|watermarkText |string|Query String/HTTP Body: text=DRAFT|Watermark text.|

## Usage examples with cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "InsertWatermarkTextOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "InsertWatermarkTextOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
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
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=doc",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=dot",
        "Rel": "alternate",
        "Type": "application/msword",
        "Title": "Download as DOT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=docx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as DOCX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=docm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.document.macroEnabled.12",
        "Title": "Download as DOCM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=dotx",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",
        "Title": "Download as DOTX"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=dotm",
        "Rel": "alternate",
        "Type": "application/vnd.ms-word.template.macroEnabled.12",
        "Title": "Download as DOTM"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=flatopc",
        "Rel": "alternate",
        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
        "Title": "Download as FLATOPC"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=rtf",
        "Rel": "alternate",
        "Type": "application/rtf",
        "Title": "Download as RTF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=wml",
        "Rel": "alternate",
        "Type": "text/xml",
        "Title": "Download as WML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=odt",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text",
        "Title": "Download as ODT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=ott",
        "Rel": "alternate",
        "Type": "application/vnd.oasis.opendocument.text-template",
        "Title": "Download as OTT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=txt",
        "Rel": "alternate",
        "Type": "text/plain",
        "Title": "Download as TXT"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=mhtml",
        "Rel": "alternate",
        "Type": "multipart/related",
        "Title": "Download as MHTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=epub",
        "Rel": "alternate",
        "Type": "application/epub+zip",
        "Title": "Download as EPUB"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=pdf",
        "Rel": "alternate",
        "Type": "application/pdf",
        "Title": "Download as PDF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=xps",
        "Rel": "alternate",
        "Type": "application/vnd.ms-xpsdocument",
        "Title": "Download as XPS"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=tiff",
        "Rel": "alternate",
        "Type": "image/tiff",
        "Title": "Download as TIFF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=png",
        "Rel": "alternate",
        "Type": "image/png",
        "Title": "Download as PNG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=jpeg",
        "Rel": "alternate",
        "Type": "image/jpeg",
        "Title": "Download as JPEG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=bmp",
        "Rel": "alternate",
        "Type": "image/bmp",
        "Title": "Download as BMP"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=gif",
        "Rel": "alternate",
        "Type": "image/gif",
        "Title": "Download as GIF"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=svg",
        "Rel": "alternate",
        "Type": "image/svg+xml",
        "Title": "Download as SVG"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=html",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTML"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=htmlfixed",
        "Rel": "alternate",
        "Type": "text/html",
        "Title": "Download as HTMLFIXED"
      },
      {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx?format=pcl",
        "Rel": "alternate",
        "Type": "application/x-pcl",
        "Title": "Download as PCL"
      }
    ],
    "FileName": "test_multi_pages.docx",
    "SourceFormat": 4,
    "IsEncrypted": false,
    "IsSigned": false,
    "DocumentProperties": {
      "List": null,
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties",
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

The following code samples show how to interact with REST API using almost any mainstream programming language. You can find a lot of other code examples in [Python](https://gist.github.com/aspose-words-cloud-gists/e26813ced70692c544820cd8011ee7e0), [Java](https://gist.github.com/aspose-words-cloud-gists/caede439bfd2e57c3010befe504faff4), [C#](https://gist.github.com/aspose-words-cloud-gists/374e1e3dd4bca8f696f29d913645f549), [JavaScript](https://gist.github.com/aspose-words-cloud-gists/a9510e4b51613f1138e7c1ec09634c4a), [PHP](https://gist.github.com/aspose-words-cloud-gists/e2a72445b96362dc0117f06ab54bb94a), [C++](https://gist.github.com/aspose-words-cloud-gists/49aa5151a094849179bae8672c887a0e), [Golang](https://gist.github.com/aspose-words-cloud-gists/625ca80adffd779e8f6e3611551e14d5), [Ruby](https://gist.github.com/aspose-words-cloud-gists/339f3835a4c0a536c81ec941de29baf7), [Swift](https://gist.github.com/aspose-words-cloud-gists/790dbd2edd5d36f170732366f52cac4c), [Dart](https://gist.github.com/aspose-words-cloud-gists/6aae628cf2b878b78fea177c3171c6bf) on GitHub. All codes are thoroughly tested and ready for production use.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "InsertWatermarkTextOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "InsertWatermarkTextOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "InsertWatermarkTextOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "InsertWatermarkTextOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "InsertWatermarkTextOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "InsertWatermarkTextOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "InsertWatermarkTextOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "InsertWatermarkTextOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "InsertWatermarkTextOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "InsertWatermarkTextOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
