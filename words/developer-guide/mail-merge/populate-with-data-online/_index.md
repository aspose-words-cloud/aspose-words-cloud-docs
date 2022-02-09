---
title: "Populate Template with Data Online"
second_title: "Mail Merge"
type: docs
url: /mail-merge/populate-with-data-online/
aliases: [/populate-mailmerge-template-with-data-online/]
keywords: "Populate, mustache template, online, Mail Merge, Word, Microsoft Word"
description: "Populate a mail merge or mustache template with data online"
weight: 40
---

In this article, you will learn how to populate a **Mail Merge** or mustache template with data online. You can download the SDK of your favorite language and start programming in the smartest way. You can send both template file and mail merge data file in the request body and the API returns populated document in API response. [This API](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMergeOnline) represents a controller for executing a mail merge.

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

## Data Formats

Both **JSON** and **XML** data formats are supported. Choosing the appropriate data format makes a difference in flexibility, scalability and performance speed of your application. XML and JSON have much in common with their own strengths and drawbacks. You need to determine which one is the most preferred for your purposes.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/MailMerge/ExecuteMailMergeOnline) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

**Case 1**: MailMerge Template

Feel free to download and explore sample input [SampleMailMergeTemplate.docx](/words/mail-merge/SampleMailMergeTemplate.docx), [SampleMailMergeTemplateData.xml](/words/mail-merge/SampleMailMergeTemplateData.xml) and output [TestPostDocumentExecuteMailMerge.docx](/words/mail-merge/TestPostDocumentExecuteMailMerge.docx) files designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "ExecuteMailMergeOnline.curl" >}}
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "ExecuteMailMergeOnline.json" >}}
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< tab tabNum="3" >}}
```json
Output Document: TestPostDocumentExecuteMailMerge.docx
```
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 2**: Mustache Template

Feel free to download and explore sample input [TestExecuteTemplate.doc](/words/mail-merge/TestExecuteTemplate.doc), [TestExecuteTemplateData.xml](/words/mail-merge/TestExecuteTemplateData.xml) and output [TestPostExecuteTemplate.docx](/words/mail-merge/TestPostExecuteTemplate.docx) files designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="4" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your `Client Id` and `Secret` credentials from https://dashboard.aspose.cloud/applications.
# Place `Client Id` in client_id argument. Place `Secret` in client_secret argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to populate mustache template with data online
curl -v "https://api.aspose.cloud/v4.0/words/MailMerge" \
-X PUT \
-F Template=@TestExecuteTemplate.doc \
-F Data=@TestExecuteTemplateData.xml \
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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="11" tabID="7" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" tabName11="Curl" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "ExecuteMailMergeOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "ExecuteMailMergeOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "ExecuteMailMergeOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "ExecuteMailMergeOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "ExecuteMailMergeOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "ExecuteMailMergeOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "ExecuteMailMergeOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "ExecuteMailMergeOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "ExecuteMailMergeOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "ExecuteMailMergeOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
