---
title: "CustomXmlPart"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/customxmlpart/
description: "CustomXmlPart"
notoc: true
weight: 140
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
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletecustomxmlpartonlinerequest">DeleteCustomXmlPartOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletecustomxmlpartrequest">DeleteCustomXmlPartRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletecustomxmlpartsonlinerequest">DeleteCustomXmlPartsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletecustomxmlpartsrequest">DeleteCustomXmlPartsRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getcustomxmlpartonlinerequest">GetCustomXmlPartOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#customxmlpartresponse">CustomXmlPartResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#customxmlpart">CustomXmlPart</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getcustomxmlpartrequest">GetCustomXmlPartRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getcustomxmlpartsonlinerequest">GetCustomXmlPartsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#customxmlpartsresponse">CustomXmlPartsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#customxmlpartscollection">CustomXmlPartsCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getcustomxmlpartsrequest">GetCustomXmlPartsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertcustomxmlpartonlinerequest">InsertCustomXmlPartOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertcustomxmlpartonlineresponse">InsertCustomXmlPartOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#customxmlpartinsert">CustomXmlPartInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertcustomxmlpartrequest">InsertCustomXmlPartRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#customxmlpartresponse">CustomXmlPartResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#customxmlpart">CustomXmlPart</a></br><a href="#customxmlpartinsert">CustomXmlPartInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatecustomxmlpartonlinerequest">UpdateCustomXmlPartOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatecustomxmlpartonlineresponse">UpdateCustomXmlPartOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#customxmlpartupdate">CustomXmlPartUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatecustomxmlpartrequest">UpdateCustomXmlPartRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#customxmlpartresponse">CustomXmlPartResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#customxmlpart">CustomXmlPart</a></br><a href="#customxmlpartupdate">CustomXmlPartUpdate</a></td>
  </tr>
  </tbody>
</table>


## CustomXmlPart

Represents a dTO container with a CustomXmlPart.

This class is inherited from [CustomXmlPartLink](#customxmlpartlink) and used in [CustomXmlPartResponse](#customxmlpartresponse), [CustomXmlPartsCollection](#customxmlpartscollection).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Data                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom xml part data. |
| Id                   | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom xml part id. |


## CustomXmlPartInsert

Represents a custom xml part insert.

This class is inherited from [CustomXmlPart](#customxmlpart) and used in [InsertCustomXmlPartOnlineRequest](#insertcustomxmlpartonlinerequest), [InsertCustomXmlPartRequest](#insertcustomxmlpartrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Data                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom xml part data. |
| Id                   | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom xml part id. |


## CustomXmlPartLink

Represents a customXmlPart link.

A single `Link` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |


## CustomXmlPartsCollection

Represents a collection of CustomXmlPart.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [CustomXmlPartsResponse](#customxmlpartsresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| CustomXmlPartsList   | List&lt;[CustomXmlPart](#customxmlpart)&gt;   | Gets or sets the collection of CustomXmlPart. |


## CustomXmlPartUpdate

Represents a custom xml part update.

This class is inherited from [CustomXmlPart](#customxmlpart) and used in [UpdateCustomXmlPartOnlineRequest](#updatecustomxmlpartonlinerequest), [UpdateCustomXmlPartRequest](#updatecustomxmlpartrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Data                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom xml part data. |
| Id                   | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom xml part id. |


## CustomXmlPartResponse

Represents a REST response with a custom xml part.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertCustomXmlPartOnlineResponse](#insertcustomxmlpartonlineresponse), [UpdateCustomXmlPartOnlineResponse](#updatecustomxmlpartonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| CustomXmlPart        | [CustomXmlPart](#customxmlpart)               | Gets or sets the custom xml part. |


## CustomXmlPartsResponse

Represents a REST response with a collection of custom xml parts.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| CustomXmlParts       | [CustomXmlPartsCollection](#customxmlpartscollection) | Gets or sets the collection of comments. |


## DeleteCustomXmlPartOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **DeleteCustomXmlPartOnlineRequest** class is created by the following constructor methods:

- DeleteCustomXmlPartOnlineRequest()
- DeleteCustomXmlPartOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***customXmlPartIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***customXmlPartIndex*** | CustomXmlPartIndex   | <span style="color:SteelBlue;">int</span>     | The index of the custom xml part. This index is the number of the entry in the collection of custom xml parts, not the ID of the part. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteCustomXmlPartRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **DeleteCustomXmlPartRequest** class is created by the following constructor methods:

- DeleteCustomXmlPartRequest()
- DeleteCustomXmlPartRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***customXmlPartIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***customXmlPartIndex*** | CustomXmlPartIndex   | <span style="color:SteelBlue;">int</span>     | The index of the custom xml part. This index is the number of the entry in the collection of custom xml parts, not the ID of the part. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteCustomXmlPartsOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **DeleteCustomXmlPartsOnlineRequest** class is created by the following constructor methods:

- DeleteCustomXmlPartsOnlineRequest()
- DeleteCustomXmlPartsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

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



## DeleteCustomXmlPartsRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **DeleteCustomXmlPartsRequest** class is created by the following constructor methods:

- DeleteCustomXmlPartsRequest()
- DeleteCustomXmlPartsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

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



## GetCustomXmlPartOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **GetCustomXmlPartOnlineRequest** class is created by the following constructor methods:

- GetCustomXmlPartOnlineRequest()
- GetCustomXmlPartOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***customXmlPartIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***customXmlPartIndex*** | CustomXmlPartIndex   | <span style="color:SteelBlue;">int</span>     | The index of the custom xml part. This index is the number of the entry in the collection of custom xml parts, not the ID of the part. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetCustomXmlPartRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **GetCustomXmlPartRequest** class is created by the following constructor methods:

- GetCustomXmlPartRequest()
- GetCustomXmlPartRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***customXmlPartIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***customXmlPartIndex*** | CustomXmlPartIndex   | <span style="color:SteelBlue;">int</span>     | The index of the custom xml part. This index is the number of the entry in the collection of custom xml parts, not the ID of the part. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetCustomXmlPartsOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **GetCustomXmlPartsOnlineRequest** class is created by the following constructor methods:

- GetCustomXmlPartsOnlineRequest()
- GetCustomXmlPartsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetCustomXmlPartsRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **GetCustomXmlPartsRequest** class is created by the following constructor methods:

- GetCustomXmlPartsRequest()
- GetCustomXmlPartsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## InsertCustomXmlPartOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **InsertCustomXmlPartOnlineRequest** class is created by the following constructor methods:

- InsertCustomXmlPartOnlineRequest()
- InsertCustomXmlPartOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [CustomXmlPartInsert](#customxmlpartinsert) ***customXmlPart***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***customXmlPart***  | CustomXmlPart        | [CustomXmlPartInsert](#customxmlpartinsert)   | Custom xml part. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertCustomXmlPartOnlineResponse

Represents a response model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **InsertCustomXmlPartOnlineResponse** class is created by the following constructor methods:

- InsertCustomXmlPartOnlineResponse([CustomXmlPartResponse](#customxmlpartresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [CustomXmlPartResponse](#customxmlpartresponse) | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## InsertCustomXmlPartRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **InsertCustomXmlPartRequest** class is created by the following constructor methods:

- InsertCustomXmlPartRequest()
- InsertCustomXmlPartRequest(<span style="color:SteelBlue;">string</span> ***name***, [CustomXmlPartInsert](#customxmlpartinsert) ***customXmlPart***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***customXmlPart***  | CustomXmlPart        | [CustomXmlPartInsert](#customxmlpartinsert)   | Custom xml part. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateCustomXmlPartOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **UpdateCustomXmlPartOnlineRequest** class is created by the following constructor methods:

- UpdateCustomXmlPartOnlineRequest()
- UpdateCustomXmlPartOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***customXmlPartIndex***, [CustomXmlPartUpdate](#customxmlpartupdate) ***customXmlPart***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***customXmlPartIndex*** | CustomXmlPartIndex   | <span style="color:SteelBlue;">int</span>     | The index of the custom xml part. This index is the number of the entry in the collection of custom xml parts, not the ID of the part. |
| ***customXmlPart***  | CustomXmlPart        | [CustomXmlPartUpdate](#customxmlpartupdate)   | Custom xml part. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateCustomXmlPartOnlineResponse

Represents a response model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **UpdateCustomXmlPartOnlineResponse** class is created by the following constructor methods:

- UpdateCustomXmlPartOnlineResponse([CustomXmlPartResponse](#customxmlpartresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [CustomXmlPartResponse](#customxmlpartresponse) | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## UpdateCustomXmlPartRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **UpdateCustomXmlPartRequest** class is created by the following constructor methods:

- UpdateCustomXmlPartRequest()
- UpdateCustomXmlPartRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***customXmlPartIndex***, [CustomXmlPartUpdate](#customxmlpartupdate) ***customXmlPart***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***customXmlPartIndex*** | CustomXmlPartIndex   | <span style="color:SteelBlue;">int</span>     | The index of the custom xml part. This index is the number of the entry in the collection of custom xml parts, not the ID of the part. |
| ***customXmlPart***  | CustomXmlPart        | [CustomXmlPartUpdate](#customxmlpartupdate)   | Custom xml part. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |


