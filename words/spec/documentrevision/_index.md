---
title: "DocumentRevision"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/documentrevision/
description: "DocumentRevision"
notoc: true
weight: 190
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>AcceptAll</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#acceptallrevisionsonlinerequest">AcceptAllRevisionsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#acceptallrevisionsonlineresponse">AcceptAllRevisionsOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#acceptallrevisionsrequest">AcceptAllRevisionsRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#revisionsmodificationresponse">RevisionsModificationResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#modificationoperationresult">ModificationOperationResult</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>RejectAll</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#rejectallrevisionsonlinerequest">RejectAllRevisionsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#rejectallrevisionsonlineresponse">RejectAllRevisionsOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#rejectallrevisionsrequest">RejectAllRevisionsRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#revisionsmodificationresponse">RevisionsModificationResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#modificationoperationresult">ModificationOperationResult</a></td>
  </tr>
  </tbody>
</table>


## ModificationOperationResult

Represents a result of the operation which modifies the original document and saves the result.

This class is used in [RevisionsModificationResponse](#revisionsmodificationresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Dest                 | [FileLink](/words/spec/link#filelink)         | Gets or sets the link to the dest document (result of the modification operation) . |
| Source               | [FileLink](/words/spec/link#filelink)         | Gets or sets the link to the source document (source for the modification operation) . |


## AcceptAllRevisionsOnlineRequest

Represents a request model for [WordsApi.AcceptAllRevisionsOnline()](/words/documents/track-changes/accept-all/) operation.

An object of the **AcceptAllRevisionsOnlineRequest** class is created by the following constructor methods:

- AcceptAllRevisionsOnlineRequest()
- AcceptAllRevisionsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## AcceptAllRevisionsOnlineResponse

Represents a response model for [WordsApi.AcceptAllRevisionsOnline()](/words/documents/track-changes/accept-all/) operation.

An object of the **AcceptAllRevisionsOnlineResponse** class is created by the following constructor methods:

- AcceptAllRevisionsOnlineResponse([RevisionsModificationResponse](#revisionsmodificationresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [RevisionsModificationResponse](#revisionsmodificationresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## AcceptAllRevisionsRequest

Represents a request model for [WordsApi.AcceptAllRevisions()](/words/documents/track-changes/accept-all/) operation.

An object of the **AcceptAllRevisionsRequest** class is created by the following constructor methods:

- AcceptAllRevisionsRequest()
- AcceptAllRevisionsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

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



## RejectAllRevisionsOnlineRequest

Represents a request model for [WordsApi.RejectAllRevisionsOnline()](/words/documents/track-changes/reject-all/) operation.

An object of the **RejectAllRevisionsOnlineRequest** class is created by the following constructor methods:

- RejectAllRevisionsOnlineRequest()
- RejectAllRevisionsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## RejectAllRevisionsOnlineResponse

Represents a response model for [WordsApi.RejectAllRevisionsOnline()](/words/documents/track-changes/reject-all/) operation.

An object of the **RejectAllRevisionsOnlineResponse** class is created by the following constructor methods:

- RejectAllRevisionsOnlineResponse([RevisionsModificationResponse](#revisionsmodificationresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [RevisionsModificationResponse](#revisionsmodificationresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## RejectAllRevisionsRequest

Represents a request model for [WordsApi.RejectAllRevisions()](/words/documents/track-changes/reject-all/) operation.

An object of the **RejectAllRevisionsRequest** class is created by the following constructor methods:

- RejectAllRevisionsRequest()
- RejectAllRevisionsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

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



## RevisionsModificationResponse

Represents a REST response with a result of the modification operations for the revisions collection (now these are acceptAll and rejectAll) .

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [AcceptAllRevisionsOnlineResponse](#acceptallrevisionsonlineresponse), [RejectAllRevisionsOnlineResponse](#rejectallrevisionsonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Result               | [ModificationOperationResult](#modificationoperationresult) | Gets or sets the result of the modification operations for the revisions collection. |

