---
title: "Split a Document"
type: docs
url: /split/
aliases: [/splitting-a-document/]
keywords: "Split Word document, word to doc,save word file as pdf,convert word document to html,word doc to html,convert pdf to word,tiff file,Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift"
description: "Split Word documents. Aspose Words Cloud provide various SDKs to split files."
weight: 12
---

While working with your documents, you may come across scenarios where you want to split the large documents into smaller ones. You can split the documents into separate documents within the MS Word document or different file formats. Splitting one large document into smaller documents of different file formats is an important aspect of document manipulation tasks. It involves a series of steps that need to be performed for getting the desired results. Aspose.Words Cloud eliminates the need for such complicated tasks and makes it hassle-free for you. Please note that we support Python, C#, Java, Ruby, PHP, NodeJS, Go, Android and Swift languages so far.

Aspose.Words Cloud has provided the simplest API to split a Word document within MS Word documents or other file formats.

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Split/SplitDocument) lets you call this REST API directly from a browser. The description of the important parameters of the API is given below:

|Parameter Name|Type|Description|
| :- | :- | :- |
|format|string|If the format is specified, the response contains the conversion data. Please see the table below for valid formats.|
|from|int|The start page number for splitting, if it is not specified, splitting starts from the first page of the document.|
|to|int|The last page number for splitting, if it is not specified, splitting ends at the last page of the document.|
|zipOutput|bool|ZipOutput or not.|
The **valid formats** are:

|format Parameter Value|Format of the returned Page|
| :- | :- |
|bmp|Bitmap Picture|
|doc|...|
|docm|...|
|docx|...|
|dot|...|
|dotm|...|
|dotx|...|
|emf|Enhanced Metafile Format|
|epub|...|
|flatopc/fopc|...|
|flatopc_macro/fopc_macro|...|
|flatopc_template/fopc_template|...|
|flatopc_template_macro/fopc_template_macro|...|
|jpeg/jpg|Joint Photographic Experts Group Image Format|
|html|...|
|htmlfixed|...|
|mhtml/mht|...|
|odt|...|
|openxps|...|
|ott|...|
|pcl|Printer Command Language Format|
|pdf|Portable Document Format|
|png|Portable Networks Graphic Image Format|
|ps|...|
|rtf|...|
|svg|...|
|text/txt|...|
|tiff/tif|Tagged Image File Format|
|wordml/wml|...|
|xps|...|
|xamlfixed|...|

**Example 1**

Split all pages from the document into PDF format:

PUT <https://api.aspose.cloud/v4.0/words/TestSplitDocument.doc/split?format=pdf>

**Example 2**

Split pages 2-3 from the document into PDF format:

PUT <https://api.aspose.cloud/v4.0/words/TestSplitDocument.doc/split?from=2&to=3&format=pdf>

**Example 3**

Split pages 2-3 from the document into JPEG format where the input document is saved in a particular folder, not on the root of the storage:

PUT <https://api.aspose.cloud/v4.0/words/TestSplitDocument.doc/split?from=2&to=3&format=jpeg&folder=SomeFolder>

**Example 4**

Split all pages from the document into PDF format and zip files:

PUT <https://api.aspose.cloud/v4.0/words/TestSplitDocument.doc/split?format=pdf&zipOutput=true>

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to split a document
curl -v "https://api.aspose.cloud/v4.0/words/test_doc.docx/split?from=2&to=3&format=pdf" \
-X PUT \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Content-Length: 0" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
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

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

### Split all Pages to new PDFs

**Split all pages**

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
### Split specific pages to new PDFs

**Split specific pages**

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
### Split specific pages to any Supported Format

**split document to any format**

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
[ ](https://gist.github.com/aspose-words/d7482a8f2824fb669f7c31d8518ad13e#file-examples-ruby-splitresource-split_specific_pages_to_any_supported_format-rb)

