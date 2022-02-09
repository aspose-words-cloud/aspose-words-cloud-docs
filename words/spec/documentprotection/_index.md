---
title: "DocumentProtection"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/documentprotection/
description: "DocumentProtection"
notoc: true
weight: 180
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="5"><strong><i>Protect</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentprotectiononlinerequest">GetDocumentProtectionOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#protectiondataresponse">ProtectionDataResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="/words/spec/link#filelink">FileLink</a></br><a href="#protectiondata">ProtectionData</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentprotectionrequest">GetDocumentProtectionRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#protectdocumentonlinerequest">ProtectDocumentOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#protectdocumentonlineresponse">ProtectDocumentOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#protectdocumentrequest">ProtectDocumentRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#protectiondataresponse">ProtectionDataResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/link#filelink">FileLink</a></br><a href="#protectiondata">ProtectionData</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#protectionrequest">ProtectionRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Unprotect</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#unprotectdocumentonlinerequest">UnprotectDocumentOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#unprotectdocumentonlineresponse">UnprotectDocumentOnlineResponse</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#unprotectdocumentrequest">UnprotectDocumentRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#protectiondataresponse">ProtectionDataResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/link#filelink">FileLink</a></br><a href="#protectiondata">ProtectionData</a></td>
  </tr>
  </tbody>
</table>


## ProtectionData

Represents a container for the data about protection of the document.

This class is used in [ProtectionDataResponse](#protectiondataresponse).

A single `ProtectionType` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ProtectionType       | <span style="color:SteelBlue;">string</span>  | Gets or sets type of the protection. |


## GetDocumentProtectionOnlineRequest

Represents a request model for [WordsApi.GetDocumentProtectionOnline()](/words/documents/protection/get/) operation.

An object of the **GetDocumentProtectionOnlineRequest** class is created by the following constructor methods:

- GetDocumentProtectionOnlineRequest()
- GetDocumentProtectionOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentProtectionRequest

Represents a request model for [WordsApi.GetDocumentProtection()](/words/documents/protection/get/) operation.

An object of the **GetDocumentProtectionRequest** class is created by the following constructor methods:

- GetDocumentProtectionRequest()
- GetDocumentProtectionRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## ProtectDocumentOnlineRequest

Represents a request model for [WordsApi.ProtectDocumentOnline()](/words/documents/protection/add/) operation.

An object of the **ProtectDocumentOnlineRequest** class is created by the following constructor methods:

- ProtectDocumentOnlineRequest()
- ProtectDocumentOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [ProtectionRequest](#protectionrequest) ***protectionRequest***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***protectionRequest*** | ProtectionRequest    | [ProtectionRequest](#protectionrequest)       | Protection request. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## ProtectDocumentOnlineResponse

Represents a response model for [WordsApi.ProtectDocumentOnline()](/words/documents/protection/add/) operation.

An object of the **ProtectDocumentOnlineResponse** class is created by the following constructor methods:

- ProtectDocumentOnlineResponse([ProtectionDataResponse](#protectiondataresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [ProtectionDataResponse](#protectiondataresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## ProtectDocumentRequest

Represents a request model for [WordsApi.ProtectDocument()](/words/documents/protection/add/) operation.

An object of the **ProtectDocumentRequest** class is created by the following constructor methods:

- ProtectDocumentRequest()
- ProtectDocumentRequest(<span style="color:SteelBlue;">string</span> ***name***, [ProtectionRequest](#protectionrequest) ***protectionRequest***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***protectionRequest*** | ProtectionRequest    | [ProtectionRequest](#protectionrequest)       | Protection request. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## ProtectionDataResponse

Represents a REST response with data on document's protection.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [ProtectDocumentOnlineResponse](#protectdocumentonlineresponse), [UnprotectDocumentOnlineResponse](#unprotectdocumentonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| DocumentLink         | [FileLink](/words/spec/link#filelink)         | Gets or sets the link to the document. |
| ProtectionData       | [ProtectionData](#protectiondata)             | Gets or sets the protection properties of the document. |


## ProtectionRequest

Represents a request on changing of protection.

This class is used in [ProtectDocumentOnlineRequest](#protectdocumentonlinerequest), [ProtectDocumentRequest](#protectdocumentrequest), [UnprotectDocumentOnlineRequest](#unprotectdocumentonlinerequest), [UnprotectDocumentRequest](#unprotectdocumentrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| NewPassword          | <span style="color:SteelBlue;">string</span>  | Gets or sets the new password. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the current password. |
| ProtectionType       | <span style="color:SteelBlue;">string</span>  | Gets or sets the new type of protection. |


## UnprotectDocumentOnlineRequest

Represents a request model for [WordsApi.UnprotectDocumentOnline()](/words/documents/protection/remove/) operation.

An object of the **UnprotectDocumentOnlineRequest** class is created by the following constructor methods:

- UnprotectDocumentOnlineRequest()
- UnprotectDocumentOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [ProtectionRequest](#protectionrequest) ***protectionRequest***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***protectionRequest*** | ProtectionRequest    | [ProtectionRequest](#protectionrequest)       | Protection request. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## UnprotectDocumentOnlineResponse

Represents a response model for [WordsApi.UnprotectDocumentOnline()](/words/documents/protection/remove/) operation.

An object of the **UnprotectDocumentOnlineResponse** class is created by the following constructor methods:

- UnprotectDocumentOnlineResponse([ProtectionDataResponse](#protectiondataresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [ProtectionDataResponse](#protectiondataresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UnprotectDocumentRequest

Represents a request model for [WordsApi.UnprotectDocument()](/words/documents/protection/remove/) operation.

An object of the **UnprotectDocumentRequest** class is created by the following constructor methods:

- UnprotectDocumentRequest()
- UnprotectDocumentRequest(<span style="color:SteelBlue;">string</span> ***name***, [ProtectionRequest](#protectionrequest) ***protectionRequest***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***protectionRequest*** | ProtectionRequest    | [ProtectionRequest](#protectionrequest)       | Protection request. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |


