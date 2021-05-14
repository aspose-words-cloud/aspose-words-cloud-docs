---
title: "Footnote"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/footnote/
description: "Footnote"
notoc: true
weight: 250
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
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletefootnoteonlinerequest">DeleteFootnoteOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletefootnoterequest">DeleteFootnoteRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">void</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getfootnoteonlinerequest">GetFootnoteOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#footnoteresponse">FootnoteResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#footnote">Footnote</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getfootnoterequest">GetFootnoteRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getfootnotesonlinerequest">GetFootnotesOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#footnotesresponse">FootnotesResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#footnotecollection">FootnoteCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getfootnotesrequest">GetFootnotesRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertfootnoteonlinerequest">InsertFootnoteOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertfootnoteonlineresponse">InsertFootnoteOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#footnoteinsert">FootnoteInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertfootnoterequest">InsertFootnoteRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#footnoteresponse">FootnoteResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#footnote">Footnote</a></br><a href="#footnoteinsert">FootnoteInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatefootnoteonlinerequest">UpdateFootnoteOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatefootnoteonlineresponse">UpdateFootnoteOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#footnoteupdate">FootnoteUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatefootnoterequest">UpdateFootnoteRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#footnoteresponse">FootnoteResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#footnote">Footnote</a></br><a href="#footnoteupdate">FootnoteUpdate</a></td>
  </tr>
  </tbody>
</table>


## Footnote

Represents a dTO container with a footnote.

This class is inherited from [FootnoteLink](#footnotelink) and used in [FootnoteCollection](#footnotecollection), [FootnoteResponse](#footnoteresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| Content              | [StoryChildNodes](/words/spec/document#storychildnodes) | Gets or sets the content of the footnote. |
| FootnoteType         | [FootnoteTypeEnum](#footnote.footnotetypeenum) | Gets or sets the value, that specifies whether this is a footnote or endnote. |
| Position             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range start node. |
| ReferenceMark        | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom reference mark to be used for this footnote. Default value is Empty, meaning auto-numbered footnotes are used. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text of the footnote. |


## FootnoteBase

Represents a footnote base class.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FootnoteType         | [FootnoteTypeEnum](#footnote.footnotetypeenum) | Gets or sets the option, that specifies whether this is a footnote or endnote. |
| Position             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range start node. |
| ReferenceMark        | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom reference mark to be used for this footnote. Default value is Empty, meaning auto-numbered footnotes are used. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text of the footnote. |


## FootnoteCollection

Represents a dTO container with a collection of footnotes.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [FootnotesResponse](#footnotesresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| List                 | List&lt;[Footnote](#footnote)&gt;             | Gets or sets the collection of footnotes. |


## FootnoteInsert

Represents a footnote for insert.

This class is inherited from [FootnoteBase](#footnotebase) and used in [InsertFootnoteOnlineRequest](#insertfootnoteonlinerequest), [InsertFootnoteRequest](#insertfootnoterequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FootnoteType         | [FootnoteTypeEnum](#footnote.footnotetypeenum) | Gets or sets the option, that specifies whether this is a footnote or endnote. |
| Position             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range start node. |
| ReferenceMark        | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom reference mark to be used for this footnote. Default value is Empty, meaning auto-numbered footnotes are used. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text of the footnote. |


## FootnoteLink

Represents a footnote link.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |


## FootnoteUpdate

Represents a footnote for update.

This class is inherited from [FootnoteBase](#footnotebase) and used in [UpdateFootnoteOnlineRequest](#updatefootnoteonlinerequest), [UpdateFootnoteRequest](#updatefootnoterequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FootnoteType         | [FootnoteTypeEnum](#footnote.footnotetypeenum) | Gets or sets the option, that specifies whether this is a footnote or endnote. |
| Position             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range start node. |
| ReferenceMark        | <span style="color:SteelBlue;">string</span>  | Gets or sets the custom reference mark to be used for this footnote. Default value is Empty, meaning auto-numbered footnotes are used. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text of the footnote. |


## DeleteFootnoteOnlineRequest

Represents a request model for [WordsApi.DeleteFootnoteOnline()](/words/footnotes/remove/) operation.

An object of the **DeleteFootnoteOnlineRequest** class is created by the following constructor methods:

- DeleteFootnoteOnlineRequest()
- DeleteFootnoteOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

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



## DeleteFootnoteRequest

Represents a request model for [WordsApi.DeleteFootnote()](/words/footnotes/remove/) operation.

An object of the **DeleteFootnoteRequest** class is created by the following constructor methods:

- DeleteFootnoteRequest()
- DeleteFootnoteRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

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



## FootnoteResponse

Represents a REST response with a footnote.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertFootnoteOnlineResponse](#insertfootnoteonlineresponse), [UpdateFootnoteOnlineResponse](#updatefootnoteonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Footnote             | [Footnote](#footnote)                         | Gets or sets the footnote. |


## FootnotesResponse

Represents a REST response with a collection of footnotes.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Footnotes            | [FootnoteCollection](#footnotecollection)     | Gets or sets the collection of footnotes. |


## GetFootnoteOnlineRequest

Represents a request model for [WordsApi.GetFootnoteOnline()](/words/footnotes/get/) operation.

An object of the **GetFootnoteOnlineRequest** class is created by the following constructor methods:

- GetFootnoteOnlineRequest()
- GetFootnoteOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetFootnoteRequest

Represents a request model for [WordsApi.GetFootnote()](/words/footnotes/get/) operation.

An object of the **GetFootnoteRequest** class is created by the following constructor methods:

- GetFootnoteRequest()
- GetFootnoteRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

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



## GetFootnotesOnlineRequest

Represents a request model for [WordsApi.GetFootnotesOnline()](/words/footnotes/get-all/) operation.

An object of the **GetFootnotesOnlineRequest** class is created by the following constructor methods:

- GetFootnotesOnlineRequest()
- GetFootnotesOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetFootnotesRequest

Represents a request model for [WordsApi.GetFootnotes()](/words/footnotes/get-all/) operation.

An object of the **GetFootnotesRequest** class is created by the following constructor methods:

- GetFootnotesRequest()
- GetFootnotesRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## InsertFootnoteOnlineRequest

Represents a request model for [WordsApi.InsertFootnoteOnline()](/words/footnotes/add/) operation.

An object of the **InsertFootnoteOnlineRequest** class is created by the following constructor methods:

- InsertFootnoteOnlineRequest()
- InsertFootnoteOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [FootnoteInsert](#footnoteinsert) ***footnoteDto***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***footnoteDto***    | FootnoteDto          | [FootnoteInsert](#footnoteinsert)             | Footnote data. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertFootnoteOnlineResponse

Represents a response model for [WordsApi.InsertFootnoteOnline()](/words/footnotes/add/) operation.

An object of the **InsertFootnoteOnlineResponse** class is created by the following constructor methods:

- InsertFootnoteOnlineResponse([FootnoteResponse](#footnoteresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [FootnoteResponse](#footnoteresponse)         | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertFootnoteRequest

Represents a request model for [WordsApi.InsertFootnote()](/words/footnotes/add/) operation.

An object of the **InsertFootnoteRequest** class is created by the following constructor methods:

- InsertFootnoteRequest()
- InsertFootnoteRequest(<span style="color:SteelBlue;">string</span> ***name***, [FootnoteInsert](#footnoteinsert) ***footnoteDto***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***footnoteDto***    | FootnoteDto          | [FootnoteInsert](#footnoteinsert)             | Footnote data. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateFootnoteOnlineRequest

Represents a request model for [WordsApi.UpdateFootnoteOnline()](/words/footnotes/update/) operation.

An object of the **UpdateFootnoteOnlineRequest** class is created by the following constructor methods:

- UpdateFootnoteOnlineRequest()
- UpdateFootnoteOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [FootnoteUpdate](#footnoteupdate) ***footnoteDto***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***footnoteDto***    | FootnoteDto          | [FootnoteUpdate](#footnoteupdate)             | Footnote data. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateFootnoteOnlineResponse

Represents a response model for [WordsApi.UpdateFootnoteOnline()](/words/footnotes/update/) operation.

An object of the **UpdateFootnoteOnlineResponse** class is created by the following constructor methods:

- UpdateFootnoteOnlineResponse([FootnoteResponse](#footnoteresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [FootnoteResponse](#footnoteresponse)         | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateFootnoteRequest

Represents a request model for [WordsApi.UpdateFootnote()](/words/footnotes/update/) operation.

An object of the **UpdateFootnoteRequest** class is created by the following constructor methods:

- UpdateFootnoteRequest()
- UpdateFootnoteRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, [FootnoteUpdate](#footnoteupdate) ***footnoteDto***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***footnoteDto***    | FootnoteDto          | [FootnoteUpdate](#footnoteupdate)             | Footnote data. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## Footnote.FootnoteTypeEnum

The following values are defined: Footnote, Endnote.


## FootnoteBase.FootnoteTypeEnum

The following values are defined: Footnote, Endnote.

