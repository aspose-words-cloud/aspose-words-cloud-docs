---
title: "DocumentProperties"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/documentproperties/
description: "DocumentProperties"
notoc: true
weight: 170
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>CreateOrUpdate</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#createorupdatedocumentpropertyonlinerequest">CreateOrUpdateDocumentPropertyOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#createorupdatedocumentpropertyonlineresponse">CreateOrUpdateDocumentPropertyOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#documentpropertycreateorupdate">DocumentPropertyCreateOrUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#createorupdatedocumentpropertyrequest">CreateOrUpdateDocumentPropertyRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#documentpropertyresponse">DocumentPropertyResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#documentproperty">DocumentProperty</a></br><a href="#documentpropertycreateorupdate">DocumentPropertyCreateOrUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Delete</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletedocumentpropertyonlinerequest">DeleteDocumentPropertyOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletedocumentpropertyrequest">DeleteDocumentPropertyRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentpropertiesonlinerequest">GetDocumentPropertiesOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#documentpropertiesresponse">DocumentPropertiesResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#documentproperties">DocumentProperties</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentpropertiesrequest">GetDocumentPropertiesRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentpropertyonlinerequest">GetDocumentPropertyOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#documentpropertyresponse">DocumentPropertyResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#documentproperty">DocumentProperty</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentpropertyrequest">GetDocumentPropertyRequest</a></td>
  </tr>
  </tbody>
</table>


## DocumentProperties

Represents a collection of document properties.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [Document](/words/spec/document#document), [DocumentPropertiesResponse](#documentpropertiesresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| List                 | List&lt;[DocumentProperty](#documentproperty)&gt; | Gets or sets the collection of document properties. |


## DocumentPropertyBase

Represents a words document property DTO base class.

A single `Value` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Value                | <span style="color:SteelBlue;">string</span>  | Gets or sets the value of the document property. |


## DocumentProperty

Represents a words document property DTO.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [DocumentProperties](#documentproperties), [DocumentPropertyResponse](#documentpropertyresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| BuiltIn              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the property is built-in or not. If true the property is built-in, if false the property is custom. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the document property. |
| Value                | <span style="color:SteelBlue;">string</span>  | Gets or sets the value of the document property. |


## DocumentPropertyCreateOrUpdate

Represents a words document property DTO for create or update.

This class is inherited from [DocumentPropertyBase](#documentpropertybase) and used in [CreateOrUpdateDocumentPropertyOnlineRequest](#createorupdatedocumentpropertyonlinerequest), [CreateOrUpdateDocumentPropertyRequest](#createorupdatedocumentpropertyrequest).

A single `Value` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Value                | <span style="color:SteelBlue;">string</span>  | Gets or sets the value of the document property. |


## DocumentPropertiesResponse

Represents a REST response with a collection of document properties.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| DocumentProperties   | [DocumentProperties](#documentproperties)     | Gets or sets the collection of document properties. |


## CreateOrUpdateDocumentPropertyOnlineRequest

Represents a request model for [WordsApi.CreateOrUpdateDocumentPropertyOnline()](/words/documents/properties/add-or-update/) operation.

An object of the **CreateOrUpdateDocumentPropertyOnlineRequest** class is created by the following constructor methods:

- CreateOrUpdateDocumentPropertyOnlineRequest()
- CreateOrUpdateDocumentPropertyOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***propertyName***, [DocumentPropertyCreateOrUpdate](#documentpropertycreateorupdate) ***property***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***propertyName***   | PropertyName         | <span style="color:SteelBlue;">string</span>  | The name of the property. |
| ***property***       | Property             | [DocumentPropertyCreateOrUpdate](#documentpropertycreateorupdate) | The property with new value. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## CreateOrUpdateDocumentPropertyOnlineResponse

Represents a response model for [WordsApi.CreateOrUpdateDocumentPropertyOnline()](/words/documents/properties/add-or-update/) operation.

An object of the **CreateOrUpdateDocumentPropertyOnlineResponse** class is created by the following constructor methods:

- CreateOrUpdateDocumentPropertyOnlineResponse([DocumentPropertyResponse](#documentpropertyresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DocumentPropertyResponse](#documentpropertyresponse) | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## CreateOrUpdateDocumentPropertyRequest

Represents a request model for [WordsApi.CreateOrUpdateDocumentProperty()](/words/documents/properties/add-or-update/) operation.

An object of the **CreateOrUpdateDocumentPropertyRequest** class is created by the following constructor methods:

- CreateOrUpdateDocumentPropertyRequest()
- CreateOrUpdateDocumentPropertyRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***propertyName***, [DocumentPropertyCreateOrUpdate](#documentpropertycreateorupdate) ***property***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***propertyName***   | PropertyName         | <span style="color:SteelBlue;">string</span>  | The name of the property. |
| ***property***       | Property             | [DocumentPropertyCreateOrUpdate](#documentpropertycreateorupdate) | The property with new value. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteDocumentPropertyOnlineRequest

Represents a request model for [WordsApi.DeleteDocumentPropertyOnline()](/words/documents/properties/delete/) operation.

An object of the **DeleteDocumentPropertyOnlineRequest** class is created by the following constructor methods:

- DeleteDocumentPropertyOnlineRequest()
- DeleteDocumentPropertyOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***propertyName***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***propertyName***   | PropertyName         | <span style="color:SteelBlue;">string</span>  | The name of the property. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteDocumentPropertyRequest

Represents a request model for [WordsApi.DeleteDocumentProperty()](/words/documents/properties/delete/) operation.

An object of the **DeleteDocumentPropertyRequest** class is created by the following constructor methods:

- DeleteDocumentPropertyRequest()
- DeleteDocumentPropertyRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***propertyName***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***propertyName***   | PropertyName         | <span style="color:SteelBlue;">string</span>  | The name of the property. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DocumentPropertyResponse

Represents a REST response with a document property.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [CreateOrUpdateDocumentPropertyOnlineResponse](#createorupdatedocumentpropertyonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| DocumentProperty     | [DocumentProperty](#documentproperty)         | Gets or sets the document property. |


## GetDocumentPropertiesOnlineRequest

Represents a request model for [WordsApi.GetDocumentPropertiesOnline()](/words/documents/properties/get-all/) operation.

An object of the **GetDocumentPropertiesOnlineRequest** class is created by the following constructor methods:

- GetDocumentPropertiesOnlineRequest()
- GetDocumentPropertiesOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentPropertiesRequest

Represents a request model for [WordsApi.GetDocumentProperties()](/words/documents/properties/get-all/) operation.

An object of the **GetDocumentPropertiesRequest** class is created by the following constructor methods:

- GetDocumentPropertiesRequest()
- GetDocumentPropertiesRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentPropertyOnlineRequest

Represents a request model for [WordsApi.GetDocumentPropertyOnline()](/words/documents/properties/get/) operation.

An object of the **GetDocumentPropertyOnlineRequest** class is created by the following constructor methods:

- GetDocumentPropertyOnlineRequest()
- GetDocumentPropertyOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***propertyName***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***propertyName***   | PropertyName         | <span style="color:SteelBlue;">string</span>  | The name of the property. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentPropertyRequest

Represents a request model for [WordsApi.GetDocumentProperty()](/words/documents/properties/get/) operation.

An object of the **GetDocumentPropertyRequest** class is created by the following constructor methods:

- GetDocumentPropertyRequest()
- GetDocumentPropertyRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***propertyName***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***propertyName***   | PropertyName         | <span style="color:SteelBlue;">string</span>  | The name of the property. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |


