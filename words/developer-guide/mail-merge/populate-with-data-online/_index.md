---
title: "Populate Template with Data Online"
second_title: "Mail Merge"
type: docs
url: /mail-merge/populate-with-data-online/
aliases: [/populate-mailmerge-template-with-data-online/]
keywords: "Populate, mustache template, online, Mail Merge, Word, Microsoft Word"
description: "Populate a mail merge or mustache template with data online. You can download the SDK of your favorite language and start programming in the smartest way."
weight: 40
---

In this article, you will learn how to populate a mail merge or mustache template with data online. You can download the SDK of your favorite language and start programming in the smartest way. You can send both template file and mail merge data file in the request body and the API returns populated document in API response. [This API](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMergeOnline) represents a controller for executing a mail merge.

The following is a description of the most important parameters:

|Parameter Name|Description|
| :- | :- |
|withRegions|<p>Merge with regions or not. False by default.</p><p>Flag 'withRegions' can be omitted, in this case, a simple mail merge will be executed. If the flag is present and value is 'true' - mail merge with regions will be executed.</p>|
|cleanup|If the cleanup parameter is omitted, cleanup options will be None.|
|useWholeParagraphAsRegion|Specifies a value indicating whether a paragraph with TableStart or TableEnd field should be fully included in the mail merge region or particular range between TableStart and TableEnd fields. The default value is true.|

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

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMergeOnline) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

**Case 1**: MailMerge Template

You can use a sample **Input Document** [SampleMailMergeTemplate.docx](/words/mail-merge/SampleMailMergeTemplate.docx) and a sample **Mail Merge Data** [SampleMailMergeTemplateData.txt](/words/mail-merge/SampleMailMergeTemplateData.txt). The **Output Document** would be as follows: [TestPostDocumentExecuteMailMerge.docx](/words/mail-merge/TestPostDocumentExecuteMailMerge.docx).

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to populate MailMerge template with Data Online
curl -v "https://api.aspose.cloud/v4.0/words/MailMerge" \
-X PUT \
-F Template=@SampleMailMergeTemplate.docx \
-F Data=@SampleMailMergeTemplateData.txt \
-H "Content-Type: multipart/form-data" \
-H "Accept: multipart/form-data" \
-H "Authorization: Bearer <jwt token>" \
-o TestPostDocumentExecuteMailMerge.docx
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
Output Document: TestPostDocumentExecuteMailMerge.docx
```

{{< /tab >}}
{{< /tabs >}}

**Case 2**: Mustache Template

You can use a sample **Input Document** [TestExecuteTemplate.doc](/words/mail-merge/TestExecuteTemplate.doc) and a sample **Mail Merge Data** [TestExecuteTemplateData.txt](/words/mail-merge/TestExecuteTemplateData.txt). The **Output Document** would be as follows: TestPostExecuteTemplate.docx.

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

# cURL example to populate mustache template with data online
curl -v "https://api.aspose.cloud/v4.0/words/MailMerge" \
-X PUT \
-F Template=@TestExecuteTemplate.doc \
-F Data=@TestExecuteTemplateData.txt \
-H "Content-Type: multipart/form-data" \
-H "Accept: multipart/form-data" \
-H "Authorization: Bearer <jwt token>" \
-o TestPostExecuteTemplate.docx
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
Output Document: TestPostExecuteTemplate.docx
```

{{< /tab >}}
{{< /tabs >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< tabs tabTotal="9" tabID="7" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "PutExecuteMailMergeOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PutExecuteMailMergeOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "PutExecuteMailMergeOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "PutExecuteMailMergeOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "PutExecuteMailMergeOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "PutExecuteMailMergeOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PutExecuteMailMergeOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PutExecuteMailMergeOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "PutExecuteMailMergeOnline.go" >}}
{{< /tab >}}
{{< /tabs >}}
