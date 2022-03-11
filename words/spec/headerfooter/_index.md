---
title: "HeaderFooter"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/headerfooter/
description: "HeaderFooter"
notoc: true
weight: 280
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
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteheaderfooteronlinerequest">DeleteHeaderFooterOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteheaderfooterrequest">DeleteHeaderFooterRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteheadersfootersonlinerequest">DeleteHeadersFootersOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteheadersfootersrequest">DeleteHeadersFootersRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="6"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getheaderfooterofsectiononlinerequest">GetHeaderFooterOfSectionOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><a href="#headerfooterresponse">HeaderFooterResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><a href="#headerfooter">HeaderFooter</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getheaderfooterofsectionrequest">GetHeaderFooterOfSectionRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getheaderfooteronlinerequest">GetHeaderFooterOnlineRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getheaderfooterrequest">GetHeaderFooterRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getheaderfootersonlinerequest">GetHeaderFootersOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#headerfootersresponse">HeaderFootersResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#headerfooterlinkcollection">HeaderFooterLinkCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getheaderfootersrequest">GetHeaderFootersRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertheaderfooteronlinerequest">InsertHeaderFooterOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#insertheaderfooteronlineresponse">InsertHeaderFooterOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertheaderfooterrequest">InsertHeaderFooterRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#headerfooterresponse">HeaderFooterResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#headerfooter">HeaderFooter</a></td>
  </tr>
  </tbody>
</table>


## HeaderFooter

Represents a dTO container with a section element.

This class is inherited from [HeaderFooterLink](#headerfooterlink) and used in [HeaderFooterResponse](#headerfooterresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Type                 | [TypeEnum](#headerfooterlink.typeenum)        | Gets or sets the paragraph's text. |
| ChildNodes           | List&lt;[NodeLink](/words/spec/link#nodelink)&gt; | Gets or sets the child nodes. |
| DrawingObjects       | [LinkElement](/words/spec/link#linkelement)   | Gets or sets the link to DrawingObjects resource. |
| Paragraphs           | [LinkElement](/words/spec/link#linkelement)   | Gets or sets the link to Paragraphs resource. |


## HeaderFooterLink

Represents a headerFooter link element.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [HeaderFooterLinkCollection](#headerfooterlinkcollection).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Type                 | [TypeEnum](#headerfooterlink.typeenum)        | Gets or sets the paragraph's text. |


## HeaderFooterLinkCollection

Represents a collection of HeaderFooter's links.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [HeaderFootersResponse](#headerfootersresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| List                 | List&lt;[HeaderFooterLink](#headerfooterlink)&gt; | Gets or sets the collection of HeaderFooter's links. |


## DeleteHeaderFooterOnlineRequest

Represents a request model for [WordsApi.DeleteHeaderFooterOnline()](/words/headers-and-footers/delete/) operation.

An object of the **DeleteHeaderFooterOnlineRequest** class is created by the following constructor methods:

- DeleteHeaderFooterOnlineRequest()
- DeleteHeaderFooterOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***sectionPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***sectionPath***    | SectionPath          | <span style="color:SteelBlue;">string</span>  | The path to the section in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteHeaderFooterRequest

Represents a request model for [WordsApi.DeleteHeaderFooter()](/words/headers-and-footers/delete/) operation.

An object of the **DeleteHeaderFooterRequest** class is created by the following constructor methods:

- DeleteHeaderFooterRequest()
- DeleteHeaderFooterRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***sectionPath***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***sectionPath***    | SectionPath          | <span style="color:SteelBlue;">string</span>  | The path to the section in the document tree. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteHeadersFootersOnlineRequest

Represents a request model for [WordsApi.DeleteHeadersFootersOnline()](/words/headers-and-footers/delete-all/) operation.

An object of the **DeleteHeadersFootersOnlineRequest** class is created by the following constructor methods:

- DeleteHeadersFootersOnlineRequest()
- DeleteHeadersFootersOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***sectionPath***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">string</span> *headersFootersTypes*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***sectionPath***    | SectionPath          | <span style="color:SteelBlue;">string</span>  | The path to the section in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *headersFootersTypes* | HeadersFootersTypes  | <span style="color:SteelBlue;">string</span>  | The list of HeaderFooter types. |



## DeleteHeadersFootersRequest

Represents a request model for [WordsApi.DeleteHeadersFooters()](/words/headers-and-footers/delete-all/) operation.

An object of the **DeleteHeadersFootersRequest** class is created by the following constructor methods:

- DeleteHeadersFootersRequest()
- DeleteHeadersFootersRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***sectionPath***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">string</span> *headersFootersTypes*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***sectionPath***    | SectionPath          | <span style="color:SteelBlue;">string</span>  | The path to the section in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *headersFootersTypes* | HeadersFootersTypes  | <span style="color:SteelBlue;">string</span>  | The list of HeaderFooter types. |



## GetHeaderFooterOfSectionOnlineRequest

Represents a request model for [WordsApi.GetHeaderFooterOfSectionOnline()](/words/headers-and-footers/get/) operation.

An object of the **GetHeaderFooterOfSectionOnlineRequest** class is created by the following constructor methods:

- GetHeaderFooterOfSectionOnlineRequest()
- GetHeaderFooterOfSectionOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***headerFooterIndex***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *filterByType*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***headerFooterIndex*** | HeaderFooterIndex    | <span style="color:SteelBlue;">int</span>     | The index of the HeaderFooter object. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *filterByType*       | FilterByType         | <span style="color:SteelBlue;">string</span>  | The list of HeaderFooter types. |



## GetHeaderFooterOfSectionRequest

Represents a request model for [WordsApi.GetHeaderFooterOfSection()](/words/headers-and-footers/get/) operation.

An object of the **GetHeaderFooterOfSectionRequest** class is created by the following constructor methods:

- GetHeaderFooterOfSectionRequest()
- GetHeaderFooterOfSectionRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***headerFooterIndex***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *filterByType*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***headerFooterIndex*** | HeaderFooterIndex    | <span style="color:SteelBlue;">int</span>     | The index of the HeaderFooter object. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *filterByType*       | FilterByType         | <span style="color:SteelBlue;">string</span>  | The list of HeaderFooter types. |



## GetHeaderFooterOnlineRequest

Represents a request model for [WordsApi.GetHeaderFooterOnline()](/words/headers-and-footers/get/) operation.

An object of the **GetHeaderFooterOnlineRequest** class is created by the following constructor methods:

- GetHeaderFooterOnlineRequest()
- GetHeaderFooterOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***headerFooterIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *filterByType*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***headerFooterIndex*** | HeaderFooterIndex    | <span style="color:SteelBlue;">int</span>     | The index of the HeaderFooter object. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *filterByType*       | FilterByType         | <span style="color:SteelBlue;">string</span>  | The list of HeaderFooter types. |



## GetHeaderFooterRequest

Represents a request model for [WordsApi.GetHeaderFooter()](/words/headers-and-footers/get/) operation.

An object of the **GetHeaderFooterRequest** class is created by the following constructor methods:

- GetHeaderFooterRequest()
- GetHeaderFooterRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***headerFooterIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *filterByType*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***headerFooterIndex*** | HeaderFooterIndex    | <span style="color:SteelBlue;">int</span>     | The index of the HeaderFooter object. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *filterByType*       | FilterByType         | <span style="color:SteelBlue;">string</span>  | The list of HeaderFooter types. |



## GetHeaderFootersOnlineRequest

Represents a request model for [WordsApi.GetHeaderFootersOnline()](/words/headers-and-footers/get-all/) operation.

An object of the **GetHeaderFootersOnlineRequest** class is created by the following constructor methods:

- GetHeaderFootersOnlineRequest()
- GetHeaderFootersOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***sectionPath***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *filterByType*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***sectionPath***    | SectionPath          | <span style="color:SteelBlue;">string</span>  | The path to the section in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *filterByType*       | FilterByType         | <span style="color:SteelBlue;">string</span>  | The list of HeaderFooter types. |



## GetHeaderFootersRequest

Represents a request model for [WordsApi.GetHeaderFooters()](/words/headers-and-footers/get-all/) operation.

An object of the **GetHeaderFootersRequest** class is created by the following constructor methods:

- GetHeaderFootersRequest()
- GetHeaderFootersRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***sectionPath***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *filterByType*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***sectionPath***    | SectionPath          | <span style="color:SteelBlue;">string</span>  | The path to the section in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *filterByType*       | FilterByType         | <span style="color:SteelBlue;">string</span>  | The list of HeaderFooter types. |



## HeaderFooterResponse

Represents a REST response with a HeaderFooter.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertHeaderFooterOnlineResponse](#insertheaderfooteronlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| HeaderFooter         | [HeaderFooter](#headerfooter)                 | Gets or sets the HeaderFooter. |


## HeaderFootersResponse

Represents a REST response with a collection of HeaderFooter elements.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| HeaderFooters        | [HeaderFooterLinkCollection](#headerfooterlinkcollection) | Gets or sets the collection of HeaderFooter elements. |


## InsertHeaderFooterOnlineRequest

Represents a request model for [WordsApi.InsertHeaderFooterOnline()](/words/headers-and-footers/add/) operation.

An object of the **InsertHeaderFooterOnlineRequest** class is created by the following constructor methods:

- InsertHeaderFooterOnlineRequest()
- InsertHeaderFooterOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***sectionPath***, <span style="color:SteelBlue;">string</span> ***headerFooterType***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***sectionPath***    | SectionPath          | <span style="color:SteelBlue;">string</span>  | The path to the section in the document tree. |
| ***headerFooterType*** | HeaderFooterType     | <span style="color:SteelBlue;">string</span>  | Type of header/footer. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertHeaderFooterOnlineResponse

Represents a response model for [WordsApi.InsertHeaderFooterOnline()](/words/headers-and-footers/add/) operation.

An object of the **InsertHeaderFooterOnlineResponse** class is created by the following constructor methods:

- InsertHeaderFooterOnlineResponse([HeaderFooterResponse](#headerfooterresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [HeaderFooterResponse](#headerfooterresponse) | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## InsertHeaderFooterRequest

Represents a request model for [WordsApi.InsertHeaderFooter()](/words/headers-and-footers/add/) operation.

An object of the **InsertHeaderFooterRequest** class is created by the following constructor methods:

- InsertHeaderFooterRequest()
- InsertHeaderFooterRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***sectionPath***, <span style="color:SteelBlue;">string</span> ***headerFooterType***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***sectionPath***    | SectionPath          | <span style="color:SteelBlue;">string</span>  | The path to the section in the document tree. |
| ***headerFooterType*** | HeaderFooterType     | <span style="color:SteelBlue;">string</span>  | Type of header/footer. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## HeaderFooterLink.TypeEnum

The following values are defined: HeaderEven, HeaderPrimary, FooterEven, FooterPrimary, HeaderFirst, FooterFirst.

