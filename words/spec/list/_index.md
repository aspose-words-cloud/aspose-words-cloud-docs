---
title: "List"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/list/
description: "List"
notoc: true
weight: 310
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getlistonlinerequest">GetListOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#listresponse">ListResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#listinfo">ListInfo</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getlistrequest">GetListRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getlistsonlinerequest">GetListsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#listsresponse">ListsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#lists">Lists</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getlistsrequest">GetListsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertlistonlinerequest">InsertListOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertlistonlineresponse">InsertListOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listinsert">ListInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertlistrequest">InsertListRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listresponse">ListResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listinfo">ListInfo</a></br><a href="#listinsert">ListInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatelistlevelonlinerequest">UpdateListLevelOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatelistlevelonlineresponse">UpdateListLevelOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listlevelupdate">ListLevelUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatelistlevelrequest">UpdateListLevelRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listresponse">ListResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listinfo">ListInfo</a></br><a href="#listlevelupdate">ListLevelUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatelistonlinerequest">UpdateListOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatelistonlineresponse">UpdateListOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listupdate">ListUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatelistrequest">UpdateListRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listresponse">ListResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listinfo">ListInfo</a></br><a href="#listupdate">ListUpdate</a></td>
  </tr>
  </tbody>
</table>


## ListInfo

Represents a dTO container with a single document list.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [ListResponse](#listresponse), [Lists](#lists).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| IsListStyleDefinition | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this list is a definition of a list style. |
| IsListStyleReference | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this list is a reference to a list style. |
| IsMultiLevel         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the list contains 9 levels; false when 1 level. |
| IsRestartAtEachSection | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether list should be restarted at each section. The default value is false. |
| ListId               | <span style="color:SteelBlue;">int</span>     | Gets or sets the unique identifier of the list. |
| ListLevels           | [ListLevels](#listlevels)                     | Gets or sets the collection of list levels for this list. |
| Style                | [Style](/words/spec/style#style)              | Gets or sets the list style that this list references or defines. |


## ListInsert

Represents a insert document to document list.

This class is used in [InsertListOnlineRequest](#insertlistonlinerequest), [InsertListRequest](#insertlistrequest).

A single `Template` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Template             | [TemplateEnum](#listinsert.templateenum)      | Gets or sets the option that controls how list should be restarted at each section. |


## ListLevel

Represents a dTO container with a document list level.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [ListLevels](#listlevels).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Alignment            | [AlignmentEnum](#listlevel.alignmentenum)     | Gets or sets the justification of the actual number of the list item. |
| Font                 | [Font](/words/spec/font#font)                 | Gets or sets character formatting used for the list label. |
| IsLegal              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the level turns all inherited numbers to Arabic, false if it preserves their number style. |
| LinkedStyle          | [Style](/words/spec/style#style)              | Gets or sets the paragraph style that is linked to this list level. |
| NumberFormat         | <span style="color:SteelBlue;">string</span>  | Gets or sets the number format for the list level. |
| NumberPosition       | <span style="color:SteelBlue;">double</span>  | Gets or sets the position (in points) of the number or bullet for the list level. |
| NumberStyle          | [NumberStyleEnum](#listlevel.numberstyleenum) | Gets or sets the number style for this list level. |
| RestartAfterLevel    | <span style="color:SteelBlue;">int</span>     | Gets or sets the list level, that must appear before the specified list level restarts numbering. |
| StartAt              | <span style="color:SteelBlue;">int</span>     | Gets or sets the starting number for this list level. |
| TabPosition          | <span style="color:SteelBlue;">double</span>  | Gets or sets the tab position (in points) for the list level. |
| TextPosition         | <span style="color:SteelBlue;">double</span>  | Gets or sets the position (in points) for the second line of wrapping text for the list level. |
| TrailingCharacter    | [TrailingCharacterEnum](#listlevel.trailingcharacterenum) | Gets or sets the character inserted after the number for the list level. |


## ListLevels

Represents a dTO container with a single document list.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [ListInfo](#listinfo).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| ListLevel            | List&lt;[ListLevel](#listlevel)&gt;           | Gets or sets the collection of list levels for this list. |


## ListLevelUpdate

Represents a document list levels.

This class is used in [UpdateListLevelOnlineRequest](#updatelistlevelonlinerequest), [UpdateListLevelRequest](#updatelistlevelrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Alignment            | [AlignmentEnum](#listlevel.alignmentenum)     | Gets or sets the justification of the actual number of the list item. |
| IsLegal              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the level turns all inherited numbers to Arabic, false if it preserves their number style. |
| NumberFormat         | <span style="color:SteelBlue;">string</span>  | Gets or sets the number format for the list level. |
| NumberPosition       | <span style="color:SteelBlue;">double</span>  | Gets or sets the position (in points) of the number or bullet for the list level. |
| NumberStyle          | [NumberStyleEnum](#listlevel.numberstyleenum) | Gets or sets the number style for this list level. |
| RestartAfterLevel    | <span style="color:SteelBlue;">int</span>     | Gets or sets the list level that must appear before the specified list level restarts numbering. |
| StartAt              | <span style="color:SteelBlue;">int</span>     | Gets or sets the starting number for this list level. |
| TabPosition          | <span style="color:SteelBlue;">double</span>  | Gets or sets the tab position (in points) for the list level. |
| TextPosition         | <span style="color:SteelBlue;">double</span>  | Gets or sets the position (in points) for the second line of wrapping text for the list level. |
| TrailingCharacter    | [TrailingCharacterEnum](#listlevel.trailingcharacterenum) | Gets or sets the character to be inserted after the number for the list level. |


## Lists

Represents a dTO container with an array of document lists.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [ListsResponse](#listsresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| ListInfo             | List&lt;[ListInfo](#listinfo)&gt;             | Gets or sets the array of document lists. |


## ListUpdate

Represents a update document properties if document list.

This class is used in [UpdateListOnlineRequest](#updatelistonlinerequest), [UpdateListRequest](#updatelistrequest).

A single `IsRestartAtEachSection` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| IsRestartAtEachSection | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether list should be restarted at each section. The default value is false. |


## GetListOnlineRequest

Represents a request model for [WordsApi.GetListOnline()](/words/lists/get/) operation.

An object of the **GetListOnlineRequest** class is created by the following constructor methods:

- GetListOnlineRequest()
- GetListOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***listId***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***listId***         | ListId               | <span style="color:SteelBlue;">int</span>     | The list Id. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetListRequest

Represents a request model for [WordsApi.GetList()](/words/lists/get/) operation.

An object of the **GetListRequest** class is created by the following constructor methods:

- GetListRequest()
- GetListRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***listId***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***listId***         | ListId               | <span style="color:SteelBlue;">int</span>     | The list Id. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetListsOnlineRequest

Represents a request model for [WordsApi.GetListsOnline()](/words/lists/get-all/) operation.

An object of the **GetListsOnlineRequest** class is created by the following constructor methods:

- GetListsOnlineRequest()
- GetListsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetListsRequest

Represents a request model for [WordsApi.GetLists()](/words/lists/get-all/) operation.

An object of the **GetListsRequest** class is created by the following constructor methods:

- GetListsRequest()
- GetListsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## InsertListOnlineRequest

Represents a request model for [WordsApi.InsertListOnline()](/words/lists/insert/) operation.

An object of the **InsertListOnlineRequest** class is created by the following constructor methods:

- InsertListOnlineRequest()
- InsertListOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [ListInsert](#listinsert) ***listInsert***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***listInsert***     | ListInsert           | [ListInsert](#listinsert)                     | List object. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertListOnlineResponse

Represents a response model for [WordsApi.InsertListOnline()](/words/lists/insert/) operation.

An object of the **InsertListOnlineResponse** class is created by the following constructor methods:

- InsertListOnlineResponse([ListResponse](#listresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [ListResponse](#listresponse)                 | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertListRequest

Represents a request model for [WordsApi.InsertList()](/words/lists/insert/) operation.

An object of the **InsertListRequest** class is created by the following constructor methods:

- InsertListRequest()
- InsertListRequest(<span style="color:SteelBlue;">string</span> ***name***, [ListInsert](#listinsert) ***listInsert***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***listInsert***     | ListInsert           | [ListInsert](#listinsert)                     | List object. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## ListResponse

Represents a REST response with a list information.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertListOnlineResponse](#insertlistonlineresponse), [UpdateListLevelOnlineResponse](#updatelistlevelonlineresponse), [UpdateListOnlineResponse](#updatelistonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| List                 | [ListInfo](#listinfo)                         | Gets or sets the list information. |


## ListsResponse

Represents a REST response with a collection of lists, contained in the document.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Lists                | [Lists](#lists)                               | Gets or sets the collection of lists, contained in the document. |


## UpdateListLevelOnlineRequest

Represents a request model for [WordsApi.UpdateListLevelOnline()](/words/lists/update-level/) operation.

An object of the **UpdateListLevelOnlineRequest** class is created by the following constructor methods:

- UpdateListLevelOnlineRequest()
- UpdateListLevelOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***listId***, [ListLevelUpdate](#listlevelupdate) ***listUpdate***, <span style="color:SteelBlue;">int</span> ***listLevel***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***listId***         | ListId               | <span style="color:SteelBlue;">int</span>     | The list Id. |
| ***listUpdate***     | ListUpdate           | [ListLevelUpdate](#listlevelupdate)           | List object. |
| ***listLevel***      | ListLevel            | <span style="color:SteelBlue;">int</span>     | The list level. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateListLevelOnlineResponse

Represents a response model for [WordsApi.UpdateListLevelOnline()](/words/lists/update-level/) operation.

An object of the **UpdateListLevelOnlineResponse** class is created by the following constructor methods:

- UpdateListLevelOnlineResponse([ListResponse](#listresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [ListResponse](#listresponse)                 | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateListLevelRequest

Represents a request model for [WordsApi.UpdateListLevel()](/words/lists/update-level/) operation.

An object of the **UpdateListLevelRequest** class is created by the following constructor methods:

- UpdateListLevelRequest()
- UpdateListLevelRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***listId***, <span style="color:SteelBlue;">int</span> ***listLevel***, [ListLevelUpdate](#listlevelupdate) ***listUpdate***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***listId***         | ListId               | <span style="color:SteelBlue;">int</span>     | The list Id. |
| ***listLevel***      | ListLevel            | <span style="color:SteelBlue;">int</span>     | The list level. |
| ***listUpdate***     | ListUpdate           | [ListLevelUpdate](#listlevelupdate)           | List object. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateListOnlineRequest

Represents a request model for [WordsApi.UpdateListOnline()](/words/lists/update/) operation.

An object of the **UpdateListOnlineRequest** class is created by the following constructor methods:

- UpdateListOnlineRequest()
- UpdateListOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***listId***, [ListUpdate](#listupdate) ***listUpdate***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***listId***         | ListId               | <span style="color:SteelBlue;">int</span>     | The list Id. |
| ***listUpdate***     | ListUpdate           | [ListUpdate](#listupdate)                     | List object. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateListOnlineResponse

Represents a response model for [WordsApi.UpdateListOnline()](/words/lists/update/) operation.

An object of the **UpdateListOnlineResponse** class is created by the following constructor methods:

- UpdateListOnlineResponse([ListResponse](#listresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [ListResponse](#listresponse)                 | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateListRequest

Represents a request model for [WordsApi.UpdateList()](/words/lists/update/) operation.

An object of the **UpdateListRequest** class is created by the following constructor methods:

- UpdateListRequest()
- UpdateListRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***listId***, [ListUpdate](#listupdate) ***listUpdate***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***listId***         | ListId               | <span style="color:SteelBlue;">int</span>     | The list Id. |
| ***listUpdate***     | ListUpdate           | [ListUpdate](#listupdate)                     | List object. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## ListInsert.TemplateEnum

The following values are defined: BulletDefault, BulletDisk, BulletCircle, BulletSquare, BulletDiamonds, BulletArrowHead, BulletTick, NumberDefault, NumberArabicDot, NumberArabicParenthesis, NumberUppercaseRomanDot, NumberUppercaseLetterDot, NumberLowercaseLetterParenthesis, NumberLowercaseLetterDot, NumberLowercaseRomanDot, OutlineNumbers, OutlineLegal, OutlineBullets, OutlineHeadingsArticleSection, OutlineHeadingsLegal, OutlineHeadingsNumbers, OutlineHeadingsChapter.


## ListLevel.AlignmentEnum

The following values are defined: Left, Center, Right.


## ListLevel.NumberStyleEnum

The following values are defined: Arabic, UppercaseRoman, LowercaseRoman, UppercaseLetter, LowercaseLetter, Ordinal, Number, OrdinalText, Hex, ChicagoManual, Kanji, KanjiDigit, AiueoHalfWidth, IrohaHalfWidth, ArabicFullWidth, ArabicHalfWidth, KanjiTraditional, KanjiTraditional2, NumberInCircle, DecimalFullWidth, Aiueo, Iroha, LeadingZero, Bullet, Ganada, Chosung, GB1, GB2, GB3, GB4, Zodiac1, Zodiac2, Zodiac3, TradChinNum1, TradChinNum2, TradChinNum3, TradChinNum4, SimpChinNum1, SimpChinNum2, SimpChinNum3, SimpChinNum4, HanjaRead, HanjaReadDigit, Hangul, Hanja, Hebrew1, Arabic1, Hebrew2, Arabic2, HindiLetter1, HindiLetter2, HindiArabic, HindiCardinalText, ThaiLetter, ThaiArabic, ThaiCardinalText, VietCardinalText, NumberInDash, LowercaseRussian, UppercaseRussian, None, Custom.


## ListLevel.TrailingCharacterEnum

The following values are defined: Tab, Space, Nothing.


## ListLevelUpdate.AlignmentEnum

The following values are defined: Left, Center, Right.


## ListLevelUpdate.NumberStyleEnum

The following values are defined: Arabic, UppercaseRoman, LowercaseRoman, UppercaseLetter, LowercaseLetter, Ordinal, Number, OrdinalText, Hex, ChicagoManual, Kanji, KanjiDigit, AiueoHalfWidth, IrohaHalfWidth, ArabicFullWidth, ArabicHalfWidth, KanjiTraditional, KanjiTraditional2, NumberInCircle, DecimalFullWidth, Aiueo, Iroha, LeadingZero, Bullet, Ganada, Chosung, GB1, GB2, GB3, GB4, Zodiac1, Zodiac2, Zodiac3, TradChinNum1, TradChinNum2, TradChinNum3, TradChinNum4, SimpChinNum1, SimpChinNum2, SimpChinNum3, SimpChinNum4, HanjaRead, HanjaReadDigit, Hangul, Hanja, Hebrew1, Arabic1, Hebrew2, Arabic2, HindiLetter1, HindiLetter2, HindiArabic, HindiCardinalText, ThaiLetter, ThaiArabic, ThaiCardinalText, VietCardinalText, NumberInDash, LowercaseRussian, UppercaseRussian, None, Custom.


## ListLevelUpdate.TrailingCharacterEnum

The following values are defined: Tab, Space, Nothing.

