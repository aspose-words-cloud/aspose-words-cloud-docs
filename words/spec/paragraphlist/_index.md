---
title: "ParagraphList"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/paragraphlist/
description: "ParagraphList"
notoc: true
weight: 370
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
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteparagraphlistformatonlinerequest">DeleteParagraphListFormatOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#deleteparagraphlistformatonlineresponse">DeleteParagraphListFormatOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteparagraphlistformatrequest">DeleteParagraphListFormatRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="3"><a href="#paragraphlistformatresponse">ParagraphListFormatResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="3"><a href="#listformat">ListFormat</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getparagraphlistformatonlinerequest">GetParagraphListFormatOnlineRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getparagraphlistformatrequest">GetParagraphListFormatRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updateparagraphlistformatonlinerequest">UpdateParagraphListFormatOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updateparagraphlistformatonlineresponse">UpdateParagraphListFormatOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listformatupdate">ListFormatUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updateparagraphlistformatrequest">UpdateParagraphListFormatRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#paragraphlistformatresponse">ParagraphListFormatResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#listformat">ListFormat</a></br><a href="#listformatupdate">ListFormatUpdate</a></td>
  </tr>
  </tbody>
</table>


## ListFormat

Represents a dTO container with a paragraph list format element.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [ParagraphListFormatResponse](#paragraphlistformatresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| IsListItem           | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the paragraph has bulleted or numbered formatting applied to it. |
| ListId               | <span style="color:SteelBlue;">int</span>     | Gets or sets the list id of this paragraph. |
| ListLevelNumber      | <span style="color:SteelBlue;">int</span>     | Gets or sets the list level number (0 to 8) for the paragraph. |


## ListFormatUpdate

Represents a paragraph list format element for update.

This class is used in [UpdateParagraphListFormatOnlineRequest](#updateparagraphlistformatonlinerequest), [UpdateParagraphListFormatRequest](#updateparagraphlistformatrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ListId               | <span style="color:SteelBlue;">int</span>     | Gets or sets the list id of this paragraph. |
| ListLevelNumber      | <span style="color:SteelBlue;">int</span>     | Gets or sets the list level number (0 to 8) for the paragraph. |


## DeleteParagraphListFormatOnlineRequest

Represents a request model for [WordsApi.DeleteParagraphListFormatOnline()](/words/paragraphs/lists/delete-paragraph-list-format-in-a-document/) operation.

An object of the **DeleteParagraphListFormatOnlineRequest** class is created by the following constructor methods:

- DeleteParagraphListFormatOnlineRequest()
- DeleteParagraphListFormatOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteParagraphListFormatOnlineResponse

Represents a response model for [WordsApi.DeleteParagraphListFormatOnline()](/words/paragraphs/lists/delete-paragraph-list-format-in-a-document/) operation.

An object of the **DeleteParagraphListFormatOnlineResponse** class is created by the following constructor methods:

- DeleteParagraphListFormatOnlineResponse([ParagraphListFormatResponse](#paragraphlistformatresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [ParagraphListFormatResponse](#paragraphlistformatresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## DeleteParagraphListFormatRequest

Represents a request model for [WordsApi.DeleteParagraphListFormat()](/words/paragraphs/lists/delete-paragraph-list-format-in-a-document/) operation.

An object of the **DeleteParagraphListFormatRequest** class is created by the following constructor methods:

- DeleteParagraphListFormatRequest()
- DeleteParagraphListFormatRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## GetParagraphListFormatOnlineRequest

Represents a request model for [WordsApi.GetParagraphListFormatOnline()](/words/paragraphs/lists/get-paragraph-list-format-in-a-document/) operation.

An object of the **GetParagraphListFormatOnlineRequest** class is created by the following constructor methods:

- GetParagraphListFormatOnlineRequest()
- GetParagraphListFormatOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetParagraphListFormatRequest

Represents a request model for [WordsApi.GetParagraphListFormat()](/words/paragraphs/lists/get-paragraph-list-format-in-a-document/) operation.

An object of the **GetParagraphListFormatRequest** class is created by the following constructor methods:

- GetParagraphListFormatRequest()
- GetParagraphListFormatRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## ParagraphListFormatResponse

Represents a REST response with a list format for a paragraph.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [DeleteParagraphListFormatOnlineResponse](#deleteparagraphlistformatonlineresponse), [UpdateParagraphListFormatOnlineResponse](#updateparagraphlistformatonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| ListFormat           | [ListFormat](#listformat)                     | Gets or sets the list format for a paragraph. |


## UpdateParagraphListFormatOnlineRequest

Represents a request model for [WordsApi.UpdateParagraphListFormatOnline()](/words/paragraphs/lists/update-paragraph-list-format-in-a-document/) operation.

An object of the **UpdateParagraphListFormatOnlineRequest** class is created by the following constructor methods:

- UpdateParagraphListFormatOnlineRequest()
- UpdateParagraphListFormatOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [ListFormatUpdate](#listformatupdate) ***listFormatDto***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***listFormatDto***  | ListFormatDto        | [ListFormatUpdate](#listformatupdate)         | ListFormatUpdate dto. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateParagraphListFormatOnlineResponse

Represents a response model for [WordsApi.UpdateParagraphListFormatOnline()](/words/paragraphs/lists/update-paragraph-list-format-in-a-document/) operation.

An object of the **UpdateParagraphListFormatOnlineResponse** class is created by the following constructor methods:

- UpdateParagraphListFormatOnlineResponse([ParagraphListFormatResponse](#paragraphlistformatresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [ParagraphListFormatResponse](#paragraphlistformatresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateParagraphListFormatRequest

Represents a request model for [WordsApi.UpdateParagraphListFormat()](/words/paragraphs/lists/update-paragraph-list-format-in-a-document/) operation.

An object of the **UpdateParagraphListFormatRequest** class is created by the following constructor methods:

- UpdateParagraphListFormatRequest()
- UpdateParagraphListFormatRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, [ListFormatUpdate](#listformatupdate) ***listFormatDto***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***listFormatDto***  | ListFormatDto        | [ListFormatUpdate](#listformatupdate)         | ListFormatUpdate dto. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |


