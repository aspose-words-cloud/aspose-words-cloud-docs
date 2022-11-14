---
title: "Generate Report Online"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /report/build-online/
aliases: [/build-report-online/]
description: "Generate a report online"
weight: 20
---

Executes the report generation process online using the specified document template and the external data source in XML, JSON or CSV format.

## REST API

| Server                         | REST endpoint        | HTTP method  |
|--------------------------------|----------------------|--------------|
| https://api.aspose.cloud/v4.0  | [/words/buildReport](https://api.aspose.cloud/v4.0/words/buildReport) | PUT |

You can use these parameters in a REST request:

| Name                 | Type   | Description                                                  |
|----------------------|--------|--------------------------------------------------------------|
| `documentFileName`   | string | The filename of the output document, that will be used when the resulting document has a dynamic field {filename}. If it is not set, the "template" will be used instead. |


{{% alert style="info" %}}
**Note**: to access this REST API, you need to register and get personal credentials. Use the '[Quick Start](/getting-started/quickstart/)' guide to go through the procedure in a couple of minutes.
{{% /alert %}}


## Supported File Formats

The following input file formats are supported: DOC, DOT, DOCX, DOCM, DOTX, DOTM, FlatOPC (with and without macros), RTF, WordML, HTML, MHTHML, MOBI, CHM, AZW3, EPUB, ODT, OTT, TXT, Markdown, PDF, XML.

The following output file formats are supported: DOC, DOT, DOCX, DOCM, DOTX, DOTM, FlatOPC (with and without macros), RTF, WordML, HTML, MTHML, AZW3, EPUB, ODT, OTT, TXT, Markdown, PDF, XPS, XAML (fixed and flow), SVG, OpenXPS, PS, PCL, TIFF, PNG, BMP, EMF, JPG, GIF.


## Usage Examples

Let's look at practical examples of using the web service. You can do this both with cURL and Postman utilities, and from your code in various programming languages: Python, Java, JavaScript, C#, PHP, C++, Go, Ruby, Swift, Dart.

### How to Generate a report online using cURL or Postman

One of the easiest and fastest ways to call a REST API is to use cURL or Postman:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="cURL Request" tabName2="Postman Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "BuildReportOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "BuildReportOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


### How to Generate a report online using Python, Java, C#, C++, JavaScript and other programming languages

Using SDK is the quickest way to speed up the development. Please take a look at the provided code examples to quickly call this web service from your favourite programming language:

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="2" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "BuildReportOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "BuildReportOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "BuildReportOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "BuildReportOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "BuildReportOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "BuildReportOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "BuildReportOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "BuildReportOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "BuildReportOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "BuildReportOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

You can also visit our [GitHub repository](https://github.com/aspose-words-cloud) to explore a wide family of Aspose.Words Cloud SDKs. These software libraries take care of all low-level document-processing details and let you focus on your primary tasks.


