---
title: "TableProperties"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/tableproperties/
description: "TableProperties"
notoc: true
weight: 470
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablepropertiesonlinerequest">GetTablePropertiesOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablepropertiesresponse">TablePropertiesResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><a href="#tableproperties">TableProperties</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablepropertiesrequest">GetTablePropertiesRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatetablepropertiesonlinerequest">UpdateTablePropertiesOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatetablepropertiesonlineresponse">UpdateTablePropertiesOnlineResponse</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatetablepropertiesrequest">UpdateTablePropertiesRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tablepropertiesresponse">TablePropertiesResponse</a></td>
  </tr>
  </tbody>
</table>


## TableProperties

Represents a dTO container with table properties.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [Table](/words/spec/table#table), [TablePropertiesResponse](#tablepropertiesresponse), [UpdateTablePropertiesOnlineRequest](#updatetablepropertiesonlinerequest), [UpdateTablePropertiesRequest](#updatetablepropertiesrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Alignment            | [AlignmentEnum](#tableproperties.alignmentenum) | Gets or sets the option that controls how an inline table is aligned in the document. |
| AllowAutoFit         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to automatically resize cells in a table to fit their contents. |
| Bidi                 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this is a right-to-left table. |
| BottomPadding        | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of space (in points) to add below the contents of cells. |
| CellSpacing          | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of space (in points) between the cells. |
| LeftIndent           | <span style="color:SteelBlue;">double</span>  | Gets or sets the value, that represents the left indent of the table. |
| LeftPadding          | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of space (in points) to add to the left of the contents of cells. |
| PreferredWidth       | [PreferredWidth](/words/spec/table#preferredwidth) | Gets or sets the table preferred width. Preferred width can be specified as a percentage, number of points or a special "auto" value. |
| RightPadding         | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of space (in points) to add to the right of the contents of cells. |
| StyleIdentifier      | [StyleIdentifierEnum](/words/spec/font#font.styleidentifierenum) | Gets or sets the locale independent style identifier of the table style applied to this table. |
| StyleName            | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the table style applied to this table. |
| StyleOptions         | [StyleOptionsEnum](/words/spec/style#tableproperties.styleoptionsenum) | Gets or sets the bit flags, that specify how a table style is applied to this table. |
| TextWrapping         | [TextWrappingEnum](#tableproperties.textwrappingenum) | Gets or sets the option that controls text wrapping for the table. |
| TopPadding           | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of space (in points) to add above the contents of cells. |


## TablePropertiesDto

Represents a tablePropertiesDto.


## GetTablePropertiesOnlineRequest

Represents a request model for [WordsApi.GetTablePropertiesOnline()](/words/tables/get-table-properties/) operation.

An object of the **GetTablePropertiesOnlineRequest** class is created by the following constructor methods:

- GetTablePropertiesOnlineRequest()
- GetTablePropertiesOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetTablePropertiesRequest

Represents a request model for [WordsApi.GetTableProperties()](/words/tables/get-table-properties/) operation.

An object of the **GetTablePropertiesRequest** class is created by the following constructor methods:

- GetTablePropertiesRequest()
- GetTablePropertiesRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

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



## TablePropertiesResponse

Represents a REST response with a table.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [UpdateTablePropertiesOnlineResponse](#updatetablepropertiesonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Properties           | [TableProperties](#tableproperties)           | Gets or sets the table. |


## UpdateTablePropertiesOnlineRequest

Represents a request model for [WordsApi.UpdateTablePropertiesOnline()](/words/tables/update-properties/) operation.

An object of the **UpdateTablePropertiesOnlineRequest** class is created by the following constructor methods:

- UpdateTablePropertiesOnlineRequest()
- UpdateTablePropertiesOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [TableProperties](#tableproperties) ***properties***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***properties***     | Properties           | [TableProperties](#tableproperties)           | The properties. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateTablePropertiesOnlineResponse

Represents a response model for [WordsApi.UpdateTablePropertiesOnline()](/words/tables/update-properties/) operation.

An object of the **UpdateTablePropertiesOnlineResponse** class is created by the following constructor methods:

- UpdateTablePropertiesOnlineResponse([TablePropertiesResponse](#tablepropertiesresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [TablePropertiesResponse](#tablepropertiesresponse) | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## UpdateTablePropertiesRequest

Represents a request model for [WordsApi.UpdateTableProperties()](/words/tables/update-properties/) operation.

An object of the **UpdateTablePropertiesRequest** class is created by the following constructor methods:

- UpdateTablePropertiesRequest()
- UpdateTablePropertiesRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, [TableProperties](#tableproperties) ***properties***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***properties***     | Properties           | [TableProperties](#tableproperties)           | The properties. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## TableProperties.AlignmentEnum

The following values are defined: Left, Center, Right.


## TableProperties.TextWrappingEnum

The following values are defined: Default, None, Around.

