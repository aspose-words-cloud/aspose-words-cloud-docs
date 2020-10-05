---
title: "Split"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /split/
aliases: [/splitting-a-document/]
keywords: "Split Word document, word to doc, save Word file as PDF, convert Word document to HTML, DOC to HTML, PDF to Word, TIFF file"
description: "Split a Word document"
weight: 240
---

Splitting a large Word document into multiple smaller documents is a common document automation task. You must have been in a situation when you have a massive DOCX, DOC, RTF file, requiring urgent team work. In this case, it is pretty necessary to split your document into several parts to speed up the collaborative workflow.

Splitting a Word document by hand with manual copying and pasting may be a long, labor-intensive, sub-optimal approach. Instead you can improve your efficiency dramatically with this API by splitting Word document into multiple files, while specifying operation parameters as you need.

Using this API you can easily split a DOCX, DOC, DOTX, DOT, RTF, ODT, OTT, TXT document and save the results to DOCX, DOC, PDF, ODT, RTF, HTML, JPEG, PNG and many other file formats.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Split/SplitDocument) lets you call this REST API directly from a browser. The description of the important parameters of the API is given below:

|Parameter Name|Type|Description|
| :- | :- | :- |
|format|string|If the format is specified, the response contains the conversion data. Please see the table below for valid formats.|
|from|int|The start page number for splitting, if it is not specified, splitting starts from the first page of the document.|
|to|int|The last page number for splitting, if it is not specified, splitting ends at the last page of the document.|
|zipOutput|bool|ZipOutput or not.|

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to split a document
curl -v "https://api.aspose.cloud/v4.0/words/test_doc.docx/split?from=2&to=3&format=pdf" \
-X PUT \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Content-Length: 0" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

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

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

### Split all Pages to new PDFs

**Split all pages**

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "SplitAllPagesToNewPDFs.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "SplitAllPagesToNewPDFs.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "SplitAllPagesToNewPDFs.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "" "fb014f439299bbee24472cb0efa6d50b" "SplitAllPagesToNewPDFs.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "" "3f3f4f7033ae386af05042ee2ad3aa06" "SplitAllPagesToNewPDFs.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "SplitAllPagesToNewPDFs.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_SplitAllPagesToNewPDFs.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_SplitAllPagesToNewPDFs.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "SplitAllPagesToNewPDFs.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
### Split specific pages to new PDFs

**Split specific pages**

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="5" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "SplitSpecificPagesToNewPDFs.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "SplitSpecificPagesToNewPDFs.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "SplitSpecificPagesToNewPDFs.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "" "fb014f439299bbee24472cb0efa6d50b" "SplitSpecificPagesToNewPDFs.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "" "3f3f4f7033ae386af05042ee2ad3aa06" "SplitSpecificPagesToNewPDFs.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "SplitSpecificPagesToNewPDFs.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_SplitSpecificPagesToNewPDFs.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_SplitSpecificPagesToNewPDFs.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "SplitSpecificPagesToNewPDFs.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
### Split specific pages to any Supported Format

**split document to any format**

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="6" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "SplitSpecificPagesToPNGs.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "SplitSpecificPagesToPNGs.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "SplitSpecificPagesToPNGs.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "" "fb014f439299bbee24472cb0efa6d50b" "SplitSpecificPagesToPNGs.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "" "3f3f4f7033ae386af05042ee2ad3aa06" "SplitSpecificPagesToPNGs.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "SplitSpecificPagesToPNGs.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_SplitSpecificPagesToPNGs.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_SplitSpecificPagesToPNGs.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "SplitSpecificPagesToPNGs.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
[ ](https://gist.github.com/aspose-words/d7482a8f2824fb669f7c31d8518ad13e#file-examples-ruby-splitresource-split_specific_pages_to_any_supported_format-rb).

## See also

- Product page description: <a href="https://products.aspose.cloud/words/python/split" target="_blank">Python</a>, <a href="https://products.aspose.cloud/words/net/split" target="_blank">C#</a>, <a href="https://products.aspose.cloud/words/java/split" target="_blank">Java</a>, <a href="https://products.aspose.cloud/words/nodejs/split" target="_blank">Node.js</a>, <a href="https://products.aspose.cloud/words/php/split" target="_blank">PHP</a>, <a href="https://products.aspose.cloud/words/go/split" target="_blank">Go</a>
- <a href="https://products.aspose.app/words/splitter" target="_blank">Free online splitter app
