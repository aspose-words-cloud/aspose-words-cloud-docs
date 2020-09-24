---
title: "Files and Storage in Aspose Cloud"
type: docs
url: /files-and-storage/
aliases: [/working-with-files-and-storage-using-aspose-words-cloud/]
weight: 30
---

Aspose.Words Cloud provides helper functions to work with files uploaded to Aspose.Words Cloud Storage or any other Cloud Storage of your choice. If you need any help getting started with setting third party storage please refer to [Aspose Cloud UI Help Topics](https://docs.aspose.cloud/display/totalcloud/Aspose+Cloud+UI+Help+Topics).

### Download a file from Cloud Storage

#### API Information

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/{path}|GET|Download a File from Storage|[DownloadFile](https://apireference.aspose.cloud/words/#/File/DownloadFile)|

#### cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="1" tabID="1" tabName1="Request" >}}
{{< tab tabNum="1" >}}

**Create Request Token**

```JAVA
curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=[]&client_secret=[]" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"
```

```JAVA
curl  -v -X GET "https://api.aspose.cloud/v4.0/words/storage/file/sample.docx" -H "Content-Type: application/json" -H "Authorization: Bearer 

[Access Token]
```

{{< /tab >}}
{{< /tabs >}}
### Uploading a file from Cloud Storage

#### API Information

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/{path}|PUT|Upload a file to Cloud Storage|[UploadFile](https://apireference.aspose.cloud/words/#/File/UploadFile)|

#### cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

**Create Request Token**

```JAVA
curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=[]&client_secret=[]" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"
```

```JAVA
curl  -v -X PUT "https://api.aspose.cloud/v4.0/words/storage/file/sample.docx" -H "Content-Type:application/octet-stream" -H "Authorization: Bearer [Access Token]
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
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
### Copying a file to a new location on Cloud Storage

#### API Information

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/copy/{srcPath}|PUT|Duplicate a file to a new location on Cloud Storage|[CopyFile](https://apireference.aspose.cloud/words/#/File/CopyFile)|

#### cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="1" tabID="8" tabName1="Request" >}}
{{< tab tabNum="1" >}}

**Create Request Token**

```JAVA
curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=[]&client_secret=[]" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"
```

```JAVA
curl -v -X PUT "https://api.aspose.cloud/v4.0/words/storage/file/copy/sample.docx/%2F?destPath=MyFolder" -H "Content-Type:application/json" -H "Authorization: Bearer [Access Token]
```

{{< /tab >}}
{{< /tabs >}}
### Moving a file to a new location on Cloud Storage

#### API Information

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/MOVE/{srcPath}|PUT|Move a file to a new location on Cloud Storage|[MoveFile](https://apireference.aspose.cloud/words/#/File/MoveFile)|

#### cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="1" tabID="11" tabName1="Request" >}}
{{< tab tabNum="1" >}}

**Create Request Token**

```JAVA
curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=[]&client_secret=[]" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"
```

```JAVA
curl -v -X PUT "https://api.aspose.cloud/v4.0/words/storage/file/move/input.docx/%2F?destPath=MyFolder" -H "Content-Type:application/json" -H "Authorization: Bearer [Access Token]
```

{{< /tab >}}
{{< /tabs >}}
### Deleting a file on Cloud Storage

#### API Information

|API|Type|Description|Swagger Link|
| :- | :- | :- | :- |
|/words/storage/file/{path}|DELETE|Delete a file from Cloud Storage|[DeleteFile](https://apireference.aspose.cloud/words/#/File/DeleteFile)|

#### cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="1" tabID="14" tabName1="Request" >}}
{{< tab tabNum="1" >}}

**Create Request Token**

```JAVA
curl -v "https://api.aspose.cloud/connect/token" -X POST -d "grant_type=client_credentials&client_id=[]&client_secret=[]" -H "Content-Type: application/x-www-form-urlencoded" -H "Accept: application/json"
```

```JAVA
curl -v -X DELETE "https://api.aspose.cloud/v4.0/words/storage/file/input.docx" -H "Content-Type:application/json" -H "Authorization: Bearer [Access Token]
```

{{< /tab >}}
{{< /tabs >}}
