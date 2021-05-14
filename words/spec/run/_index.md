---
title: "Run"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/run/
description: "Run"
notoc: true
weight: 410
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
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleterunonlinerequest">DeleteRunOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleterunrequest">DeleteRunRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">void</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="6"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getrunfontonlinerequest">GetRunFontOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#fontresponse">FontResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="/words/spec/font#font">Font</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getrunfontrequest">GetRunFontRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getrunonlinerequest">GetRunOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#runresponse">RunResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#run">Run</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getrunrequest">GetRunRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getrunsonlinerequest">GetRunsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#runsresponse">RunsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#runs">Runs</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getrunsrequest">GetRunsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertrunonlinerequest">InsertRunOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertrunonlineresponse">InsertRunOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#runinsert">RunInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertrunrequest">InsertRunRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#runresponse">RunResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#run">Run</a></br><a href="#runinsert">RunInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updaterunfontonlinerequest">UpdateRunFontOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updaterunfontonlineresponse">UpdateRunFontOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="/words/spec/font#font">Font</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updaterunfontrequest">UpdateRunFontRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#fontresponse">FontResponse</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updaterunonlinerequest">UpdateRunOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updaterunonlineresponse">UpdateRunOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#runupdate">RunUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updaterunrequest">UpdateRunRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#runresponse">RunResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#run">Run</a></br><a href="#runupdate">RunUpdate</a></td>
  </tr>
  </tbody>
</table>


## Run

Represents a run element.

This class is inherited from [RunLink](#runlink) and used in [RunResponse](#runresponse), [Runs](#runs).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the run's text. |


## RunBase

Represents a run element.

A single `Text` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the run's text. |


## RunInsert

Represents a run element for insert.

This class is inherited from [RunBase](#runbase) and used in [InsertRunOnlineRequest](#insertrunonlinerequest), [InsertRunRequest](#insertrunrequest).

A single `Text` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the run's text. |


## RunLink

Represents a run link element.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the run's text. |


## Runs

Represents a dTO container with a collection of runs.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [RunsResponse](#runsresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| List                 | List&lt;[Run](#run)&gt;                       | Gets or sets the collection of runs. |


## RunUpdate

Represents a run element for insert.

This class is inherited from [RunBase](#runbase) and used in [UpdateRunOnlineRequest](#updaterunonlinerequest), [UpdateRunRequest](#updaterunrequest).

A single `Text` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the run's text. |


## DeleteRunOnlineRequest

Represents a request model for [WordsApi.DeleteRunOnline()](/words/paragraphs/remove-run/) operation.

An object of the **DeleteRunOnlineRequest** class is created by the following constructor methods:

- DeleteRunOnlineRequest()
- DeleteRunOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteRunRequest

Represents a request model for [WordsApi.DeleteRun()](/words/paragraphs/remove-run/) operation.

An object of the **DeleteRunRequest** class is created by the following constructor methods:

- DeleteRunRequest()
- DeleteRunRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## FontResponse

Represents a REST response with a font.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [UpdateRunFontOnlineResponse](#updaterunfontonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Font                 | [Font](/words/spec/font#font)                 | Gets or sets the font. |


## GetRunFontOnlineRequest

Represents a request model for [WordsApi.GetRunFontOnline()](/words/paragraphs/get-font/) operation.

An object of the **GetRunFontOnlineRequest** class is created by the following constructor methods:

- GetRunFontOnlineRequest()
- GetRunFontOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetRunFontRequest

Represents a request model for [WordsApi.GetRunFont()](/words/paragraphs/get-font/) operation.

An object of the **GetRunFontRequest** class is created by the following constructor methods:

- GetRunFontRequest()
- GetRunFontRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetRunOnlineRequest

Represents a request model for [WordsApi.GetRunOnline()](/words/paragraphs/get-run/) operation.

An object of the **GetRunOnlineRequest** class is created by the following constructor methods:

- GetRunOnlineRequest()
- GetRunOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetRunRequest

Represents a request model for [WordsApi.GetRun()](/words/paragraphs/get-run/) operation.

An object of the **GetRunRequest** class is created by the following constructor methods:

- GetRunRequest()
- GetRunRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetRunsOnlineRequest

Represents a request model for [WordsApi.GetRunsOnline()](/words/paragraphs/get-all-runs/) operation.

An object of the **GetRunsOnlineRequest** class is created by the following constructor methods:

- GetRunsOnlineRequest()
- GetRunsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetRunsRequest

Represents a request model for [WordsApi.GetRuns()](/words/paragraphs/get-all-runs/) operation.

An object of the **GetRunsRequest** class is created by the following constructor methods:

- GetRunsRequest()
- GetRunsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## InsertRunOnlineRequest

Represents a request model for [WordsApi.InsertRunOnline()](/words/paragraphs/add-run/) operation.

An object of the **InsertRunOnlineRequest** class is created by the following constructor methods:

- InsertRunOnlineRequest()
- InsertRunOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, [RunInsert](#runinsert) ***run***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">string</span> *insertBeforeNode*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***run***            | Run                  | [RunInsert](#runinsert)                       | Run data. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *insertBeforeNode*   | InsertBeforeNode     | <span style="color:SteelBlue;">string</span>  | The index of the node. A new Run object will be inserted before the node with the specified node Id. |



## InsertRunOnlineResponse

Represents a response model for [WordsApi.InsertRunOnline()](/words/paragraphs/add-run/) operation.

An object of the **InsertRunOnlineResponse** class is created by the following constructor methods:

- InsertRunOnlineResponse([RunResponse](#runresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [RunResponse](#runresponse)                   | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertRunRequest

Represents a request model for [WordsApi.InsertRun()](/words/paragraphs/add-run/) operation.

An object of the **InsertRunRequest** class is created by the following constructor methods:

- InsertRunRequest()
- InsertRunRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, [RunInsert](#runinsert) ***run***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">string</span> *insertBeforeNode*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***run***            | Run                  | [RunInsert](#runinsert)                       | Run data. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *insertBeforeNode*   | InsertBeforeNode     | <span style="color:SteelBlue;">string</span>  | The index of the node. A new Run object will be inserted before the node with the specified node Id. |



## RunResponse

Represents a REST response with a Run element.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertRunOnlineResponse](#insertrunonlineresponse), [UpdateRunOnlineResponse](#updaterunonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Run                  | [Run](#run)                                   | Gets or sets the Run element. |


## RunsResponse

Represents a REST response with a collection of Run elements.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Runs                 | [Runs](#runs)                                 | Gets or sets the collection of Run elements. |


## UpdateRunFontOnlineRequest

Represents a request model for [WordsApi.UpdateRunFontOnline()](/words/paragraphs/update-font-properties-of-the-text/) operation.

An object of the **UpdateRunFontOnlineRequest** class is created by the following constructor methods:

- UpdateRunFontOnlineRequest()
- UpdateRunFontOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, [Font](/words/spec/font#font) ***fontDto***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***fontDto***        | FontDto              | [Font](/words/spec/font#font)                 | Font dto object. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateRunFontOnlineResponse

Represents a response model for [WordsApi.UpdateRunFontOnline()](/words/paragraphs/update-font-properties-of-the-text/) operation.

An object of the **UpdateRunFontOnlineResponse** class is created by the following constructor methods:

- UpdateRunFontOnlineResponse([FontResponse](#fontresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [FontResponse](#fontresponse)                 | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateRunFontRequest

Represents a request model for [WordsApi.UpdateRunFont()](/words/paragraphs/update-font-properties-of-the-text/) operation.

An object of the **UpdateRunFontRequest** class is created by the following constructor methods:

- UpdateRunFontRequest()
- UpdateRunFontRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">int</span> ***index***, [Font](/words/spec/font#font) ***fontDto***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***fontDto***        | FontDto              | [Font](/words/spec/font#font)                 | Font dto object. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateRunOnlineRequest

Represents a request model for [WordsApi.UpdateRunOnline()](/words/paragraphs/update-run/) operation.

An object of the **UpdateRunOnlineRequest** class is created by the following constructor methods:

- UpdateRunOnlineRequest()
- UpdateRunOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, [RunUpdate](#runupdate) ***run***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***run***            | Run                  | [RunUpdate](#runupdate)                       | Run data. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateRunOnlineResponse

Represents a response model for [WordsApi.UpdateRunOnline()](/words/paragraphs/update-run/) operation.

An object of the **UpdateRunOnlineResponse** class is created by the following constructor methods:

- UpdateRunOnlineResponse([RunResponse](#runresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [RunResponse](#runresponse)                   | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateRunRequest

Represents a request model for [WordsApi.UpdateRun()](/words/paragraphs/update-run/) operation.

An object of the **UpdateRunRequest** class is created by the following constructor methods:

- UpdateRunRequest()
- UpdateRunRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***paragraphPath***, <span style="color:SteelBlue;">int</span> ***index***, [RunUpdate](#runupdate) ***run***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***paragraphPath***  | ParagraphPath        | <span style="color:SteelBlue;">string</span>  | The path to the paragraph in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***run***            | Run                  | [RunUpdate](#runupdate)                       | Run data. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |


