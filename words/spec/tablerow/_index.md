---
title: "TableRow"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/tablerow/
description: "TableRow"
notoc: true
weight: 480
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
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletetablerowonlinerequest">DeleteTableRowOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletetablerowrequest">DeleteTableRowRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablerowformatonlinerequest">GetTableRowFormatOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablerowformatresponse">TableRowFormatResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablerowformat">TableRowFormat</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablerowformatrequest">GetTableRowFormatRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablerowonlinerequest">GetTableRowOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablerowresponse">TableRowResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablerow">TableRow</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablerowrequest">GetTableRowRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#inserttablerowonlinerequest">InsertTableRowOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#inserttablerowonlineresponse">InsertTableRowOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tablerowinsert">TableRowInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#inserttablerowrequest">InsertTableRowRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tablerowresponse">TableRowResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tablerow">TableRow</a></br><a href="#tablerowinsert">TableRowInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatetablerowformatonlinerequest">UpdateTableRowFormatOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatetablerowformatonlineresponse">UpdateTableRowFormatOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablerowformat">TableRowFormat</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatetablerowformatrequest">UpdateTableRowFormatRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tablerowformatresponse">TableRowFormatResponse</a></td>
  </tr>
  </tbody>
</table>


## TableRow

Represents a dTO container with a table row element.

This class is inherited from [NodeLink](/words/spec/link#nodelink) and used in [Table](/words/spec/table#table), [TableRowResponse](#tablerowresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| RowFormat            | [TableRowFormat](#tablerowformat)             | Gets or sets the formatting properties of a row. |
| TableCellList        | List&lt;[TableCell](/words/spec/tablecell#tablecell)&gt; | Gets or sets the collection of rows. |


## TableRowFormatDto

Represents a tableRowFormatDto.


## TableRowInsertDto

Represents a dTO container with a table row element.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ColumnsCount         | <span style="color:SteelBlue;">int</span>     | Gets or sets the count of columns. The default value is 1. |
| InsertAfter          | <span style="color:SteelBlue;">int</span>     | Gets or sets table row will be inserted after row with specified 0-based index. |


## TableRowFormat

Represents a dTO container with formatting for a table row.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [TableRow](#tablerow), [TableRowFormatResponse](#tablerowformatresponse), [UpdateTableRowFormatOnlineRequest](#updatetablerowformatonlinerequest), [UpdateTableRowFormatRequest](#updatetablerowformatrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| AllowBreakAcrossPages | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the text in a table row is allowed to split across a page break. |
| HeadingFormat        | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the row is repeated as a table heading on every page when the table spans more than one page. |
| Height               | <span style="color:SteelBlue;">double</span>  | Gets or sets the height of the table row in points. |
| HeightRule           | [HeightRuleEnum](#tablerowformat.heightruleenum) | Gets or sets the rule for determining the height of the table row. |


## TableRowInsert

Represents a dTO container with a table row element.

This class is used in [InsertTableRowOnlineRequest](#inserttablerowonlinerequest), [InsertTableRowRequest](#inserttablerowrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ColumnsCount         | <span style="color:SteelBlue;">int</span>     | Gets or sets the count of columns. The default value is 1. |
| InsertAfter          | <span style="color:SteelBlue;">int</span>     | Gets or sets table row will be inserted after row with specified 0-based index. |


## DeleteTableRowOnlineRequest

Represents a request model for [WordsApi.DeleteTableRowOnline()](/words/tables/delete-row/) operation.

An object of the **DeleteTableRowOnlineRequest** class is created by the following constructor methods:

- DeleteTableRowOnlineRequest()
- DeleteTableRowOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tablePath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteTableRowRequest

Represents a request model for [WordsApi.DeleteTableRow()](/words/tables/delete-row/) operation.

An object of the **DeleteTableRowRequest** class is created by the following constructor methods:

- DeleteTableRowRequest()
- DeleteTableRowRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tablePath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## GetTableRowFormatOnlineRequest

Represents a request model for [WordsApi.GetTableRowFormatOnline()](/words/tables/get-row-format/) operation.

An object of the **GetTableRowFormatOnlineRequest** class is created by the following constructor methods:

- GetTableRowFormatOnlineRequest()
- GetTableRowFormatOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tablePath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetTableRowFormatRequest

Represents a request model for [WordsApi.GetTableRowFormat()](/words/tables/get-row-format/) operation.

An object of the **GetTableRowFormatRequest** class is created by the following constructor methods:

- GetTableRowFormatRequest()
- GetTableRowFormatRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tablePath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetTableRowOnlineRequest

Represents a request model for [WordsApi.GetTableRowOnline()](/words/tables/get-row/) operation.

An object of the **GetTableRowOnlineRequest** class is created by the following constructor methods:

- GetTableRowOnlineRequest()
- GetTableRowOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tablePath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetTableRowRequest

Represents a request model for [WordsApi.GetTableRow()](/words/tables/get-row/) operation.

An object of the **GetTableRowRequest** class is created by the following constructor methods:

- GetTableRowRequest()
- GetTableRowRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tablePath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## InsertTableRowOnlineRequest

Represents a request model for [WordsApi.InsertTableRowOnline()](/words/tables/add-row/) operation.

An object of the **InsertTableRowOnlineRequest** class is created by the following constructor methods:

- InsertTableRowOnlineRequest()
- InsertTableRowOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tablePath***, [TableRowInsert](#tablerowinsert) ***row***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***row***            | Row                  | [TableRowInsert](#tablerowinsert)             | Table row parameters. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertTableRowOnlineResponse

Represents a response model for [WordsApi.InsertTableRowOnline()](/words/tables/add-row/) operation.

An object of the **InsertTableRowOnlineResponse** class is created by the following constructor methods:

- InsertTableRowOnlineResponse([TableRowResponse](#tablerowresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [TableRowResponse](#tablerowresponse)         | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## InsertTableRowRequest

Represents a request model for [WordsApi.InsertTableRow()](/words/tables/add-row/) operation.

An object of the **InsertTableRowRequest** class is created by the following constructor methods:

- InsertTableRowRequest()
- InsertTableRowRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tablePath***, [TableRowInsert](#tablerowinsert) ***row***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***row***            | Row                  | [TableRowInsert](#tablerowinsert)             | Table row parameters. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## TableRowFormatResponse

Represents a REST response with the formatting properties of a table row.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [UpdateTableRowFormatOnlineResponse](#updatetablerowformatonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| RowFormat            | [TableRowFormat](#tablerowformat)             | Gets or sets the formatting properties of a table row. |


## TableRowResponse

Represents a REST response with a table row.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertTableRowOnlineResponse](#inserttablerowonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Row                  | [TableRow](#tablerow)                         | Gets or sets the table row. |


## UpdateTableRowFormatOnlineRequest

Represents a request model for [WordsApi.UpdateTableRowFormatOnline()](/words/tables/update-row-format/) operation.

An object of the **UpdateTableRowFormatOnlineRequest** class is created by the following constructor methods:

- UpdateTableRowFormatOnlineRequest()
- UpdateTableRowFormatOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tablePath***, [TableRowFormat](#tablerowformat) ***format***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***format***         | Format               | [TableRowFormat](#tablerowformat)             | Table row format. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateTableRowFormatOnlineResponse

Represents a response model for [WordsApi.UpdateTableRowFormatOnline()](/words/tables/update-row-format/) operation.

An object of the **UpdateTableRowFormatOnlineResponse** class is created by the following constructor methods:

- UpdateTableRowFormatOnlineResponse([TableRowFormatResponse](#tablerowformatresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [TableRowFormatResponse](#tablerowformatresponse) | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## UpdateTableRowFormatRequest

Represents a request model for [WordsApi.UpdateTableRowFormat()](/words/tables/update-row-format/) operation.

An object of the **UpdateTableRowFormatRequest** class is created by the following constructor methods:

- UpdateTableRowFormatRequest()
- UpdateTableRowFormatRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tablePath***, <span style="color:SteelBlue;">int</span> ***index***, [TableRowFormat](#tablerowformat) ***format***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tablePath***      | TablePath            | <span style="color:SteelBlue;">string</span>  | The path to the table in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***format***         | Format               | [TableRowFormat](#tablerowformat)             | Table row format. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## TableRowFormat.HeightRuleEnum

The following values are defined: AtLeast, Exactly, Auto.

