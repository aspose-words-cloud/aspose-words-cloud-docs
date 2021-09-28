---
title: "File"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/file/
description: "File"
notoc: true
weight: 230
---


<table>
  <thead>
    <tr>
      <th style="text-align:center;"></th>
      <th><i>Request</i></th>
      <th><i>Response</i></th>
      <th><i>Model</i></th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Copy</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#copyfilerequest">CopyFileRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="5" colspan="2"><span style="color:SteelBlue;">void</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="6"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#copyfolderrequest">CopyFolderRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><strong><i>Create</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#createfolderrequest">CreateFolderRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Delete</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletefilerequest">DeleteFileRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletefolderrequest">DeleteFolderRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><strong><i>Download</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#downloadfilerequest">DownloadFileRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Stream</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getfileslistrequest">GetFilesListRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#fileslist">FilesList</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#storagefile">StorageFile</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Move</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#movefilerequest">MoveFileRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2" colspan="2"><span style="color:SteelBlue;">void</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#movefolderrequest">MoveFolderRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><strong><i>Upload</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#uploadfilerequest">UploadFileRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#filesuploadresult">FilesUploadResult</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#error">Error</a></td>
  </tr>
  </tbody>
</table>


## Error

Represents a error.

This class is used in [FilesUploadResult](#filesuploadresult).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Code                 | <span style="color:SteelBlue;">string</span>  | Code. |
| Description          | <span style="color:SteelBlue;">string</span>  | Description. |
| InnerError           | [ErrorDetails](#errordetails)                 | Inner Error. |
| Message              | <span style="color:SteelBlue;">string</span>  | Message. |


## ErrorDetails

Represents a error details.

This class is used in [Error](#error).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ErrorDateTime        | <span style="color:SteelBlue;">DateTime</span> | Error datetime. |
| RequestId            | <span style="color:SteelBlue;">string</span>  | The request id. |


## FilesList

Represents a files list.

This class is used in [WordsApi](/words/spec/wordsapi#wordsapi).

A single `Value` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Value                | List&lt;[StorageFile](#storagefile)&gt;       | Files and folders contained by folder StorageFile. |


## FilesUploadResult

Represents a file upload result.

This class is used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Errors               | List&lt;[Error](#error)&gt;                   | List of errors. |
| Uploaded             | List&lt;<span style="color:SteelBlue;">string</span>&gt; | List of uploaded file names. |


## StorageFile

Represents a file or folder information.

This class is used in [FilesList](#fileslist).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| IsFolder             | <span style="color:SteelBlue;">bool</span>    | True if it is a folder. |
| ModifiedDate         | <span style="color:SteelBlue;">DateTime</span> | File or folder last modified DateTime. |
| Name                 | <span style="color:SteelBlue;">string</span>  | File or folder name. |
| Path                 | <span style="color:SteelBlue;">string</span>  | File or folder path. |
| Size                 | <span style="color:SteelBlue;">int</span>     | File or folder size. |


## CopyFileRequest

Represents a request model for [WordsApi.CopyFile()](/words/files-and-storage/) operation.

An object of the **CopyFileRequest** class is created by the following constructor methods:

- CopyFileRequest()
- CopyFileRequest(<span style="color:SteelBlue;">string</span> ***destPath***, <span style="color:SteelBlue;">string</span> ***srcPath***, <span style="color:SteelBlue;">string</span> *srcStorageName*, <span style="color:SteelBlue;">string</span> *destStorageName*, <span style="color:SteelBlue;">string</span> *versionId*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***destPath***       | DestPath             | <span style="color:SteelBlue;">string</span>  | Destination file path. |
| ***srcPath***        | SrcPath              | <span style="color:SteelBlue;">string</span>  | Source file's path e.g. '/Folder 1/file.ext' or '/Bucket/Folder 1/file.ext'. |
| *srcStorageName*     | SrcStorageName       | <span style="color:SteelBlue;">string</span>  | Source storage name. |
| *destStorageName*    | DestStorageName      | <span style="color:SteelBlue;">string</span>  | Destination storage name. |
| *versionId*          | VersionId            | <span style="color:SteelBlue;">string</span>  | File version ID to copy. |



## CopyFolderRequest

Represents a request model for [WordsApi.CopyFolder()](/words/files-and-storage/) operation.

An object of the **CopyFolderRequest** class is created by the following constructor methods:

- CopyFolderRequest()
- CopyFolderRequest(<span style="color:SteelBlue;">string</span> ***destPath***, <span style="color:SteelBlue;">string</span> ***srcPath***, <span style="color:SteelBlue;">string</span> *srcStorageName*, <span style="color:SteelBlue;">string</span> *destStorageName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***destPath***       | DestPath             | <span style="color:SteelBlue;">string</span>  | Destination folder path e.g. '/dst'. |
| ***srcPath***        | SrcPath              | <span style="color:SteelBlue;">string</span>  | Source folder path e.g. /Folder1. |
| *srcStorageName*     | SrcStorageName       | <span style="color:SteelBlue;">string</span>  | Source storage name. |
| *destStorageName*    | DestStorageName      | <span style="color:SteelBlue;">string</span>  | Destination storage name. |



## CreateFolderRequest

Represents a request model for [WordsApi.CreateFolder()](/words/files-and-storage/) operation.

An object of the **CreateFolderRequest** class is created by the following constructor methods:

- CreateFolderRequest()
- CreateFolderRequest(<span style="color:SteelBlue;">string</span> ***path***, <span style="color:SteelBlue;">string</span> *storageName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***path***           | Path                 | <span style="color:SteelBlue;">string</span>  | Target folder's path e.g. Folder1/Folder2/. The folders will be created recursively. |
| *storageName*        | StorageName          | <span style="color:SteelBlue;">string</span>  | Storage name. |



## DeleteFileRequest

Represents a request model for [WordsApi.DeleteFile()](/words/files-and-storage/) operation.

An object of the **DeleteFileRequest** class is created by the following constructor methods:

- DeleteFileRequest()
- DeleteFileRequest(<span style="color:SteelBlue;">string</span> ***path***, <span style="color:SteelBlue;">string</span> *storageName*, <span style="color:SteelBlue;">string</span> *versionId*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***path***           | Path                 | <span style="color:SteelBlue;">string</span>  | Path of the file including the file name and extension e.g. /folder1/file.ext. |
| *storageName*        | StorageName          | <span style="color:SteelBlue;">string</span>  | Storage name. |
| *versionId*          | VersionId            | <span style="color:SteelBlue;">string</span>  | File version ID to delete. |



## DeleteFolderRequest

Represents a request model for [WordsApi.DeleteFolder()](/words/files-and-storage/) operation.

An object of the **DeleteFolderRequest** class is created by the following constructor methods:

- DeleteFolderRequest()
- DeleteFolderRequest(<span style="color:SteelBlue;">string</span> ***path***, <span style="color:SteelBlue;">string</span> *storageName*, <span style="color:SteelBlue;">bool?</span> *recursive*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***path***           | Path                 | <span style="color:SteelBlue;">string</span>  | Folder path e.g. '/folder'. |
| *storageName*        | StorageName          | <span style="color:SteelBlue;">string</span>  | Storage name. |
| *recursive*          | Recursive            | <span style="color:SteelBlue;">bool?</span>   | Enable to delete folders, subfolders and files. |



## DownloadFileRequest

Represents a request model for [WordsApi.DownloadFile()](/words/files-and-storage/) operation.

An object of the **DownloadFileRequest** class is created by the following constructor methods:

- DownloadFileRequest()
- DownloadFileRequest(<span style="color:SteelBlue;">string</span> ***path***, <span style="color:SteelBlue;">string</span> *storageName*, <span style="color:SteelBlue;">string</span> *versionId*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***path***           | Path                 | <span style="color:SteelBlue;">string</span>  | Path of the file including the file name and extension e.g. /folder1/file.ext. |
| *storageName*        | StorageName          | <span style="color:SteelBlue;">string</span>  | Storage name. |
| *versionId*          | VersionId            | <span style="color:SteelBlue;">string</span>  | File version ID to download. |



## GetFilesListRequest

Represents a request model for [WordsApi.GetFilesList()](/words/files-and-storage/) operation.

An object of the **GetFilesListRequest** class is created by the following constructor methods:

- GetFilesListRequest()
- GetFilesListRequest(<span style="color:SteelBlue;">string</span> ***path***, <span style="color:SteelBlue;">string</span> *storageName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***path***           | Path                 | <span style="color:SteelBlue;">string</span>  | Folder path e.g. '/folder'. |
| *storageName*        | StorageName          | <span style="color:SteelBlue;">string</span>  | Storage name. |



## MoveFileRequest

Represents a request model for [WordsApi.MoveFile()](/words/files-and-storage/) operation.

An object of the **MoveFileRequest** class is created by the following constructor methods:

- MoveFileRequest()
- MoveFileRequest(<span style="color:SteelBlue;">string</span> ***destPath***, <span style="color:SteelBlue;">string</span> ***srcPath***, <span style="color:SteelBlue;">string</span> *srcStorageName*, <span style="color:SteelBlue;">string</span> *destStorageName*, <span style="color:SteelBlue;">string</span> *versionId*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***destPath***       | DestPath             | <span style="color:SteelBlue;">string</span>  | Destination file path e.g. '/dest.ext'. |
| ***srcPath***        | SrcPath              | <span style="color:SteelBlue;">string</span>  | Source file's path e.g. '/Folder 1/file.ext' or '/Bucket/Folder 1/file.ext'. |
| *srcStorageName*     | SrcStorageName       | <span style="color:SteelBlue;">string</span>  | Source storage name. |
| *destStorageName*    | DestStorageName      | <span style="color:SteelBlue;">string</span>  | Destination storage name. |
| *versionId*          | VersionId            | <span style="color:SteelBlue;">string</span>  | File version ID to move. |



## MoveFolderRequest

Represents a request model for [WordsApi.MoveFolder()](/words/files-and-storage/) operation.

An object of the **MoveFolderRequest** class is created by the following constructor methods:

- MoveFolderRequest()
- MoveFolderRequest(<span style="color:SteelBlue;">string</span> ***destPath***, <span style="color:SteelBlue;">string</span> ***srcPath***, <span style="color:SteelBlue;">string</span> *srcStorageName*, <span style="color:SteelBlue;">string</span> *destStorageName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***destPath***       | DestPath             | <span style="color:SteelBlue;">string</span>  | Destination folder path to move to e.g '/dst'. |
| ***srcPath***        | SrcPath              | <span style="color:SteelBlue;">string</span>  | Source folder path e.g. /Folder1. |
| *srcStorageName*     | SrcStorageName       | <span style="color:SteelBlue;">string</span>  | Source storage name. |
| *destStorageName*    | DestStorageName      | <span style="color:SteelBlue;">string</span>  | Destination storage name. |



## UploadFileRequest

Represents a request model for [WordsApi.UploadFile()](/words/files-and-storage/) operation.

An object of the **UploadFileRequest** class is created by the following constructor methods:

- UploadFileRequest()
- UploadFileRequest(<span style="color:SteelBlue;">Stream</span> ***fileContent***, <span style="color:SteelBlue;">string</span> ***path***, <span style="color:SteelBlue;">string</span> *storageName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***fileContent***    | FileContent          | <span style="color:SteelBlue;">Stream</span>  | File to upload. |
| ***path***           | Path                 | <span style="color:SteelBlue;">string</span>  | Path where to upload including filename and extension e.g. /file.ext or /Folder 1/file.ext If the content is multipart and path does not contains the file name it tries to get them from filename parameter from Content-Disposition header. |
| *storageName*        | StorageName          | <span style="color:SteelBlue;">string</span>  | Storage name. |


