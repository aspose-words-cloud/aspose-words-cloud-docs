---
title: "TableCell"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/tablecell/
description: "TableCell"
notoc: true
weight: 460
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
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletetablecellonlinerequest">DeleteTableCellOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletetablecellrequest">DeleteTableCellRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablecellformatonlinerequest">GetTableCellFormatOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablecellformatresponse">TableCellFormatResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablecellformat">TableCellFormat</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablecellformatrequest">GetTableCellFormatRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablecellonlinerequest">GetTableCellOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablecellresponse">TableCellResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablecell">TableCell</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#gettablecellrequest">GetTableCellRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#inserttablecellonlinerequest">InsertTableCellOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#inserttablecellonlineresponse">InsertTableCellOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tablecellinsert">TableCellInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#inserttablecellrequest">InsertTableCellRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tablecellresponse">TableCellResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tablecell">TableCell</a></br><a href="#tablecellinsert">TableCellInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatetablecellformatonlinerequest">UpdateTableCellFormatOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatetablecellformatonlineresponse">UpdateTableCellFormatOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#tablecellformat">TableCellFormat</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatetablecellformatrequest">UpdateTableCellFormatRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tablecellformatresponse">TableCellFormatResponse</a></td>
  </tr>
  </tbody>
</table>


## TableCell

Represents a dTO container with a table cell element.

This class is inherited from [NodeLink](/words/spec/link#nodelink) and used in [TableCellResponse](#tablecellresponse), [TableRow](/words/spec/tablerow#tablerow).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| ChildNodes           | List&lt;[NodeLink](/words/spec/link#nodelink)&gt; | Gets or sets the list of child nodes. |


## TableCellFormatDto

Represents a tableCellFormatDto.


## TableCellInsertDto

Represents a dTO container with a table cell.

A single `InsertAfter` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| InsertAfter          | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index, the table cell will be inserted after. |


## TableCellFormat

Represents a dTO container with all formatting for a table row.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [TableCellFormatResponse](#tablecellformatresponse), [UpdateTableCellFormatOnlineRequest](#updatetablecellformatonlinerequest), [UpdateTableCellFormatRequest](#updatetablecellformatrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| BottomPadding        | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of space (in points) to add below the contents of the cell. |
| FitText              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to fit text in the cell, compress each paragraph to the width of the cell. |
| HorizontalMerge      | [HorizontalMergeEnum](#tablecellformat.horizontalmergeenum) | Gets or sets the option that controls how the cell is merged horizontally with other cells in the row. |
| LeftPadding          | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of space (in points) to add to the left of the contents of the cell. |
| Orientation          | [OrientationEnum](#tablecellformat.orientationenum) | Gets or sets the orientation of text in a table cell. |
| PreferredWidth       | [PreferredWidth](/words/spec/table#preferredwidth) | Gets or sets the preferred width of the cell. |
| RightPadding         | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of space (in points) to add to the right of the contents of the cell. |
| TopPadding           | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of space (in points) to add above the contents of the cell. |
| VerticalAlignment    | [VerticalAlignmentEnum](#tablecellformat.verticalalignmentenum) | Gets or sets the vertical alignment of text in the cell. |
| VerticalMerge        | [VerticalMergeEnum](#tablecellformat.verticalmergeenum) | Gets or sets the option that controls how the cell is merged with other cells vertically. |
| Width                | <span style="color:SteelBlue;">double</span>  | Gets or sets the width of the cell in points. |
| WrapText             | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to wrap text in the cell. |


## TableCellInsert

Represents a dTO container with a table cell.

This class is used in [InsertTableCellOnlineRequest](#inserttablecellonlinerequest), [InsertTableCellRequest](#inserttablecellrequest).

A single `InsertAfter` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| InsertAfter          | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index, the table cell will be inserted after. |


## DeleteTableCellOnlineRequest

Represents a request model for [WordsApi.DeleteTableCellOnline()](/words/tables/delete-cell/) operation.

An object of the **DeleteTableCellOnlineRequest** class is created by the following constructor methods:

- DeleteTableCellOnlineRequest()
- DeleteTableCellOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteTableCellRequest

Represents a request model for [WordsApi.DeleteTableCell()](/words/tables/delete-cell/) operation.

An object of the **DeleteTableCellRequest** class is created by the following constructor methods:

- DeleteTableCellRequest()
- DeleteTableCellRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## GetTableCellFormatOnlineRequest

Represents a request model for [WordsApi.GetTableCellFormatOnline()](/words/tables/get-cell-format/) operation.

An object of the **GetTableCellFormatOnlineRequest** class is created by the following constructor methods:

- GetTableCellFormatOnlineRequest()
- GetTableCellFormatOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetTableCellFormatRequest

Represents a request model for [WordsApi.GetTableCellFormat()](/words/tables/get-cell-format/) operation.

An object of the **GetTableCellFormatRequest** class is created by the following constructor methods:

- GetTableCellFormatRequest()
- GetTableCellFormatRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetTableCellOnlineRequest

Represents a request model for [WordsApi.GetTableCellOnline()](/words/tables/get-cell/) operation.

An object of the **GetTableCellOnlineRequest** class is created by the following constructor methods:

- GetTableCellOnlineRequest()
- GetTableCellOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetTableCellRequest

Represents a request model for [WordsApi.GetTableCell()](/words/tables/get-cell/) operation.

An object of the **GetTableCellRequest** class is created by the following constructor methods:

- GetTableCellRequest()
- GetTableCellRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## InsertTableCellOnlineRequest

Represents a request model for [WordsApi.InsertTableCellOnline()](/words/tables/add-cell/) operation.

An object of the **InsertTableCellOnlineRequest** class is created by the following constructor methods:

- InsertTableCellOnlineRequest()
- InsertTableCellOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, [TableCellInsert](#tablecellinsert) ***cell***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***cell***           | Cell                 | [TableCellInsert](#tablecellinsert)           | Table cell parameters. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertTableCellOnlineResponse

Represents a response model for [WordsApi.InsertTableCellOnline()](/words/tables/add-cell/) operation.

An object of the **InsertTableCellOnlineResponse** class is created by the following constructor methods:

- InsertTableCellOnlineResponse([TableCellResponse](#tablecellresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [TableCellResponse](#tablecellresponse)       | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## InsertTableCellRequest

Represents a request model for [WordsApi.InsertTableCell()](/words/tables/add-cell/) operation.

An object of the **InsertTableCellRequest** class is created by the following constructor methods:

- InsertTableCellRequest()
- InsertTableCellRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, [TableCellInsert](#tablecellinsert) ***cell***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***cell***           | Cell                 | [TableCellInsert](#tablecellinsert)           | Table cell parameters. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## TableCellFormatResponse

Represents a REST response with the formatting properties of a table cell.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [UpdateTableCellFormatOnlineResponse](#updatetablecellformatonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| CellFormat           | [TableCellFormat](#tablecellformat)           | Gets or sets the formatting properties of a table cell. |


## TableCellResponse

Represents a REST response with a table cell.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertTableCellOnlineResponse](#inserttablecellonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Cell                 | [TableCell](#tablecell)                       | Gets or sets the table cell. |


## UpdateTableCellFormatOnlineRequest

Represents a request model for [WordsApi.UpdateTableCellFormatOnline()](/words/tables/update-cell-format/) operation.

An object of the **UpdateTableCellFormatOnlineRequest** class is created by the following constructor methods:

- UpdateTableCellFormatOnlineRequest()
- UpdateTableCellFormatOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, [TableCellFormat](#tablecellformat) ***format***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***format***         | Format               | [TableCellFormat](#tablecellformat)           | The properties. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateTableCellFormatOnlineResponse

Represents a response model for [WordsApi.UpdateTableCellFormatOnline()](/words/tables/update-cell-format/) operation.

An object of the **UpdateTableCellFormatOnlineResponse** class is created by the following constructor methods:

- UpdateTableCellFormatOnlineResponse([TableCellFormatResponse](#tablecellformatresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [TableCellFormatResponse](#tablecellformatresponse) | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## UpdateTableCellFormatRequest

Represents a request model for [WordsApi.UpdateTableCellFormat()](/words/tables/update-cell-format/) operation.

An object of the **UpdateTableCellFormatRequest** class is created by the following constructor methods:

- UpdateTableCellFormatRequest()
- UpdateTableCellFormatRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***tableRowPath***, <span style="color:SteelBlue;">int</span> ***index***, [TableCellFormat](#tablecellformat) ***format***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***tableRowPath***   | TableRowPath         | <span style="color:SteelBlue;">string</span>  | The path to the table row in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***format***         | Format               | [TableCellFormat](#tablecellformat)           | The properties. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## TableCellFormat.HorizontalMergeEnum

The following values are defined: None, First, Previous.


## TableCellFormat.OrientationEnum

The following values are defined: Horizontal, Downward, Upward, HorizontalRotatedFarEast, VerticalFarEast, VerticalRotatedFarEast.


## TableCellFormat.VerticalAlignmentEnum

The following values are defined: Top, Center, Bottom.


## TableCellFormat.VerticalMergeEnum

The following values are defined: None, First, Previous.

