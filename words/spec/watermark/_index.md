---
title: "Watermark"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/watermark/
description: "Watermark"
notoc: true
weight: 500
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Delete</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletewatermarkonlinerequest">DeleteWatermarkOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#deletewatermarkonlineresponse">DeleteWatermarkOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletewatermarkrequest">DeleteWatermarkRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertwatermarkimageonlinerequest">InsertWatermarkImageOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#insertwatermarkimageonlineresponse">InsertWatermarkImageOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertwatermarkimagerequest">InsertWatermarkImageRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertwatermarktextonlinerequest">InsertWatermarkTextOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertwatermarktextonlineresponse">InsertWatermarkTextOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#watermarktext">WatermarkText</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertwatermarktextrequest">InsertWatermarkTextRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></br><a href="#watermarktext">WatermarkText</a></td>
  </tr>
  </tbody>
</table>


## WatermarkText

Represents a class for insert watermark text request building.

This class is used in [InsertWatermarkTextOnlineRequest](#insertwatermarktextonlinerequest), [InsertWatermarkTextRequest](#insertwatermarktextrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RotationAngle        | <span style="color:SteelBlue;">double</span>  | Gets or sets the watermark rotation angle. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the watermark text. |


## DeleteWatermarkOnlineRequest

Represents a request model for [WordsApi.DeleteWatermarkOnline()](/words/watermark/delete/) operation.

An object of the **DeleteWatermarkOnlineRequest** class is created by the following constructor methods:

- DeleteWatermarkOnlineRequest()
- DeleteWatermarkOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteWatermarkOnlineResponse

Represents a response model for [WordsApi.DeleteWatermarkOnline()](/words/watermark/delete/) operation.

An object of the **DeleteWatermarkOnlineResponse** class is created by the following constructor methods:

- DeleteWatermarkOnlineResponse([DocumentResponse](/words/spec/document#documentresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DocumentResponse](/words/spec/document#documentresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## DeleteWatermarkRequest

Represents a request model for [WordsApi.DeleteWatermark()](/words/watermark/delete/) operation.

An object of the **DeleteWatermarkRequest** class is created by the following constructor methods:

- DeleteWatermarkRequest()
- DeleteWatermarkRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertWatermarkImageOnlineRequest

Represents a request model for [WordsApi.InsertWatermarkImageOnline()](/words/watermark/insert-image/) operation.

An object of the **InsertWatermarkImageOnlineRequest** class is created by the following constructor methods:

- InsertWatermarkImageOnlineRequest()
- InsertWatermarkImageOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">Stream</span> ***imageFile***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">double?</span> *rotationAngle*, <span style="color:SteelBlue;">string</span> *image*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***imageFile***      | ImageFile            | <span style="color:SteelBlue;">Stream</span>  | File with image. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *rotationAngle*      | RotationAngle        | <span style="color:SteelBlue;">double?</span> | The rotation angle of the watermark. |
| *image*              | Image                | <span style="color:SteelBlue;">string</span>  | The filename of the image. If the parameter value is missing — the image data is expected in the request content. |



## InsertWatermarkImageOnlineResponse

Represents a response model for [WordsApi.InsertWatermarkImageOnline()](/words/watermark/insert-image/) operation.

An object of the **InsertWatermarkImageOnlineResponse** class is created by the following constructor methods:

- InsertWatermarkImageOnlineResponse([DocumentResponse](/words/spec/document#documentresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DocumentResponse](/words/spec/document#documentresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertWatermarkImageRequest

Represents a request model for [WordsApi.InsertWatermarkImage()](/words/watermark/insert-image/) operation.

An object of the **InsertWatermarkImageRequest** class is created by the following constructor methods:

- InsertWatermarkImageRequest()
- InsertWatermarkImageRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">Stream</span> *imageFile*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">double?</span> *rotationAngle*, <span style="color:SteelBlue;">string</span> *image*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *imageFile*          | ImageFile            | <span style="color:SteelBlue;">Stream</span>  | File with image. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *rotationAngle*      | RotationAngle        | <span style="color:SteelBlue;">double?</span> | The rotation angle of the watermark. |
| *image*              | Image                | <span style="color:SteelBlue;">string</span>  | The filename of the image. If the parameter value is missing — the image data is expected in the request content. |



## InsertWatermarkTextOnlineRequest

Represents a request model for [WordsApi.InsertWatermarkTextOnline()](/words/watermark/insert-text/) operation.

An object of the **InsertWatermarkTextOnlineRequest** class is created by the following constructor methods:

- InsertWatermarkTextOnlineRequest()
- InsertWatermarkTextOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [WatermarkText](#watermarktext) ***watermarkText***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***watermarkText***  | WatermarkText        | [WatermarkText](#watermarktext)               | The watermark data. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertWatermarkTextOnlineResponse

Represents a response model for [WordsApi.InsertWatermarkTextOnline()](/words/watermark/insert-text/) operation.

An object of the **InsertWatermarkTextOnlineResponse** class is created by the following constructor methods:

- InsertWatermarkTextOnlineResponse([DocumentResponse](/words/spec/document#documentresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DocumentResponse](/words/spec/document#documentresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertWatermarkTextRequest

Represents a request model for [WordsApi.InsertWatermarkText()](/words/watermark/insert-text/) operation.

An object of the **InsertWatermarkTextRequest** class is created by the following constructor methods:

- InsertWatermarkTextRequest()
- InsertWatermarkTextRequest(<span style="color:SteelBlue;">string</span> ***name***, [WatermarkText](#watermarktext) ***watermarkText***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***watermarkText***  | WatermarkText        | [WatermarkText](#watermarktext)               | The watermark data. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |


