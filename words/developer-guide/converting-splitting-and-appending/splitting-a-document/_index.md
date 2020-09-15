---
title: "Splitting a Document"
type: docs
url: /splitting-a-document/
keywords: "Split word document, word to doc,save word file as pdf,convert word document to html,word doc to html,convert pdf to word,tiff file,Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift"
description: "While working with your documents, you may come across scenarios where you want to split the large documents into smaller ones. You can split the documents into separate documents within the MS Word document or different file formats. Splitting one large document into smaller documents of different file formats is an important aspect of document manipulation tasks. It involves a series of steps that need to be performed for getting the desired results. Aspose.Words Cloud eliminates the need for such complicated tasks and makes it hassle-free for you. You can perform this operation in various languages. Currently we support Python, C#, Java, Ruby, PHP, NodeJS, Go, Android and Swift."
weight: 30
---

## **Introduction**
While working with your documents, you may come across scenarios where you want to split the large documents into smaller ones. You can split the documents into separate documents within the MS Word document or different file formats. Splitting one large document into smaller documents of different file formats is an important aspect of document manipulation tasks. It involves a series of steps that need to be performed for getting the desired results. Aspose.Words Cloud eliminates the need for such complicated tasks and makes it hassle-free for you. Please note that we support Python, C#, Java, Ruby, PHP, NodeJS, Go, Android and Swift languages so far.

Aspose.Words Cloud has provided the simplest API to split a Word document within MS Word documents or other file formats.
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Split/SplitDocument) lets you call this REST API directly from the browser. The description of the important parameters of the API is given below:

|**Parameter Name**|**Type**|**Description**|
| :- | :- | :- |
|format|string|If the format is specified, the response contains the conversion data. Please see the table below for valid formats.|
|from|int|The start page number for splitting, if it is not specified, splitting starts from the first page of the document.|
|to|int|The last page number for splitting, if it is not specified, splitting ends at the last page of the document.|
|zipOutput|bool|ZipOutput or not.|
The **valid formats** are:

|**format Parameter Value**|**Format of the returned Page**|
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
|flatopc\_macro/fopc\_macro|...|
|flatopc\_template/fopc\_template|...|
|flatopc\_template\_macro/fopc\_template\_macro|...|
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
## **cURL Example**
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \

-X POST \

-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"

// cURL example to split a document

curl -v "https://api.aspose.cloud/v4.0/words/test\_doc.docx/split?from=2&to=3&format=pdf" \

-X PUT \

-H "Content-Type: application/json" \

-H "Accept: application/json" \

-H "Content-Length: 0" \

-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "SplitResult": {

    "SourceDocument": {

      "Href": "test\_doc.docx",

      "Rel": "self"

    },

    "Pages": [

      {

        "Href": "test\_doc\_page2.pdf",

        "Rel": "page"

      },

      {

        "Href": "test\_doc\_page3.pdf",

        "Rel": "page"

      }

    ]

  }

}

```

{{< /tab >}}

{{< /tabs >}}
## **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
### **Split all Pages to new PDFs**
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

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_SplitAllPagesToNewPDFs.java" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_SplitAllPagesToNewPDFs.swift" >}}

{{< /tab >}}

{{< tab tabNum="9" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "SplitAllPagesToNewPDFs.go" >}}

{{< /tab >}}

{{< /tabs >}}
### **Split specific pages to new PDFs**
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

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_SplitSpecificPagesToNewPDFs.java" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_SplitSpecificPagesToNewPDFs.swift" >}}

{{< /tab >}}

{{< tab tabNum="9" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "SplitSpecificPagesToNewPDFs.go" >}}

{{< /tab >}}

{{< /tabs >}}
### **Split specific pages to any Supported Format**
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

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_SplitSpecificPagesToPNGs.java" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_SplitSpecificPagesToPNGs.swift" >}}

{{< /tab >}}

{{< tab tabNum="9" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "SplitSpecificPagesToPNGs.go" >}}

{{< /tab >}}

{{< /tabs >}}

[ ](https://gist.github.com/aspose-words/d7482a8f2824fb669f7c31d8518ad13e#file-examples-ruby-splitresource-split_specific_pages_to_any_supported_format-rb)


