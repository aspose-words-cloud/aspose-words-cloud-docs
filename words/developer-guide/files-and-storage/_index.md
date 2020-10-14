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

## Downloading a file from the Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/{path}|GET|Download a File from Storage|[DownloadFile](https://apireference.aspose.cloud/words/#/File/DownloadFile)|

You can use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< nosnippet >}}
{{< tabs tabTotal="1" tabID="1" tabName1="Request" >}}
{{< tab tabNum="1" >}}

```bash
curl -v -X GET "https://api.aspose.cloud/v4.0/words/storage/file/sample.docx" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Uploading a file to the Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/{path}|PUT|Upload a file to Cloud Storage|[UploadFile](https://apireference.aspose.cloud/words/#/File/UploadFile)|

The following are a few examples of using cURL:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
curl  -v -X PUT "https://api.aspose.cloud/v4.0/words/storage/file/sample.docx" \
-H "Content-Type:application/octet-stream" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

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

## Copying a file to a new location in the Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/copy/{srcPath}|PUT|Duplicate a file to a new location on Cloud Storage|[CopyFile](https://apireference.aspose.cloud/words/#/File/CopyFile)|

The following are a few examples of using cURL:

{{< nosnippet >}}
{{< tabs tabTotal="1" tabID="8" tabName1="Request" >}}
{{< tab tabNum="1" >}}

```bash
curl -v -X PUT "https://api.aspose.cloud/v4.0/words/storage/file/copy/sample.docx/%2F?destPath=MyFolder" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Moving a file to a new location in the Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/MOVE/{srcPath}|PUT|Move a file to a new location on Cloud Storage|[MoveFile](https://apireference.aspose.cloud/words/#/File/MoveFile)|

The following are a few examples of using cURL:

{{< nosnippet >}}
{{< tabs tabTotal="1" tabID="11" tabName1="Request" >}}
{{< tab tabNum="1" >}}

```bash
curl -v -X PUT "https://api.aspose.cloud/v4.0/words/storage/file/move/input.docx/%2F?destPath=MyFolder" \
-H "Content-Type:application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Deleting a file from the Cloud Storage

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/{path}|DELETE|Delete a file from Cloud Storage|[DeleteFile](https://apireference.aspose.cloud/words/#/File/DeleteFile)|

The following are a few examples of using cURL:

{{< nosnippet >}}
{{< tabs tabTotal="1" tabID="14" tabName1="Request" >}}
{{< tab tabNum="1" >}}

```bash
curl -v -X DELETE "https://api.aspose.cloud/v4.0/words/storage/file/input.docx" \
-H "Content-Type:application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
