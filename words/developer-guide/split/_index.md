---
title: "Split"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /split/
aliases: [/splitting-a-document/]
keywords: ""
description: "Split Word documents. Split DOCX into small PDF, Word files with ease."
weight: 240
---

Aspose provides a powerful API to split Word documents. It's a common document automation task when you need to break a large document into a number of smaller ones to handle them separately.

For example, you must have been in a situation when you have a massive [DOCX](https://docs.fileformat.com/word-processing/docx/) file, requiring urgent team work. In this case, it is pretty necessary to divide a Word document into sub-documents to speed up the collaborative workflow.

Task to split a [DOCX](https://docs.fileformat.com/word-processing/docx/) document by hand with manual copying and pasting may be a long, labor-intensive, sub-optimal approach. Instead, you can improve your efficiency dramatically with this API by breaking Word document into files, while specifying operation parameters as you need.

Using this API you can easily split a [DOC](https://docs.fileformat.com/word-processing/doc/), [DOT](https://docs.fileformat.com/word-processing/dot/), [DOCX](https://docs.fileformat.com/word-processing/docx/), [DOTX](https://docs.fileformat.com/word-processing/dotx/), [RTF](https://docs.fileformat.com/word-processing/rtf/), [ODT](https://docs.fileformat.com/word-processing/odt/), [OTT](https://docs.fileformat.com/word-processing/ott/), [TXT](https://docs.fileformat.com/word-processing/txt/) document and save the results to [DOC](https://docs.fileformat.com/word-processing/doc/), [DOCX](https://docs.fileformat.com/word-processing/docx/), [PDF](https://docs.fileformat.com/pdf/), [ODT](https://docs.fileformat.com/word-processing/odt/), [RTF](https://docs.fileformat.com/word-processing/rtf/), [HTML](https://docs.fileformat.com/web/html/), [JPEG](https://docs.fileformat.com/image/jpeg/), [PNG](https://docs.fileformat.com/Image/png/) and many other file formats.

## REST API calls using cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "SplitDocumentOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "SplitDocumentOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "SplitResult": {
    "SourceDocument": {
      "Href": "test_doc.docx",
      "Rel": "self"
    },
    "Pages": [
      {
        "Href": "test_doc_page2.pdf",
        "Rel": "page"
      },
      {
        "Href": "test_doc_page3.pdf",
        "Rel": "page"
      }
    ]
  }
}
```
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Code samples in Python, Java, C#, etc.

The following code samples show how to interact with REST API using almost any mainstream programming language (Python, Java, C#, JavaScript, PHP, C++, Golang, Ruby, Swift, Dart):

### Split DOCX to PDFs

The following code examples demonstrate how to split all pages in a Word document.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "SplitDocumentOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "SplitDocumentOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "SplitDocumentOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "SplitDocumentOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "SplitDocumentOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "SplitDocumentOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "SplitDocumentOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "SplitDocumentOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "SplitDocumentOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "SplitDocumentOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

### Split specific pages to PDFs

The following code examples demonstrate how to split specific pages of a Word document.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "SplitDocumentOnline_2.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "SplitDocumentOnline_2.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "SplitDocumentOnline_2.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "SplitDocumentOnline_2.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "SplitDocumentOnline_2.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "SplitDocumentOnline_2.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "SplitDocumentOnline_2.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "SplitDocumentOnline_2.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "SplitDocumentOnline_2.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "SplitDocumentOnline_2.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

### Split specific pages to any Supported Format

The following code examples demonstrate how to split a Word document to any format.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "SplitDocumentOnline_1.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "SplitDocumentOnline_1.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "SplitDocumentOnline_1.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "SplitDocumentOnline_1.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "SplitDocumentOnline_1.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "SplitDocumentOnline_1.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "SplitDocumentOnline_1.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "SplitDocumentOnline_1.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "SplitDocumentOnline_1.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "SplitDocumentOnline_1.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See also

- Product page description: <a href="https://products.aspose.cloud/words/python/split" target="_blank">Python</a>, <a href="https://products.aspose.cloud/words/net/split" target="_blank">C#</a>, <a href="https://products.aspose.cloud/words/java/split" target="_blank">Java</a>, <a href="https://products.aspose.cloud/words/nodejs/split" target="_blank">Node.js</a>, <a href="https://products.aspose.cloud/words/php/split" target="_blank">PHP</a>, <a href="https://products.aspose.cloud/words/go/split" target="_blank">Go</a>
- <a href="https://products.aspose.app/words/splitter" target="_blank" rel="noopener">Free online splitter app</a>
