---
title: "Files and Storage"
second_title: "Aspose Words Cloud"
type: docs
url: /files-and-storage/
aliases: [/working-with-files-and-storage-using-aspose-words-cloud/]
description: "Learn how to work with Aspose Words Cloud file storage"
weight: 90
---

Aspose.Words Cloud provides helper functions to work with files uploaded to Aspose.Words Cloud Storage or any other Cloud Storage of your choice. If you need any help getting started with setting third party storage please refer to [Aspose Cloud UI Help Topics](https://docs.aspose.cloud/display/totalcloud/Aspose+Cloud+UI+Help+Topics).

## Downloading a file from Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/{path}|GET|Download a File from Storage|[DownloadFile](https://apireference.aspose.cloud/words/#/File/DownloadFile)|

You can use cURL command-line utility to test this REST API. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="1" tabID="1" tabName1="Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetFilesList.curl" >}}
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Uploading a file to Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/{path}|PUT|Upload a file to Cloud Storage|[UploadFile](https://apireference.aspose.cloud/words/#/File/UploadFile)|

The following code demonstrates how to upload a file to Cloud Storage with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="4" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "UploadFile.curl" >}}
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "UploadFile.json" >}}
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
   "uploaded":[
      "sample.docx"
   ],
   "errors":[
   ]
}
```
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Copying a file to a new location in Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/copy/{srcPath}|PUT|Duplicate a file to a new location on Cloud Storage|[CopyFile](https://apireference.aspose.cloud/words/#/File/CopyFile)|

The following code demonstrates how to copy a file to a new location in Cloud Storage with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="1" tabID="8" tabName1="Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "CopyFile.curl" >}}
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Moving a file to a new location in Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/MOVE/{srcPath}|PUT|Move a file to a new location on Cloud Storage|[MoveFile](https://apireference.aspose.cloud/words/#/File/MoveFile)|

The following code demonstrates how to move a file to a new location in Cloud Storage with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="1" tabID="11" tabName1="Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "MoveFile.curl" >}}
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Deleting a file from Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/{path}|DELETE|Delete a file from Cloud Storage|[DeleteFile](https://apireference.aspose.cloud/words/#/File/DeleteFile)|

The following code demonstrates how to delete a file from Cloud Storage with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="1" tabID="14" tabName1="Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "DeleteFile.curl" >}}
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
