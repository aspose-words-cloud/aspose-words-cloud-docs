---
title: "Convert Word Document from Request Content to Specified Format"
type: docs
url: /convert/specified-format/
aliases: [/convert-word-document-from-request-content-to-specified-format/]
keywords: "convert to, word to doc,save word file as pdf,convert word document to html,word doc to html,convert pdf to word,tiff file, Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift"
description: "You can easily convert word document to PDF, HTML, XHTML or a specified format from a URL request content. We support Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift. The API request contains a document to convert and the response contains the conversion result, or if the output parameter specified - the API saves the result to the Cloud storage and return OK status code. "
weight: 10
---

You can check the quality of Aspose.Words Cloud conversion and view the results online at these links:

- [Conversion](https://products.aspose.app/words/conversion)
- [Viewer](https://products.aspose.app/words/viewer)

## Introduction

[PUT /words/convert](https://apireference.aspose.cloud/words/#/Convert/ConvertDocument) API lets you convert MS Word document to another format. The API request contains a document to convert and the response contains the conversion result, or if outPath parameter specified - the API saves the result to the Cloud storage and return OK status code. The list of supported formats are:

|format Parameter Value|Format of the returned Presentation|
| :- | :- |
|bmp|Bitmap image file|
|doc|Word document|
|docm|Word Open XML Macro-Enabled Document|
|docx|Microsoft Word Open XML Document|
|dot|Word Document Template|
|dotm|Word Open XML Macro-Enabled Document Template|
|dotx|Word Open XML Document Template|
|emf|Enhanced Windows Metafile|
|epub|Open eBook File|
|flatopc|Flat OPC format|
|gif|Gif Image|
|html|Hypertext Markup Language File|
|jpeg|JPEG Image|
|mhtml|MIME HTML File|
|odt|OpenDocument Text Document|
|ott|OpenDocument Document Template|
|pcl|Printer Command Language File|
|pdf|Portable Document Format File|
|png|Portable Network Graphic|
|rtf|Rich Text Format File|
|svg|Scalable Vector Graphics File|
|swf|Shockwave Flash Movie(removed)|
|txt|Plain Text File|
|tiff|Tagged Image File Format|
|wml|Wireless Markup Language File|
|xps|XML Paper Specification File|

The most important parameters of this API are listed in the following table:

|Parameter Name|Type|Query String|Description|
| :- | :- | :- | :- |
|format|string|format=jpeg|Return the document in the specified format. Valid values for this parameter are given above.|
|outPath|string|outPath=SomeFolder/result.jpeg|A path for saving operation results to the Cloud storage.|

The format can also be specified by the request Accept header.

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Convert/ConvertDocument) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

**Input Document**: [TableDocument.doc](attachments/885335/1180089.doc)

**Output Document**: [TableDocument.pdf](attachments/885335/1180090.pdf)** 

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

# cURL example to convert MS Word Document to PDF
curl -v "https://api.aspose.cloud/v4.0/words/convert?format=pdf" \
-X PUT \
-F document=@TableDocument.doc \
-H "Content-Type: multipart/form-data" \
-H "Accept: multipart/form-data" \
-H "Authorization: Bearer <jwt token>" \
-o TableDocument.pdf
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
PDF Document 
```

{{< /tab >}}
{{< /tabs >}}

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples.

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "ConvertWordDocumentToAnotherFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "ConvertWordDocumentToAnotherFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "ConvertWordDocumentToAnotherFormat.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "ConvertWordDocumentToAnotherFormat.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "ConvertWordDocumentToAnotherFormat.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "ConvertWordDocumentToAnotherFormat.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_ConvertWordDocumentToAnotherFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_ConvertWordDocumentToAnotherFormat.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "ConvertWordDocumentToAnotherFormat.go" >}}
{{< /tab >}}
{{< /tabs >}}
