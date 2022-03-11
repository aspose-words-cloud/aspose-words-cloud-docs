---
title: "Text"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/text/
description: "Text"
notoc: true
weight: 490
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Replace</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#replacetextonlinerequest">ReplaceTextOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#replacetextonlineresponse">ReplaceTextOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#replacetextparameters">ReplaceTextParameters</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#replacetextrequest">ReplaceTextRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#replacetextresponse">ReplaceTextResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/link#filelink">FileLink</a></br><a href="#replacetextparameters">ReplaceTextParameters</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#replacewithtextonlinerequest">ReplaceWithTextOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#replacewithtextonlineresponse">ReplaceWithTextOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#replacerange">ReplaceRange</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#replacewithtextrequest">ReplaceWithTextRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></br><a href="#replacerange">ReplaceRange</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Search</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#searchonlinerequest">SearchOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#searchresponse">SearchResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#searchresultscollection">SearchResultsCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#searchrequest">SearchRequest</a></td>
  </tr>
  </tbody>
</table>


## ReplaceRange

Represents a dTO container with a range element.

This class is used in [ReplaceWithTextOnlineRequest](#replacewithtextonlinerequest), [ReplaceWithTextRequest](#replacewithtextrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the range's text. |
| TextType             | [TextTypeEnum](/words/spec/range#replacerange.texttypeenum) | Gets or sets the range's text type. |


## ReplaceTextParameters

Represents a class for document replace text request building.

This class is used in [ReplaceTextOnlineRequest](#replacetextonlinerequest), [ReplaceTextRequest](#replacetextrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| IsMatchCase          | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether flag, true means the search is case-sensitive; false means the search is not case-sensitive. |
| IsMatchWholeWord     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether flag, means that only whole word matched are replaced. |
| IsOldValueRegex      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether flag, means that OldValue contains regex expression. |
| NewValue             | <span style="color:SteelBlue;">string</span>  | Gets or sets the new text value to replace by. |
| OldValue             | <span style="color:SteelBlue;">string</span>  | Gets or sets the old text value (or regex pattern IsOldValueRegex) to replace. |


## SearchResult

Represents a result of search operation.

This class is used in [SearchResultsCollection](#searchresultscollection).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RangeEnd             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to result range end node. |
| RangeStart           | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the link to result range start node. |


## SearchResultsCollection

Represents a collection of search results.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [SearchResponse](#searchresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| ResultsList          | List&lt;[SearchResult](#searchresult)&gt;     | Gets or sets the collection of comments. |


## ReplaceTextOnlineRequest

Represents a request model for [WordsApi.ReplaceTextOnline()](/words/text/replace/) operation.

An object of the **ReplaceTextOnlineRequest** class is created by the following constructor methods:

- ReplaceTextOnlineRequest()
- ReplaceTextOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [ReplaceTextParameters](#replacetextparameters) ***replaceText***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***replaceText***    | ReplaceText          | [ReplaceTextParameters](#replacetextparameters) | The replace operation settings. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## ReplaceTextOnlineResponse

Represents a response model for [WordsApi.ReplaceTextOnline()](/words/text/replace/) operation.

An object of the **ReplaceTextOnlineResponse** class is created by the following constructor methods:

- ReplaceTextOnlineResponse([ReplaceTextResponse](#replacetextresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [ReplaceTextResponse](#replacetextresponse)   | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## ReplaceTextRequest

Represents a request model for [WordsApi.ReplaceText()](/words/text/replace/) operation.

An object of the **ReplaceTextRequest** class is created by the following constructor methods:

- ReplaceTextRequest()
- ReplaceTextRequest(<span style="color:SteelBlue;">string</span> ***name***, [ReplaceTextParameters](#replacetextparameters) ***replaceText***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***replaceText***    | ReplaceText          | [ReplaceTextParameters](#replacetextparameters) | The replace operation settings. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## ReplaceTextResponse

Represents a REST response with a number of occurrences of the captured text in the document.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [ReplaceTextOnlineResponse](#replacetextonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| DocumentLink         | [FileLink](/words/spec/link#filelink)         | Gets or sets the link to the document. |
| Matches              | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of occurrences of the captured text in the document. |


## ReplaceWithTextOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **ReplaceWithTextOnlineRequest** class is created by the following constructor methods:

- ReplaceWithTextOnlineRequest()
- ReplaceWithTextOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***rangeStartIdentifier***, [ReplaceRange](#replacerange) ***rangeText***, <span style="color:SteelBlue;">string</span> *rangeEndIdentifier*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***rangeStartIdentifier*** | RangeStartIdentifier | <span style="color:SteelBlue;">string</span>  | The range start identifier. |
| ***rangeText***      | RangeText            | [ReplaceRange](#replacerange)                 | Model with text for replacement. |
| *rangeEndIdentifier* | RangeEndIdentifier   | <span style="color:SteelBlue;">string</span>  | The range end identifier. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## ReplaceWithTextOnlineResponse

Represents a response model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **ReplaceWithTextOnlineResponse** class is created by the following constructor methods:

- ReplaceWithTextOnlineResponse([DocumentResponse](/words/spec/document#documentresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DocumentResponse](/words/spec/document#documentresponse) | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## ReplaceWithTextRequest

Represents a request model for [WordsApi.ReplaceWithText()](/words/range/) operation.

An object of the **ReplaceWithTextRequest** class is created by the following constructor methods:

- ReplaceWithTextRequest()
- ReplaceWithTextRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***rangeStartIdentifier***, [ReplaceRange](#replacerange) ***rangeText***, <span style="color:SteelBlue;">string</span> *rangeEndIdentifier*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***rangeStartIdentifier*** | RangeStartIdentifier | <span style="color:SteelBlue;">string</span>  | The range start identifier. |
| ***rangeText***      | RangeText            | [ReplaceRange](#replacerange)                 | Model with text for replacement. |
| *rangeEndIdentifier* | RangeEndIdentifier   | <span style="color:SteelBlue;">string</span>  | The range end identifier. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## SearchOnlineRequest

Represents a request model for [WordsApi.SearchOnline()](/words/text/search/) operation.

An object of the **SearchOnlineRequest** class is created by the following constructor methods:

- SearchOnlineRequest()
- SearchOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***pattern***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***pattern***        | Pattern              | <span style="color:SteelBlue;">string</span>  | The regular expression used to find matches. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## SearchRequest

Represents a request model for [WordsApi.Search()](/words/text/search/) operation.

An object of the **SearchRequest** class is created by the following constructor methods:

- SearchRequest()
- SearchRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***pattern***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***pattern***        | Pattern              | <span style="color:SteelBlue;">string</span>  | The regular expression used to find matches. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## SearchResponse

Represents a REST response with a regular expression pattern and a collection of search results.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| SearchingPattern     | <span style="color:SteelBlue;">string</span>  | Gets or sets the regular expression pattern used to find matches. |
| SearchResults        | [SearchResultsCollection](#searchresultscollection) | Gets or sets the collection of search results. |

