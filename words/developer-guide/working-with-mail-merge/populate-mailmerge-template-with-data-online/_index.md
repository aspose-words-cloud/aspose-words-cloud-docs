---
title: "Populate MailMerge Template with Data Online"
type: docs
url: /populate-mailmerge-template-with-data-online/
aliases: [/populate-mailmerge-template-with-data-online/]
keywords: "Populate, mustache template, online, Mail Merge, Word, Microsoft Word, Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "In this article, you will learn how to populate a mail merge or mustache template with data online in various languages. You can download the SDK of your favorite language and start programming in the smartest way. The SDKs are available in Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android and Go languages."
weight: 20
---

In this article, you will learn how to populate a mail merge or mustache template with data online in various languages. You can download the SDK of your favorite language and start programming in the smartest way. The SDKs are available in Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android and Go languages. You can send both template file and mail merge data file in the request body and the API returns populated document in API response. [This API](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMergeOnline) represents a controller for executing a mail merge. Description of some important parameters of the API is given below:

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

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMergeOnline) lets you call this REST API directly from the browser. The description of the API and its parameters is also given there.

## cURL Example

**Case 1: MailMerge Template**

**Input Document:** [SampleMailMergeTemplate.docx](attachments/884946/1180099.docx)

**Mail Merge Data:** [SampleMailMergeTemplateData.txt](attachments/884946/1180097.txt)

**Output Document:** [TestPostDocumentExecuteMailMerge.docx](attachments/884946/8028163.docx)

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to populate MailMerge template with Data Online
curl -v "https://api.aspose.cloud/v4.0/words/MailMerge" \
-X PUT \
-F Template=@SampleMailMergeTemplate.docx \
-F Data=@SampleMailMergeTemplateData.txt \
-H "Content-Type: multipart/form-data" \
-H "Accept: multipart/form-data" \
-H "Authorization: Bearer <jwt token>" \
-o TestPostDocumentExecuteMailMerge.docx
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
Output Document: TestPostDocumentExecuteMailMerge.docx
```

{{< /tab >}}
{{< /tabs >}}
**Case 2: Mustache Template**

**Input Document:** [TestExecuteTemplate.doc](attachments/884965/7209026.doc)

**Mail Merge Data:** [TestExecuteTemplateData.txt](attachments/884965/7209027.txt)

**Output Document:** TestPostExecuteTemplate.docx

{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to populate mustache template with data online
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
```java
Output Document: TestPostExecuteTemplate.docx
```

{{< /tab >}}
{{< /tabs >}}
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples.

## SDK Examples

Code examples for various SDKs are presented below:
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
