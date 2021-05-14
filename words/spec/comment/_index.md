---
title: "Comment"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/comment/
description: "Comment"
notoc: true
weight: 130
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
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletecommentonlinerequest">DeleteCommentOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletecommentrequest">DeleteCommentRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">void</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletecommentsonlinerequest">DeleteCommentsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Stream</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletecommentsrequest">DeleteCommentsRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">void</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getcommentonlinerequest">GetCommentOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#commentresponse">CommentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#comment">Comment</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getcommentrequest">GetCommentRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getcommentsonlinerequest">GetCommentsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#commentsresponse">CommentsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#commentscollection">CommentsCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getcommentsrequest">GetCommentsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertcommentonlinerequest">InsertCommentOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertcommentonlineresponse">InsertCommentOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#commentinsert">CommentInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertcommentrequest">InsertCommentRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#commentresponse">CommentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#comment">Comment</a></br><a href="#commentinsert">CommentInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatecommentonlinerequest">UpdateCommentOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatecommentonlineresponse">UpdateCommentOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#commentupdate">CommentUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatecommentrequest">UpdateCommentRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#commentresponse">CommentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#comment">Comment</a></br><a href="#commentupdate">CommentUpdate</a></td>
  </tr>
  </tbody>
</table>


## Comment

Represents a dTO container with a comment.

This class is inherited from [CommentLink](#commentlink) and used in [CommentResponse](#commentresponse), [CommentsCollection](#commentscollection).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Author               | <span style="color:SteelBlue;">string</span>  | Gets or sets the author name for a comment. |
| Content              | [StoryChildNodes](/words/spec/document#storychildnodes) | Gets or sets the content of the comment. |
| DateTime             | <span style="color:SteelBlue;">DateTime</span> | Gets or sets the date and time that the comment was made. |
| Initial              | <span style="color:SteelBlue;">string</span>  | Gets or sets the initials of the user associated with a specific comment. |
| RangeEnd             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range end node. |
| RangeStart           | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range start node. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text of the comment. |


## CommentBase

Represents a comment.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Author               | <span style="color:SteelBlue;">string</span>  | Gets or sets the author name for a comment. |
| DateTime             | <span style="color:SteelBlue;">DateTime</span> | Gets or sets the date and time that the comment was made. |
| Initial              | <span style="color:SteelBlue;">string</span>  | Gets or sets the initials of the user associated with a specific comment. |
| RangeEnd             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range end node. |
| RangeStart           | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range start node. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text of the comment. |


## CommentInsert

Represents a comment insert.

This class is inherited from [CommentBase](#commentbase) and used in [InsertCommentOnlineRequest](#insertcommentonlinerequest), [InsertCommentRequest](#insertcommentrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Author               | <span style="color:SteelBlue;">string</span>  | Gets or sets the author name for a comment. |
| DateTime             | <span style="color:SteelBlue;">DateTime</span> | Gets or sets the date and time that the comment was made. |
| Initial              | <span style="color:SteelBlue;">string</span>  | Gets or sets the initials of the user associated with a specific comment. |
| RangeEnd             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range end node. |
| RangeStart           | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range start node. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text of the comment. |


## CommentLink

Represents a comment link.

A single `Link` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |


## CommentsCollection

Represents a collection of comments.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [CommentsResponse](#commentsresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| CommentList          | List&lt;[Comment](#comment)&gt;               | Gets or sets the collection of comments. |


## CommentUpdate

Represents a comment update.

This class is inherited from [CommentBase](#commentbase) and used in [UpdateCommentOnlineRequest](#updatecommentonlinerequest), [UpdateCommentRequest](#updatecommentrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Author               | <span style="color:SteelBlue;">string</span>  | Gets or sets the author name for a comment. |
| DateTime             | <span style="color:SteelBlue;">DateTime</span> | Gets or sets the date and time that the comment was made. |
| Initial              | <span style="color:SteelBlue;">string</span>  | Gets or sets the initials of the user associated with a specific comment. |
| RangeEnd             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range end node. |
| RangeStart           | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to comment range start node. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text of the comment. |


## CommentResponse

Represents a REST response with a comment.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertCommentOnlineResponse](#insertcommentonlineresponse), [UpdateCommentOnlineResponse](#updatecommentonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Comment              | [Comment](#comment)                           | Gets or sets the comment. |


## CommentsResponse

Represents a REST response with a collection of comments.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Comments             | [CommentsCollection](#commentscollection)     | Gets or sets the collection of comments. |


## DeleteCommentOnlineRequest

Represents a request model for [WordsApi.DeleteCommentOnline()](/words/comments/delete/) operation.

An object of the **DeleteCommentOnlineRequest** class is created by the following constructor methods:

- DeleteCommentOnlineRequest()
- DeleteCommentOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***commentIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***commentIndex***   | CommentIndex         | <span style="color:SteelBlue;">int</span>     | The index of the comment. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteCommentRequest

Represents a request model for [WordsApi.DeleteComment()](/words/comments/delete/) operation.

An object of the **DeleteCommentRequest** class is created by the following constructor methods:

- DeleteCommentRequest()
- DeleteCommentRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***commentIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***commentIndex***   | CommentIndex         | <span style="color:SteelBlue;">int</span>     | The index of the comment. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteCommentsOnlineRequest

Represents a request model for [WordsApi.DeleteCommentsOnline()](/words/comments/delete-all/) operation.

An object of the **DeleteCommentsOnlineRequest** class is created by the following constructor methods:

- DeleteCommentsOnlineRequest()
- DeleteCommentsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteCommentsRequest

Represents a request model for [WordsApi.DeleteComments()](/words/comments/delete-all/) operation.

An object of the **DeleteCommentsRequest** class is created by the following constructor methods:

- DeleteCommentsRequest()
- DeleteCommentsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## GetCommentOnlineRequest

Represents a request model for [WordsApi.GetCommentOnline()](/words/comments/get/) operation.

An object of the **GetCommentOnlineRequest** class is created by the following constructor methods:

- GetCommentOnlineRequest()
- GetCommentOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***commentIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***commentIndex***   | CommentIndex         | <span style="color:SteelBlue;">int</span>     | The index of the comment. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetCommentRequest

Represents a request model for [WordsApi.GetComment()](/words/comments/get/) operation.

An object of the **GetCommentRequest** class is created by the following constructor methods:

- GetCommentRequest()
- GetCommentRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***commentIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***commentIndex***   | CommentIndex         | <span style="color:SteelBlue;">int</span>     | The index of the comment. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetCommentsOnlineRequest

Represents a request model for [WordsApi.GetCommentsOnline()](/words/comments/get-all/) operation.

An object of the **GetCommentsOnlineRequest** class is created by the following constructor methods:

- GetCommentsOnlineRequest()
- GetCommentsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetCommentsRequest

Represents a request model for [WordsApi.GetComments()](/words/comments/get-all/) operation.

An object of the **GetCommentsRequest** class is created by the following constructor methods:

- GetCommentsRequest()
- GetCommentsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## InsertCommentOnlineRequest

Represents a request model for [WordsApi.InsertCommentOnline()](/words/comments/add/) operation.

An object of the **InsertCommentOnlineRequest** class is created by the following constructor methods:

- InsertCommentOnlineRequest()
- InsertCommentOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [CommentInsert](#commentinsert) ***comment***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***comment***        | Comment              | [CommentInsert](#commentinsert)               | Comment data. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertCommentOnlineResponse

Represents a response model for [WordsApi.InsertCommentOnline()](/words/comments/add/) operation.

An object of the **InsertCommentOnlineResponse** class is created by the following constructor methods:

- InsertCommentOnlineResponse([CommentResponse](#commentresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [CommentResponse](#commentresponse)           | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertCommentRequest

Represents a request model for [WordsApi.InsertComment()](/words/comments/add/) operation.

An object of the **InsertCommentRequest** class is created by the following constructor methods:

- InsertCommentRequest()
- InsertCommentRequest(<span style="color:SteelBlue;">string</span> ***name***, [CommentInsert](#commentinsert) ***comment***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***comment***        | Comment              | [CommentInsert](#commentinsert)               | Comment data. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateCommentOnlineRequest

Represents a request model for [WordsApi.UpdateCommentOnline()](/words/comments/update/) operation.

An object of the **UpdateCommentOnlineRequest** class is created by the following constructor methods:

- UpdateCommentOnlineRequest()
- UpdateCommentOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***commentIndex***, [CommentUpdate](#commentupdate) ***comment***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***commentIndex***   | CommentIndex         | <span style="color:SteelBlue;">int</span>     | The index of the comment. |
| ***comment***        | Comment              | [CommentUpdate](#commentupdate)               | Comment data. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateCommentOnlineResponse

Represents a response model for [WordsApi.UpdateCommentOnline()](/words/comments/update/) operation.

An object of the **UpdateCommentOnlineResponse** class is created by the following constructor methods:

- UpdateCommentOnlineResponse([CommentResponse](#commentresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [CommentResponse](#commentresponse)           | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateCommentRequest

Represents a request model for [WordsApi.UpdateComment()](/words/comments/update/) operation.

An object of the **UpdateCommentRequest** class is created by the following constructor methods:

- UpdateCommentRequest()
- UpdateCommentRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***commentIndex***, [CommentUpdate](#commentupdate) ***comment***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***commentIndex***   | CommentIndex         | <span style="color:SteelBlue;">int</span>     | The index of the comment. |
| ***comment***        | Comment              | [CommentUpdate](#commentupdate)               | Comment data. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |


