---
title: "Field"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/field/
description: "Field"
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Delete</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletefieldonlinerequest">DeleteFieldOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletefieldrequest">DeleteFieldRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletefieldsonlinerequest">DeleteFieldsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletefieldsrequest">DeleteFieldsRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="6"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentfieldnamesonlinerequest">GetDocumentFieldNamesOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#fieldnamesresponse">FieldNamesResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#fieldnames">FieldNames</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentfieldnamesrequest">GetDocumentFieldNamesRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getfieldonlinerequest">GetFieldOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#fieldresponse">FieldResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#field">Field</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getfieldrequest">GetFieldRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getfieldsonlinerequest">GetFieldsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#fieldsresponse">FieldsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#fieldcollection">FieldCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getfieldsrequest">GetFieldsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertfieldonlinerequest">InsertFieldOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertfieldonlineresponse">InsertFieldOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#fieldinsert">FieldInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertfieldrequest">InsertFieldRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#fieldresponse">FieldResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#field">Field</a></br><a href="#fieldinsert">FieldInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatefieldonlinerequest">UpdateFieldOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatefieldonlineresponse">UpdateFieldOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#fieldupdate">FieldUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatefieldrequest">UpdateFieldRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#fieldresponse">FieldResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#field">Field</a></br><a href="#fieldupdate">FieldUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatefieldsonlinerequest">UpdateFieldsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#updatefieldsonlineresponse">UpdateFieldsOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatefieldsrequest">UpdateFieldsRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></td>
  </tr>
  </tbody>
</table>


## Field

Represents a dTO container with a field.

This class is inherited from [FieldLink](#fieldlink) and used in [FieldCollection](#fieldcollection), [FieldResponse](#fieldresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| FieldCode            | <span style="color:SteelBlue;">string</span>  | Gets or sets the field code. |
| LocaleId             | <span style="color:SteelBlue;">string</span>  | Gets or sets the LCID of the field. |
| Result               | <span style="color:SteelBlue;">string</span>  | Gets or sets the field result. |


## FieldBase

Represents a field.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FieldCode            | <span style="color:SteelBlue;">string</span>  | Gets or sets the field code. |
| LocaleId             | <span style="color:SteelBlue;">string</span>  | Gets or sets the LCID of the field. |


## FieldCollection

Represents a dTO container with a collection of fields.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [FieldsResponse](#fieldsresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| List                 | List&lt;[Field](#field)&gt;                   | Gets or sets the collection of fields. |


## FieldInsert

Represents a field for insert.

This class is inherited from [FieldBase](#fieldbase) and used in [InsertFieldOnlineRequest](#insertfieldonlinerequest), [InsertFieldRequest](#insertfieldrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FieldCode            | <span style="color:SteelBlue;">string</span>  | Gets or sets the field code. |
| LocaleId             | <span style="color:SteelBlue;">string</span>  | Gets or sets the LCID of the field. |


## FieldLink

Represents a field link.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| FieldCode            | <span style="color:SteelBlue;">string</span>  | Gets or sets the field code. |


## FieldNames

Represents a collection of merge fields within a document.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [FieldNamesResponse](#fieldnamesresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Names                | List&lt;<span style="color:SteelBlue;">string</span>&gt; | Gets or sets the collection of fields names. |


## FieldUpdate

Represents a field for update.

This class is inherited from [FieldBase](#fieldbase) and used in [UpdateFieldOnlineRequest](#updatefieldonlinerequest), [UpdateFieldRequest](#updatefieldrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FieldCode            | <span style="color:SteelBlue;">string</span>  | Gets or sets the field code. |
| LocaleId             | <span style="color:SteelBlue;">string</span>  | Gets or sets the LCID of the field. |


## FieldNamesResponse

Represents a REST response with a collection of mail merge fields.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| FieldNames           | [FieldNames](#fieldnames)                     | Gets or sets the collection of mail merge fields. |


## DeleteFieldOnlineRequest

Represents a request model for [WordsApi.DeleteFieldOnline()](/words/fields/delete/) operation.

An object of the **DeleteFieldOnlineRequest** class is created by the following constructor methods:

- DeleteFieldOnlineRequest()
- DeleteFieldOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteFieldRequest

Represents a request model for [WordsApi.DeleteField()](/words/fields/delete/) operation.

An object of the **DeleteFieldRequest** class is created by the following constructor methods:

- DeleteFieldRequest()
- DeleteFieldRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteFieldsOnlineRequest

Represents a request model for [WordsApi.DeleteFieldsOnline()](/words/fields/remove/) operation.

An object of the **DeleteFieldsOnlineRequest** class is created by the following constructor methods:

- DeleteFieldsOnlineRequest()
- DeleteFieldsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteFieldsRequest

Represents a request model for [WordsApi.DeleteFields()](/words/fields/remove/) operation.

An object of the **DeleteFieldsRequest** class is created by the following constructor methods:

- DeleteFieldsRequest()
- DeleteFieldsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## FieldResponse

Represents a REST response with a field.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertFieldOnlineResponse](#insertfieldonlineresponse), [UpdateFieldOnlineResponse](#updatefieldonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Field                | [Field](#field)                               | Gets or sets the field. |


## FieldsResponse

Represents a REST response with a collection of fields.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Fields               | [FieldCollection](#fieldcollection)           | Gets or sets the collection of fields. |


## GetDocumentFieldNamesOnlineRequest

Represents a request model for [WordsApi.GetDocumentFieldNamesOnline()](/words/mail-merge/read-field-names-online/) operation.

An object of the **GetDocumentFieldNamesOnlineRequest** class is created by the following constructor methods:

- GetDocumentFieldNamesOnlineRequest()
- GetDocumentFieldNamesOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***template***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">bool?</span> *useNonMergeFields*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***template***       | Template             | <span style="color:SteelBlue;">Stream</span>  | The template document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *useNonMergeFields*  | UseNonMergeFields    | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to use non merge fields. If true, result includes "mustache" field names. |



## GetDocumentFieldNamesRequest

Represents a request model for [WordsApi.GetDocumentFieldNames()](/words/mail-merge/read-field-names-online/) operation.

An object of the **GetDocumentFieldNamesRequest** class is created by the following constructor methods:

- GetDocumentFieldNamesRequest()
- GetDocumentFieldNamesRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">bool?</span> *useNonMergeFields*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *useNonMergeFields*  | UseNonMergeFields    | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to use non merge fields. If true, result includes "mustache" field names. |



## GetFieldOnlineRequest

Represents a request model for [WordsApi.GetFieldOnline()](/words/fields/get/) operation.

An object of the **GetFieldOnlineRequest** class is created by the following constructor methods:

- GetFieldOnlineRequest()
- GetFieldOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetFieldRequest

Represents a request model for [WordsApi.GetField()](/words/fields/get/) operation.

An object of the **GetFieldRequest** class is created by the following constructor methods:

- GetFieldRequest()
- GetFieldRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetFieldsOnlineRequest

Represents a request model for [WordsApi.GetFieldsOnline()](/words/fields/get-all/) operation.

An object of the **GetFieldsOnlineRequest** class is created by the following constructor methods:

- GetFieldsOnlineRequest()
- GetFieldsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetFieldsRequest

Represents a request model for [WordsApi.GetFields()](/words/fields/get-all/) operation.

An object of the **GetFieldsRequest** class is created by the following constructor methods:

- GetFieldsRequest()
- GetFieldsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## InsertFieldOnlineRequest

Represents a request model for [WordsApi.InsertFieldOnline()](/words/fields/add/) operation.

An object of the **InsertFieldOnlineRequest** class is created by the following constructor methods:

- InsertFieldOnlineRequest()
- InsertFieldOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [FieldInsert](#fieldinsert) ***field***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">string</span> *insertBeforeNode*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***field***          | Field                | [FieldInsert](#fieldinsert)                   | Field data. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *insertBeforeNode*   | InsertBeforeNode     | <span style="color:SteelBlue;">string</span>  | The index of the node. A new field will be inserted before the node with the specified node Id. |



## InsertFieldOnlineResponse

Represents a response model for [WordsApi.InsertFieldOnline()](/words/fields/add/) operation.

An object of the **InsertFieldOnlineResponse** class is created by the following constructor methods:

- InsertFieldOnlineResponse([FieldResponse](#fieldresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [FieldResponse](#fieldresponse)               | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## InsertFieldRequest

Represents a request model for [WordsApi.InsertField()](/words/fields/add/) operation.

An object of the **InsertFieldRequest** class is created by the following constructor methods:

- InsertFieldRequest()
- InsertFieldRequest(<span style="color:SteelBlue;">string</span> ***name***, [FieldInsert](#fieldinsert) ***field***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">string</span> *insertBeforeNode*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***field***          | Field                | [FieldInsert](#fieldinsert)                   | Field data. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *insertBeforeNode*   | InsertBeforeNode     | <span style="color:SteelBlue;">string</span>  | The index of the node. A new field will be inserted before the node with the specified node Id. |



## UpdateFieldOnlineRequest

Represents a request model for [WordsApi.UpdateFieldOnline()](/words/fields/update-field-properties/) operation.

An object of the **UpdateFieldOnlineRequest** class is created by the following constructor methods:

- UpdateFieldOnlineRequest()
- UpdateFieldOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [FieldUpdate](#fieldupdate) ***field***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***field***          | Field                | [FieldUpdate](#fieldupdate)                   | Field data. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateFieldOnlineResponse

Represents a response model for [WordsApi.UpdateFieldOnline()](/words/fields/update-field-properties/) operation.

An object of the **UpdateFieldOnlineResponse** class is created by the following constructor methods:

- UpdateFieldOnlineResponse([FieldResponse](#fieldresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [FieldResponse](#fieldresponse)               | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## UpdateFieldRequest

Represents a request model for [WordsApi.UpdateField()](/words/fields/update-field-properties/) operation.

An object of the **UpdateFieldRequest** class is created by the following constructor methods:

- UpdateFieldRequest()
- UpdateFieldRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, [FieldUpdate](#fieldupdate) ***field***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***field***          | Field                | [FieldUpdate](#fieldupdate)                   | Field data. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateFieldsOnlineRequest

Represents a request model for [WordsApi.UpdateFieldsOnline()](/words/fields/update/) operation.

An object of the **UpdateFieldsOnlineRequest** class is created by the following constructor methods:

- UpdateFieldsOnlineRequest()
- UpdateFieldsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## UpdateFieldsOnlineResponse

Represents a response model for [WordsApi.UpdateFieldsOnline()](/words/fields/update/) operation.

An object of the **UpdateFieldsOnlineResponse** class is created by the following constructor methods:

- UpdateFieldsOnlineResponse([DocumentResponse](/words/spec/document#documentresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DocumentResponse](/words/spec/document#documentresponse) | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## UpdateFieldsRequest

Represents a request model for [WordsApi.UpdateFields()](/words/fields/update/) operation.

An object of the **UpdateFieldsRequest** class is created by the following constructor methods:

- UpdateFieldsRequest()
- UpdateFieldsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

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



## FieldOptions.FieldIndexFormatEnum

The following values are defined: Template, Classic, Fancy, Modern, Bulleted, Formal, Simple.


## FieldOptions.FieldUpdateCultureSourceEnum

The following values are defined: CurrentThread, FieldCode.

