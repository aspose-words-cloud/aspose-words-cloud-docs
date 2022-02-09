---
title: "ParagraphTabStop"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/paragraphtabstop/
description: "ParagraphTabStop"
notoc: true
weight: 390
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>DeleteAll</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteallparagraphtabstopsonlinerequest">DeleteAllParagraphTabStopsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#deleteallparagraphtabstopsonlineresponse">DeleteAllParagraphTabStopsOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteallparagraphtabstopsrequest">DeleteAllParagraphTabStopsRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tabstopsresponse">TabStopsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tabstop">TabStop</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Delete</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteparagraphtabstoponlinerequest">DeleteParagraphTabStopOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#deleteparagraphtabstoponlineresponse">DeleteParagraphTabStopOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteparagraphtabstoprequest">DeleteParagraphTabStopRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="3"><a href="#tabstopsresponse">TabStopsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="3"><a href="#tabstop">TabStop</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getparagraphtabstopsonlinerequest">GetParagraphTabStopsOnlineRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getparagraphtabstopsrequest">GetParagraphTabStopsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>InsertOrUpdate</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertorupdateparagraphtabstoponlinerequest">InsertOrUpdateParagraphTabStopOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertorupdateparagraphtabstoponlineresponse">InsertOrUpdateParagraphTabStopOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tabstopinsert">TabStopInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertorupdateparagraphtabstoprequest">InsertOrUpdateParagraphTabStopRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tabstopsresponse">TabStopsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#tabstop">TabStop</a></br><a href="#tabstopinsert">TabStopInsert</a></td>
  </tr>
  </tbody>
</table>


## TabStopBase

Represents a base class for paragraph format tab stop DTO.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Alignment            | [AlignmentEnum](#tabstopbase.alignmentenum)   | Gets or sets the alignment of text at this tab stop. |
| Leader               | [LeaderEnum](#tabstopbase.leaderenum)         | Gets or sets the type of the leader line displayed under the tab character. |
| Position             | <span style="color:SteelBlue;">double</span>  | Gets or sets the position of the tab stop in points. |


## TabStop

Represents a dTO container with paragraph format tab stop.

This class is inherited from [TabStopBase](#tabstopbase) and used in [TabStopsResponse](#tabstopsresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Alignment            | [AlignmentEnum](#tabstopbase.alignmentenum)   | Gets or sets the alignment of text at this tab stop. |
| Leader               | [LeaderEnum](#tabstopbase.leaderenum)         | Gets or sets the type of the leader line displayed under the tab character. |
| Position             | <span style="color:SteelBlue;">double</span>  | Gets or sets the position of the tab stop in points. |
| IsClear              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this tab stop clears any existing tab stops in this position. |


## TabStopInsert

Represents a DTO to Insert / replace a tab stop.

This class is inherited from [TabStopBase](#tabstopbase) and used in [InsertOrUpdateParagraphTabStopOnlineRequest](#insertorupdateparagraphtabstoponlinerequest), [InsertOrUpdateParagraphTabStopRequest](#insertorupdateparagraphtabstoprequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Alignment            | [AlignmentEnum](#tabstopbase.alignmentenum)   | Gets or sets the alignment of text at this tab stop. |
| Leader               | [LeaderEnum](#tabstopbase.leaderenum)         | Gets or sets the type of the leader line displayed under the tab character. |
| Position             | <span style="color:SteelBlue;">double</span>  | Gets or sets the position of the tab stop in points. |


## DeleteAllParagraphTabStopsOnlineRequest

Represents a request model for [WordsApi.DeleteAllParagraphTabStopsOnline()](/words/paragraphs/tab-stop/delete-all-paragraph-tab-stops-in-a-document/) operation.

An object of the **DeleteAllParagraphTabStopsOnlineRequest** class is created by the following constructor methods:

- DeleteAllParagraphTabStopsOnlineRequest()
- DeleteAllParagraphTabStopsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

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



## DeleteAllParagraphTabStopsOnlineResponse

Represents a response model for [WordsApi.DeleteAllParagraphTabStopsOnline()](/words/paragraphs/tab-stop/delete-all-paragraph-tab-stops-in-a-document/) operation.

An object of the **DeleteAllParagraphTabStopsOnlineResponse** class is created by the following constructor methods:

- DeleteAllParagraphTabStopsOnlineResponse([TabStopsResponse](#tabstopsresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [TabStopsResponse](#tabstopsresponse)         | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## DeleteAllParagraphTabStopsRequest

Represents a request model for [WordsApi.DeleteAllParagraphTabStops()](/words/paragraphs/tab-stop/delete-all-paragraph-tab-stops-in-a-document/) operation.

An object of the **DeleteAllParagraphTabStopsRequest** class is created by the following constructor methods:

- DeleteAllParagraphTabStopsRequest()
- DeleteAllParagraphTabStopsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

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



## DeleteParagraphTabStopOnlineRequest

Represents a request model for [WordsApi.DeleteParagraphTabStopOnline()](/words/paragraphs/tab-stop/delete-a-paragraph-tab-stop-in-a-document/) operation.

An object of the **DeleteParagraphTabStopOnlineRequest** class is created by the following constructor methods:

- DeleteParagraphTabStopOnlineRequest()
- DeleteParagraphTabStopOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">double</span> ***position***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***position***       | Position             | <span style="color:SteelBlue;">double</span>  | The position of a tab stop to remove. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## DeleteParagraphTabStopOnlineResponse

Represents a response model for [WordsApi.DeleteParagraphTabStopOnline()](/words/paragraphs/tab-stop/delete-a-paragraph-tab-stop-in-a-document/) operation.

An object of the **DeleteParagraphTabStopOnlineResponse** class is created by the following constructor methods:

- DeleteParagraphTabStopOnlineResponse([TabStopsResponse](#tabstopsresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [TabStopsResponse](#tabstopsresponse)         | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## DeleteParagraphTabStopRequest

Represents a request model for [WordsApi.DeleteParagraphTabStop()](/words/paragraphs/tab-stop/delete-a-paragraph-tab-stop-in-a-document/) operation.

An object of the **DeleteParagraphTabStopRequest** class is created by the following constructor methods:

- DeleteParagraphTabStopRequest()
- DeleteParagraphTabStopRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">double</span> ***position***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***position***       | Position             | <span style="color:SteelBlue;">double</span>  | The position of a tab stop to remove. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## GetParagraphTabStopsOnlineRequest

Represents a request model for [WordsApi.GetParagraphTabStopsOnline()](/words/paragraphs/tab-stop/get-paragraph-tab-stop-in-a-document/) operation.

An object of the **GetParagraphTabStopsOnlineRequest** class is created by the following constructor methods:

- GetParagraphTabStopsOnlineRequest()
- GetParagraphTabStopsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetParagraphTabStopsRequest

Represents a request model for [WordsApi.GetParagraphTabStops()](/words/paragraphs/tab-stop/get-paragraph-tab-stop-in-a-document/) operation.

An object of the **GetParagraphTabStopsRequest** class is created by the following constructor methods:

- GetParagraphTabStopsRequest()
- GetParagraphTabStopsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

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



## InsertOrUpdateParagraphTabStopOnlineRequest

Represents a request model for [WordsApi.InsertOrUpdateParagraphTabStopOnline()](/words/paragraphs/tab-stop/insert-or-update-paragraph-tab-stop-in-a-document/) operation.

An object of the **InsertOrUpdateParagraphTabStopOnlineRequest** class is created by the following constructor methods:

- InsertOrUpdateParagraphTabStopOnlineRequest()
- InsertOrUpdateParagraphTabStopOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [TabStopInsert](#tabstopinsert) ***tabStopInsertDto***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***tabStopInsertDto*** | TabStopInsertDto     | [TabStopInsert](#tabstopinsert)               | TabStopInsert dto. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## InsertOrUpdateParagraphTabStopOnlineResponse

Represents a response model for [WordsApi.InsertOrUpdateParagraphTabStopOnline()](/words/paragraphs/tab-stop/insert-or-update-paragraph-tab-stop-in-a-document/) operation.

An object of the **InsertOrUpdateParagraphTabStopOnlineResponse** class is created by the following constructor methods:

- InsertOrUpdateParagraphTabStopOnlineResponse([TabStopsResponse](#tabstopsresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [TabStopsResponse](#tabstopsresponse)         | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertOrUpdateParagraphTabStopRequest

Represents a request model for [WordsApi.InsertOrUpdateParagraphTabStop()](/words/paragraphs/tab-stop/insert-or-update-paragraph-tab-stop-in-a-document/) operation.

An object of the **InsertOrUpdateParagraphTabStopRequest** class is created by the following constructor methods:

- InsertOrUpdateParagraphTabStopRequest()
- InsertOrUpdateParagraphTabStopRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, [TabStopInsert](#tabstopinsert) ***tabStopInsertDto***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***tabStopInsertDto*** | TabStopInsertDto     | [TabStopInsert](#tabstopinsert)               | TabStopInsert dto. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## TabStopsResponse

Represents a REST response with an array of tab stops.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [DeleteAllParagraphTabStopsOnlineResponse](#deleteallparagraphtabstopsonlineresponse), [DeleteParagraphTabStopOnlineResponse](#deleteparagraphtabstoponlineresponse), [InsertOrUpdateParagraphTabStopOnlineResponse](#insertorupdateparagraphtabstoponlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| TabStops             | List&lt;[TabStop](#tabstop)&gt;               | Gets or sets the array of tab stops. |


## TabStopBase.AlignmentEnum

The following values are defined: Left, Center, Right, Decimal, Bar, List, Clear.


## TabStopBase.LeaderEnum

The following values are defined: None, Dots, Dashes, Line, Heavy, MiddleDot.

