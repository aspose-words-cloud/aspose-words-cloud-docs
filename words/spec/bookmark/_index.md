---
title: "Bookmark"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/bookmark/
description: "Bookmark"
notoc: true
weight: 110
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>GetByName</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getbookmarkbynameonlinerequest">GetBookmarkByNameOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#bookmarkresponse">BookmarkResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#bookmark">Bookmark</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getbookmarkbynamerequest">GetBookmarkByNameRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getbookmarksonlinerequest">GetBookmarksOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#bookmarksresponse">BookmarksResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#bookmarks">Bookmarks</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getbookmarksrequest">GetBookmarksRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatebookmarkonlinerequest">UpdateBookmarkOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatebookmarkonlineresponse">UpdateBookmarkOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#bookmarkdata">BookmarkData</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatebookmarkrequest">UpdateBookmarkRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#bookmarkresponse">BookmarkResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#bookmark">Bookmark</a></br><a href="#bookmarkdata">BookmarkData</a></td>
  </tr>
  </tbody>
</table>


## Bookmark

Represents a single bookmark.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [BookmarkResponse](#bookmarkresponse), [Bookmarks](#bookmarks).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the bookmark. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text, enclosed in the bookmark. |


## Bookmarks

Represents a an array of bookmarks.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [BookmarksResponse](#bookmarksresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| BookmarkList         | List&lt;[Bookmark](#bookmark)&gt;             | Gets or sets the array of bookmarks. |


## BookmarkData

Represents a dTO for bookmark updating.

This class is used in [UpdateBookmarkOnlineRequest](#updatebookmarkonlinerequest), [UpdateBookmarkRequest](#updatebookmarkrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the bookmark. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets text, enclosed in the bookmark. |


## BookmarkResponse

Represents a REST response with a bookmark.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [UpdateBookmarkOnlineResponse](#updatebookmarkonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Bookmark             | [Bookmark](#bookmark)                         | Gets or sets the bookmark. |


## BookmarksResponse

Represents a REST response with a collection of bookmarks.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Bookmarks            | [Bookmarks](#bookmarks)                       | Gets or sets the collection of bookmarks. |


## GetBookmarkByNameOnlineRequest

Represents a request model for [WordsApi.GetBookmarkByNameOnline()](/words/bookmarks/read/) operation.

An object of the **GetBookmarkByNameOnlineRequest** class is created by the following constructor methods:

- GetBookmarkByNameOnlineRequest()
- GetBookmarkByNameOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***bookmarkName***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***bookmarkName***   | BookmarkName         | <span style="color:SteelBlue;">string</span>  | The name of the bookmark. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetBookmarkByNameRequest

Represents a request model for [WordsApi.GetBookmarkByName()](/words/bookmarks/read/) operation.

An object of the **GetBookmarkByNameRequest** class is created by the following constructor methods:

- GetBookmarkByNameRequest()
- GetBookmarkByNameRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***bookmarkName***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***bookmarkName***   | BookmarkName         | <span style="color:SteelBlue;">string</span>  | The name of the bookmark. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetBookmarksOnlineRequest

Represents a request model for [WordsApi.GetBookmarksOnline()](/words/bookmarks/get/) operation.

An object of the **GetBookmarksOnlineRequest** class is created by the following constructor methods:

- GetBookmarksOnlineRequest()
- GetBookmarksOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetBookmarksRequest

Represents a request model for [WordsApi.GetBookmarks()](/words/bookmarks/get/) operation.

An object of the **GetBookmarksRequest** class is created by the following constructor methods:

- GetBookmarksRequest()
- GetBookmarksRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## UpdateBookmarkOnlineRequest

Represents a request model for [WordsApi.UpdateBookmarkOnline()](/words/bookmarks/update/) operation.

An object of the **UpdateBookmarkOnlineRequest** class is created by the following constructor methods:

- UpdateBookmarkOnlineRequest()
- UpdateBookmarkOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***bookmarkName***, [BookmarkData](#bookmarkdata) ***bookmarkData***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***bookmarkName***   | BookmarkName         | <span style="color:SteelBlue;">string</span>  | The name of the bookmark. |
| ***bookmarkData***   | BookmarkData         | [BookmarkData](#bookmarkdata)                 | Bookmark data. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateBookmarkOnlineResponse

Represents a response model for [WordsApi.UpdateBookmarkOnline()](/words/bookmarks/update/) operation.

An object of the **UpdateBookmarkOnlineResponse** class is created by the following constructor methods:

- UpdateBookmarkOnlineResponse([BookmarkResponse](#bookmarkresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [BookmarkResponse](#bookmarkresponse)         | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateBookmarkRequest

Represents a request model for [WordsApi.UpdateBookmark()](/words/bookmarks/update/) operation.

An object of the **UpdateBookmarkRequest** class is created by the following constructor methods:

- UpdateBookmarkRequest()
- UpdateBookmarkRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***bookmarkName***, [BookmarkData](#bookmarkdata) ***bookmarkData***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***bookmarkName***   | BookmarkName         | <span style="color:SteelBlue;">string</span>  | The name of the bookmark. |
| ***bookmarkData***   | BookmarkData         | [BookmarkData](#bookmarkdata)                 | Bookmark data. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |


