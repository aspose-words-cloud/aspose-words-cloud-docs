---
title: "Style"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/style/
description: "Style"
notoc: true
weight: 430
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>ApplyStyleTo</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#applystyletodocumentelementonlinerequest">ApplyStyleToDocumentElementOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#applystyletodocumentelementonlineresponse">ApplyStyleToDocumentElementOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#styleapply">StyleApply</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#applystyletodocumentelementrequest">ApplyStyleToDocumentElementRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#wordsresponse">WordsResponse</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Copy</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#copystyleonlinerequest">CopyStyleOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#copystyleonlineresponse">CopyStyleOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#stylecopy">StyleCopy</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#copystylerequest">CopyStyleRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="5"><a href="#styleresponse">StyleResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#style">Style</a></br><a href="#stylecopy">StyleCopy</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="6"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getstylefromdocumentelementonlinerequest">GetStyleFromDocumentElementOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="6"><a href="#style">Style</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getstylefromdocumentelementrequest">GetStyleFromDocumentElementRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getstyleonlinerequest">GetStyleOnlineRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getstylerequest">GetStyleRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getstylesonlinerequest">GetStylesOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#stylesresponse">StylesResponse</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getstylesrequest">GetStylesRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertstyleonlinerequest">InsertStyleOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertstyleonlineresponse">InsertStyleOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#styleinsert">StyleInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertstylerequest">InsertStyleRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#styleresponse">StyleResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#style">Style</a></br><a href="#styleinsert">StyleInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatestyleonlinerequest">UpdateStyleOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatestyleonlineresponse">UpdateStyleOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#styleupdate">StyleUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatestylerequest">UpdateStyleRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#styleresponse">StyleResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#style">Style</a></br><a href="#styleupdate">StyleUpdate</a></td>
  </tr>
  </tbody>
</table>


## Style

Represents a dTO container with a single document style.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [ListInfo](/words/spec/list#listinfo), [ListLevel](/words/spec/list#listlevel), [StyleResponse](#styleresponse), [StylesResponse](#stylesresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Aliases              | List&lt;<span style="color:SteelBlue;">string</span>&gt; | Gets or sets all aliases of this style. If style has no aliases then empty array of string is returned. |
| BaseStyleName        | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the style this style is based on. |
| BuiltIn              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this style is one of the built-in styles in MS Word. |
| Font                 | [Font](/words/spec/font#font)                 | Gets or sets the character formatting of the style. |
| IsHeading            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the style is one of the built-in Heading styles. |
| IsQuickStyle         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this style is shown in the Quick Style gallery inside MS Word UI. |
| LinkedStyleName      | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the Style linked to this one. Returns Empty string if no styles are linked. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the style. |
| NextParagraphStyleName | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the style to be applied automatically to a new paragraph inserted after a paragraph formatted with the specified style. |
| StyleIdentifier      | [StyleIdentifierEnum](#paragraphformatbase.styleidentifierenum) | Gets or sets the locale independent style identifier for a built-in style. |
| Type                 | [TypeEnum](#style.typeenum)                   | Gets or sets the style type (paragraph or character) . |


## XmlColor

Represents a utility class for Color serialization.

This class is used in [Border](/words/spec/border#border), [Font](/words/spec/font#font), [Shading](/words/spec/paragraphformat#shading).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Alpha                | <span style="color:SteelBlue;">int</span>     | Gets or sets the Alpha component of color structure. |
| Web                  | <span style="color:SteelBlue;">string</span>  | Gets or sets the HTML string color representation. |


## StyleApply

Represents a single document style to insert.

This class is used in [ApplyStyleToDocumentElementOnlineRequest](#applystyletodocumentelementonlinerequest), [ApplyStyleToDocumentElementRequest](#applystyletodocumentelementrequest).

A single `StyleName` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| StyleName            | <span style="color:SteelBlue;">string</span>  | Gets or sets the case sensitive name of the style to apply. |


## StyleCopy

Represents a single document style to insert.

This class is used in [CopyStyleOnlineRequest](#copystyleonlinerequest), [CopyStyleRequest](#copystylerequest).

A single `StyleName` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| StyleName            | <span style="color:SteelBlue;">string</span>  | Gets or sets the case sensitive name of the style to copy from it. |


## StyleInsert

Represents a single document style to insert.

This class is used in [InsertStyleOnlineRequest](#insertstyleonlinerequest), [InsertStyleRequest](#insertstylerequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| StyleName            | <span style="color:SteelBlue;">string</span>  | Gets or sets the case sensitive name of the style to create. |
| StyleType            | [StyleTypeEnum](#styleinsert.styletypeenum)   | Gets or sets the StyleType value that specifies the type of the style to create. |


## StyleUpdate

Represents a single document style properties to update.

This class is used in [UpdateStyleOnlineRequest](#updatestyleonlinerequest), [UpdateStyleRequest](#updatestylerequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| BaseStyleName        | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the style this style is based on. |
| IsQuickStyle         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this style is shown in the Quick Style gallery inside MS Word UI. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the style. |
| NextParagraphStyleName | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the style to be applied automatically to a new paragraph inserted after a paragraph formatted with the specified style. |


## StylesResponse

Represents a REST response with an array of styles.

This class is inherited from [WordsResponse](#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Styles               | List&lt;[Style](#style)&gt;                   | Gets or sets the array of styles. |


## ApplyStyleToDocumentElementOnlineRequest

Represents a request model for [WordsApi.ApplyStyleToDocumentElementOnline()](/words/styles/apply/) operation.

An object of the **ApplyStyleToDocumentElementOnlineRequest** class is created by the following constructor methods:

- ApplyStyleToDocumentElementOnlineRequest()
- ApplyStyleToDocumentElementOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***styledNodePath***, [StyleApply](#styleapply) ***styleApply***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***styledNodePath*** | StyledNodePath       | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree, that supports styles: ParagraphFormat, List, ListLevel, Table. |
| ***styleApply***     | StyleApply           | [StyleApply](#styleapply)                     | Style to apply. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## ApplyStyleToDocumentElementOnlineResponse

Represents a response model for [WordsApi.ApplyStyleToDocumentElementOnline()](/words/styles/apply/) operation.

An object of the **ApplyStyleToDocumentElementOnlineResponse** class is created by the following constructor methods:

- ApplyStyleToDocumentElementOnlineResponse([WordsResponse](#wordsresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [WordsResponse](#wordsresponse)               | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## ApplyStyleToDocumentElementRequest

Represents a request model for [WordsApi.ApplyStyleToDocumentElement()](/words/styles/apply/) operation.

An object of the **ApplyStyleToDocumentElementRequest** class is created by the following constructor methods:

- ApplyStyleToDocumentElementRequest()
- ApplyStyleToDocumentElementRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***styledNodePath***, [StyleApply](#styleapply) ***styleApply***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***styledNodePath*** | StyledNodePath       | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree, that supports styles: ParagraphFormat, List, ListLevel, Table. |
| ***styleApply***     | StyleApply           | [StyleApply](#styleapply)                     | Style to apply. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## CopyStyleOnlineRequest

Represents a request model for [WordsApi.CopyStyleOnline()](/words/styles/copy/) operation.

An object of the **CopyStyleOnlineRequest** class is created by the following constructor methods:

- CopyStyleOnlineRequest()
- CopyStyleOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [StyleCopy](#stylecopy) ***styleCopy***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***styleCopy***      | StyleCopy            | [StyleCopy](#stylecopy)                       | Style to copy. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## CopyStyleOnlineResponse

Represents a response model for [WordsApi.CopyStyleOnline()](/words/styles/copy/) operation.

An object of the **CopyStyleOnlineResponse** class is created by the following constructor methods:

- CopyStyleOnlineResponse([StyleResponse](#styleresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [StyleResponse](#styleresponse)               | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## CopyStyleRequest

Represents a request model for [WordsApi.CopyStyle()](/words/styles/copy/) operation.

An object of the **CopyStyleRequest** class is created by the following constructor methods:

- CopyStyleRequest()
- CopyStyleRequest(<span style="color:SteelBlue;">string</span> ***name***, [StyleCopy](#stylecopy) ***styleCopy***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***styleCopy***      | StyleCopy            | [StyleCopy](#stylecopy)                       | Style to copy. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## GetStyleFromDocumentElementOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **GetStyleFromDocumentElementOnlineRequest** class is created by the following constructor methods:

- GetStyleFromDocumentElementOnlineRequest()
- GetStyleFromDocumentElementOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***styledNodePath***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***styledNodePath*** | StyledNodePath       | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree, that supports styles: ParagraphFormat, List, ListLevel, Table. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetStyleFromDocumentElementRequest

Represents a request model for [WordsApi.GetStyleFromDocumentElement()](/words/styles/get/) operation.

An object of the **GetStyleFromDocumentElementRequest** class is created by the following constructor methods:

- GetStyleFromDocumentElementRequest()
- GetStyleFromDocumentElementRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***styledNodePath***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***styledNodePath*** | StyledNodePath       | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree, that supports styles: ParagraphFormat, List, ListLevel, Table. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetStyleOnlineRequest

Represents a request model for [WordsApi.GetStyleOnline()](/words/styles/get/) operation.

An object of the **GetStyleOnlineRequest** class is created by the following constructor methods:

- GetStyleOnlineRequest()
- GetStyleOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***styleName***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***styleName***      | StyleName            | <span style="color:SteelBlue;">string</span>  | The name of the style. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetStyleRequest

Represents a request model for [WordsApi.GetStyle()](/words/styles/get/) operation.

An object of the **GetStyleRequest** class is created by the following constructor methods:

- GetStyleRequest()
- GetStyleRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***styleName***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***styleName***      | StyleName            | <span style="color:SteelBlue;">string</span>  | The name of the style. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetStylesOnlineRequest

Represents a request model for [WordsApi.GetStylesOnline()](/words/styles/get-all/) operation.

An object of the **GetStylesOnlineRequest** class is created by the following constructor methods:

- GetStylesOnlineRequest()
- GetStylesOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetStylesRequest

Represents a request model for [WordsApi.GetStyles()](/words/styles/get-all/) operation.

An object of the **GetStylesRequest** class is created by the following constructor methods:

- GetStylesRequest()
- GetStylesRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## InsertStyleOnlineRequest

Represents a request model for [WordsApi.InsertStyleOnline()](/words/styles/insert/) operation.

An object of the **InsertStyleOnlineRequest** class is created by the following constructor methods:

- InsertStyleOnlineRequest()
- InsertStyleOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [StyleInsert](#styleinsert) ***styleInsert***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***styleInsert***    | StyleInsert          | [StyleInsert](#styleinsert)                   | Style to insert. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertStyleOnlineResponse

Represents a response model for [WordsApi.InsertStyleOnline()](/words/styles/insert/) operation.

An object of the **InsertStyleOnlineResponse** class is created by the following constructor methods:

- InsertStyleOnlineResponse([StyleResponse](#styleresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [StyleResponse](#styleresponse)               | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertStyleRequest

Represents a request model for [WordsApi.InsertStyle()](/words/styles/insert/) operation.

An object of the **InsertStyleRequest** class is created by the following constructor methods:

- InsertStyleRequest()
- InsertStyleRequest(<span style="color:SteelBlue;">string</span> ***name***, [StyleInsert](#styleinsert) ***styleInsert***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***styleInsert***    | StyleInsert          | [StyleInsert](#styleinsert)                   | Style to insert. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## StyleResponse

Represents a REST response with a style.

This class is inherited from [WordsResponse](#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [CopyStyleOnlineResponse](#copystyleonlineresponse), [InsertStyleOnlineResponse](#insertstyleonlineresponse), [UpdateStyleOnlineResponse](#updatestyleonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Style                | [Style](#style)                               | Gets or sets the style, containded in the document. |


## UpdateStyleOnlineRequest

Represents a request model for [WordsApi.UpdateStyleOnline()](/words/styles/update/) operation.

An object of the **UpdateStyleOnlineRequest** class is created by the following constructor methods:

- UpdateStyleOnlineRequest()
- UpdateStyleOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***styleName***, [StyleUpdate](#styleupdate) ***styleUpdate***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***styleName***      | StyleName            | <span style="color:SteelBlue;">string</span>  | The name of the style. |
| ***styleUpdate***    | StyleUpdate          | [StyleUpdate](#styleupdate)                   | Style properties to update. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateStyleOnlineResponse

Represents a response model for [WordsApi.UpdateStyleOnline()](/words/styles/update/) operation.

An object of the **UpdateStyleOnlineResponse** class is created by the following constructor methods:

- UpdateStyleOnlineResponse([StyleResponse](#styleresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [StyleResponse](#styleresponse)               | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateStyleRequest

Represents a request model for [WordsApi.UpdateStyle()](/words/styles/update/) operation.

An object of the **UpdateStyleRequest** class is created by the following constructor methods:

- UpdateStyleRequest()
- UpdateStyleRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***styleName***, [StyleUpdate](#styleupdate) ***styleUpdate***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***styleName***      | StyleName            | <span style="color:SteelBlue;">string</span>  | The name of the style. |
| ***styleUpdate***    | StyleUpdate          | [StyleUpdate](#styleupdate)                   | Style properties to update. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## WordsResponse

Represents a base class for all responses.

This class is used in [WordsApi](/words/spec/wordsapi#wordsapi), [ApplyStyleToDocumentElementOnlineResponse](#applystyletodocumentelementonlineresponse).

A single `RequestId` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |


## ParagraphFormatBase.StyleIdentifierEnum

The following values are defined: Normal, Heading1, Heading2, Heading3, Heading4, Heading5, Heading6, Heading7, Heading8, Heading9, Index1, Index2, Index3, Index4, Index5, Index6, Index7, Index8, Index9, Toc1, Toc2, Toc3, Toc4, Toc5, Toc6, Toc7, Toc8, Toc9, NormalIndent, FootnoteText, CommentText, Header, Footer, IndexHeading, Caption, TableOfFigures, EnvelopeAddress, EnvelopeReturn, FootnoteReference, CommentReference, LineNumber, PageNumber, EndnoteReference, EndnoteText, TableOfAuthorities, Macro, ToaHeading, List, ListBullet, ListNumber, List2, List3, List4, List5, ListBullet2, ListBullet3, ListBullet4, ListBullet5, ListNumber2, ListNumber3, ListNumber4, ListNumber5, Title, Closing, Signature, DefaultParagraphFont, BodyText, BodyTextInd, ListContinue, ListContinue2, ListContinue3, ListContinue4, ListContinue5, MessageHeader, Subtitle, Salutation, Date, BodyText1I, BodyText1I2, NoteHeading, BodyText2, BodyText3, BodyTextInd2, BodyTextInd3, BlockText, Hyperlink, FollowedHyperlink, Strong, Emphasis, DocumentMap, PlainText, EmailSignature, HtmlTopOfForm, HtmlBottomOfForm, NormalWeb, HtmlAcronym, HtmlAddress, HtmlCite, HtmlCode, HtmlDefinition, HtmlKeyboard, HtmlPreformatted, HtmlSample, HtmlTypewriter, HtmlVariable, TableNormal, CommentSubject, NoList, OutlineList1, OutlineList2, OutlineList3, TableSimple1, TableSimple2, TableSimple3, TableClassic1, TableClassic2, TableClassic3, TableClassic4, TableColorful1, TableColorful2, TableColorful3, TableColumns1, TableColumns2, TableColumns3, TableColumns4, TableColumns5, TableGrid1, TableGrid2, TableGrid3, TableGrid4, TableGrid5, TableGrid6, TableGrid7, TableGrid8, TableList1, TableList2, TableList3, TableList4, TableList5, TableList6, TableList7, TableList8, Table3DEffects1, Table3DEffects2, Table3DEffects3, TableContemporary, TableElegant, TableProfessional, TableSubtle1, TableSubtle2, TableWeb1, TableWeb2, TableWeb3, BalloonText, TableGrid, TableTheme, PlaceholderText, NoSpacing, LightShading, LightList, LightGrid, MediumShading1, MediumShading2, MediumList1, MediumList2, MediumGrid1, MediumGrid2, MediumGrid3, DarkList, ColorfulShading, ColorfulList, ColorfulGrid, LightShadingAccent1, LightListAccent1, LightGridAccent1, MediumShading1Accent1, MediumShading2Accent1, MediumList1Accent1, Revision, ListParagraph, Quote, IntenseQuote, MediumList2Accent1, MediumGrid1Accent1, MediumGrid2Accent1, MediumGrid3Accent1, DarkListAccent1, ColorfulShadingAccent1, ColorfulListAccent1, ColorfulGridAccent1, LightShadingAccent2, LightListAccent2, LightGridAccent2, MediumShading1Accent2, MediumShading2Accent2, MediumList1Accent2, MediumList2Accent2, MediumGrid1Accent2, MediumGrid2Accent2, MediumGrid3Accent2, DarkListAccent2, ColorfulShadingAccent2, ColorfulListAccent2, ColorfulGridAccent2, LightShadingAccent3, LightListAccent3, LightGridAccent3, MediumShading1Accent3, MediumShading2Accent3, MediumList1Accent3, MediumList2Accent3, MediumGrid1Accent3, MediumGrid2Accent3, MediumGrid3Accent3, DarkListAccent3, ColorfulShadingAccent3, ColorfulListAccent3, ColorfulGridAccent3, LightShadingAccent4, LightListAccent4, LightGridAccent4, MediumShading1Accent4, MediumShading2Accent4, MediumList1Accent4, MediumList2Accent4, MediumGrid1Accent4, MediumGrid2Accent4, MediumGrid3Accent4, DarkListAccent4, ColorfulShadingAccent4, ColorfulListAccent4, ColorfulGridAccent4, LightShadingAccent5, LightListAccent5, LightGridAccent5, MediumShading1Accent5, MediumShading2Accent5, MediumList1Accent5, MediumList2Accent5, MediumGrid1Accent5, MediumGrid2Accent5, MediumGrid3Accent5, DarkListAccent5, ColorfulShadingAccent5, ColorfulListAccent5, ColorfulGridAccent5, LightShadingAccent6, LightListAccent6, LightGridAccent6, MediumShading1Accent6, MediumShading2Accent6, MediumList1Accent6, MediumList2Accent6, MediumGrid1Accent6, MediumGrid2Accent6, MediumGrid3Accent6, DarkListAccent6, ColorfulShadingAccent6, ColorfulListAccent6, ColorfulGridAccent6, SubtleEmphasis, IntenseEmphasis, SubtleReference, IntenseReference, BookTitle, Bibliography, TocHeading, PlainTable1, PlainTable2, PlainTable3, PlainTable4, PlainTable5, TableGridLight, GridTable1Light, GridTable2, GridTable3, GridTable4, GridTable5Dark, GridTable6Colorful, GridTable7Colorful, GridTable1LightAccent1, GridTable2Accent1, GridTable3Accent1, GridTable4Accent1, GridTable5DarkAccent1, GridTable6ColorfulAccent1, GridTable7ColorfulAccent1, GridTable1LightAccent2, GridTable2Accent2, GridTable3Accent2, GridTable4Accent2, GridTable5DarkAccent2, GridTable6ColorfulAccent2, GridTable7ColorfulAccent2, GridTable1LightAccent3, GridTable2Accent3, GridTable3Accent3, GridTable4Accent3, GridTable5DarkAccent3, GridTable6ColorfulAccent3, GridTable7ColorfulAccent3, GridTable1LightAccent4, GridTable2Accent4, GridTable3Accent4, GridTable4Accent4, GridTable5DarkAccent4, GridTable6ColorfulAccent4, GridTable7ColorfulAccent4, GridTable1LightAccent5, GridTable2Accent5, GridTable3Accent5, GridTable4Accent5, GridTable5DarkAccent5, GridTable6ColorfulAccent5, GridTable7ColorfulAccent5, GridTable1LightAccent6, GridTable2Accent6, GridTable3Accent6, GridTable4Accent6, GridTable5DarkAccent6, GridTable6ColorfulAccent6, GridTable7ColorfulAccent6, ListTable1Light, ListTable2, ListTable3, ListTable4, ListTable5Dark, ListTable6Colorful, ListTable7Colorful, ListTable1LightAccent1, ListTable2Accent1, ListTable3Accent1, ListTable4Accent1, ListTable5DarkAccent1, ListTable6ColorfulAccent1, ListTable7ColorfulAccent1, ListTable1LightAccent2, ListTable2Accent2, ListTable3Accent2, ListTable4Accent2, ListTable5DarkAccent2, ListTable6ColorfulAccent2, ListTable7ColorfulAccent2, ListTable1LightAccent3, ListTable2Accent3, ListTable3Accent3, ListTable4Accent3, ListTable5DarkAccent3, ListTable6ColorfulAccent3, ListTable7ColorfulAccent3, ListTable1LightAccent4, ListTable2Accent4, ListTable3Accent4, ListTable4Accent4, ListTable5DarkAccent4, ListTable6ColorfulAccent4, ListTable7ColorfulAccent4, ListTable1LightAccent5, ListTable2Accent5, ListTable3Accent5, ListTable4Accent5, ListTable5DarkAccent5, ListTable6ColorfulAccent5, ListTable7ColorfulAccent5, ListTable1LightAccent6, ListTable2Accent6, ListTable3Accent6, ListTable4Accent6, ListTable5DarkAccent6, ListTable6ColorfulAccent6, ListTable7ColorfulAccent6, SmartLink, User, Nil.


## Shading.TextureEnum

The following values are defined: TextureNone, TextureSolid, Texture5Percent, Texture10Percent, Texture20Percent, Texture25Percent, Texture30Percent, Texture40Percent, Texture50Percent, Texture60Percent, Texture70Percent, Texture75Percent, Texture80Percent, Texture90Percent, TextureDarkHorizontal, TextureDarkVertical, TextureDarkDiagonalDown, TextureDarkDiagonalUp, TextureDarkCross, TextureDarkDiagonalCross, TextureHorizontal, TextureVertical, TextureDiagonalDown, TextureDiagonalUp, TextureCross, TextureDiagonalCross, Texture2Pt5Percent, Texture7Pt5Percent, Texture12Pt5Percent, Texture15Percent, Texture17Pt5Percent, Texture22Pt5Percent, Texture27Pt5Percent, Texture32Pt5Percent, Texture35Percent, Texture37Pt5Percent, Texture42Pt5Percent, Texture45Percent, Texture47Pt5Percent, Texture52Pt5Percent, Texture55Percent, Texture57Pt5Percent, Texture62Pt5Percent, Texture65Percent, Texture67Pt5Percent, Texture72Pt5Percent, Texture77Pt5Percent, Texture82Pt5Percent, Texture85Percent, Texture87Pt5Percent, Texture92Pt5Percent, Texture95Percent, Texture97Pt5Percent, TextureNil.


## Style.StyleIdentifierEnum

The following values are defined: Normal, Heading1, Heading2, Heading3, Heading4, Heading5, Heading6, Heading7, Heading8, Heading9, Index1, Index2, Index3, Index4, Index5, Index6, Index7, Index8, Index9, Toc1, Toc2, Toc3, Toc4, Toc5, Toc6, Toc7, Toc8, Toc9, NormalIndent, FootnoteText, CommentText, Header, Footer, IndexHeading, Caption, TableOfFigures, EnvelopeAddress, EnvelopeReturn, FootnoteReference, CommentReference, LineNumber, PageNumber, EndnoteReference, EndnoteText, TableOfAuthorities, Macro, ToaHeading, List, ListBullet, ListNumber, List2, List3, List4, List5, ListBullet2, ListBullet3, ListBullet4, ListBullet5, ListNumber2, ListNumber3, ListNumber4, ListNumber5, Title, Closing, Signature, DefaultParagraphFont, BodyText, BodyTextInd, ListContinue, ListContinue2, ListContinue3, ListContinue4, ListContinue5, MessageHeader, Subtitle, Salutation, Date, BodyText1I, BodyText1I2, NoteHeading, BodyText2, BodyText3, BodyTextInd2, BodyTextInd3, BlockText, Hyperlink, FollowedHyperlink, Strong, Emphasis, DocumentMap, PlainText, EmailSignature, HtmlTopOfForm, HtmlBottomOfForm, NormalWeb, HtmlAcronym, HtmlAddress, HtmlCite, HtmlCode, HtmlDefinition, HtmlKeyboard, HtmlPreformatted, HtmlSample, HtmlTypewriter, HtmlVariable, TableNormal, CommentSubject, NoList, OutlineList1, OutlineList2, OutlineList3, TableSimple1, TableSimple2, TableSimple3, TableClassic1, TableClassic2, TableClassic3, TableClassic4, TableColorful1, TableColorful2, TableColorful3, TableColumns1, TableColumns2, TableColumns3, TableColumns4, TableColumns5, TableGrid1, TableGrid2, TableGrid3, TableGrid4, TableGrid5, TableGrid6, TableGrid7, TableGrid8, TableList1, TableList2, TableList3, TableList4, TableList5, TableList6, TableList7, TableList8, Table3DEffects1, Table3DEffects2, Table3DEffects3, TableContemporary, TableElegant, TableProfessional, TableSubtle1, TableSubtle2, TableWeb1, TableWeb2, TableWeb3, BalloonText, TableGrid, TableTheme, PlaceholderText, NoSpacing, LightShading, LightList, LightGrid, MediumShading1, MediumShading2, MediumList1, MediumList2, MediumGrid1, MediumGrid2, MediumGrid3, DarkList, ColorfulShading, ColorfulList, ColorfulGrid, LightShadingAccent1, LightListAccent1, LightGridAccent1, MediumShading1Accent1, MediumShading2Accent1, MediumList1Accent1, Revision, ListParagraph, Quote, IntenseQuote, MediumList2Accent1, MediumGrid1Accent1, MediumGrid2Accent1, MediumGrid3Accent1, DarkListAccent1, ColorfulShadingAccent1, ColorfulListAccent1, ColorfulGridAccent1, LightShadingAccent2, LightListAccent2, LightGridAccent2, MediumShading1Accent2, MediumShading2Accent2, MediumList1Accent2, MediumList2Accent2, MediumGrid1Accent2, MediumGrid2Accent2, MediumGrid3Accent2, DarkListAccent2, ColorfulShadingAccent2, ColorfulListAccent2, ColorfulGridAccent2, LightShadingAccent3, LightListAccent3, LightGridAccent3, MediumShading1Accent3, MediumShading2Accent3, MediumList1Accent3, MediumList2Accent3, MediumGrid1Accent3, MediumGrid2Accent3, MediumGrid3Accent3, DarkListAccent3, ColorfulShadingAccent3, ColorfulListAccent3, ColorfulGridAccent3, LightShadingAccent4, LightListAccent4, LightGridAccent4, MediumShading1Accent4, MediumShading2Accent4, MediumList1Accent4, MediumList2Accent4, MediumGrid1Accent4, MediumGrid2Accent4, MediumGrid3Accent4, DarkListAccent4, ColorfulShadingAccent4, ColorfulListAccent4, ColorfulGridAccent4, LightShadingAccent5, LightListAccent5, LightGridAccent5, MediumShading1Accent5, MediumShading2Accent5, MediumList1Accent5, MediumList2Accent5, MediumGrid1Accent5, MediumGrid2Accent5, MediumGrid3Accent5, DarkListAccent5, ColorfulShadingAccent5, ColorfulListAccent5, ColorfulGridAccent5, LightShadingAccent6, LightListAccent6, LightGridAccent6, MediumShading1Accent6, MediumShading2Accent6, MediumList1Accent6, MediumList2Accent6, MediumGrid1Accent6, MediumGrid2Accent6, MediumGrid3Accent6, DarkListAccent6, ColorfulShadingAccent6, ColorfulListAccent6, ColorfulGridAccent6, SubtleEmphasis, IntenseEmphasis, SubtleReference, IntenseReference, BookTitle, Bibliography, TocHeading, PlainTable1, PlainTable2, PlainTable3, PlainTable4, PlainTable5, TableGridLight, GridTable1Light, GridTable2, GridTable3, GridTable4, GridTable5Dark, GridTable6Colorful, GridTable7Colorful, GridTable1LightAccent1, GridTable2Accent1, GridTable3Accent1, GridTable4Accent1, GridTable5DarkAccent1, GridTable6ColorfulAccent1, GridTable7ColorfulAccent1, GridTable1LightAccent2, GridTable2Accent2, GridTable3Accent2, GridTable4Accent2, GridTable5DarkAccent2, GridTable6ColorfulAccent2, GridTable7ColorfulAccent2, GridTable1LightAccent3, GridTable2Accent3, GridTable3Accent3, GridTable4Accent3, GridTable5DarkAccent3, GridTable6ColorfulAccent3, GridTable7ColorfulAccent3, GridTable1LightAccent4, GridTable2Accent4, GridTable3Accent4, GridTable4Accent4, GridTable5DarkAccent4, GridTable6ColorfulAccent4, GridTable7ColorfulAccent4, GridTable1LightAccent5, GridTable2Accent5, GridTable3Accent5, GridTable4Accent5, GridTable5DarkAccent5, GridTable6ColorfulAccent5, GridTable7ColorfulAccent5, GridTable1LightAccent6, GridTable2Accent6, GridTable3Accent6, GridTable4Accent6, GridTable5DarkAccent6, GridTable6ColorfulAccent6, GridTable7ColorfulAccent6, ListTable1Light, ListTable2, ListTable3, ListTable4, ListTable5Dark, ListTable6Colorful, ListTable7Colorful, ListTable1LightAccent1, ListTable2Accent1, ListTable3Accent1, ListTable4Accent1, ListTable5DarkAccent1, ListTable6ColorfulAccent1, ListTable7ColorfulAccent1, ListTable1LightAccent2, ListTable2Accent2, ListTable3Accent2, ListTable4Accent2, ListTable5DarkAccent2, ListTable6ColorfulAccent2, ListTable7ColorfulAccent2, ListTable1LightAccent3, ListTable2Accent3, ListTable3Accent3, ListTable4Accent3, ListTable5DarkAccent3, ListTable6ColorfulAccent3, ListTable7ColorfulAccent3, ListTable1LightAccent4, ListTable2Accent4, ListTable3Accent4, ListTable4Accent4, ListTable5DarkAccent4, ListTable6ColorfulAccent4, ListTable7ColorfulAccent4, ListTable1LightAccent5, ListTable2Accent5, ListTable3Accent5, ListTable4Accent5, ListTable5DarkAccent5, ListTable6ColorfulAccent5, ListTable7ColorfulAccent5, ListTable1LightAccent6, ListTable2Accent6, ListTable3Accent6, ListTable4Accent6, ListTable5DarkAccent6, ListTable6ColorfulAccent6, ListTable7ColorfulAccent6, SmartLink, User, Nil.


## Style.TypeEnum

The following values are defined: Paragraph, Character, Table, List.


## StyleInsert.StyleTypeEnum

The following values are defined: Paragraph, Character, Table, List.


## TableProperties.StyleIdentifierEnum

The following values are defined: Normal, Heading1, Heading2, Heading3, Heading4, Heading5, Heading6, Heading7, Heading8, Heading9, Index1, Index2, Index3, Index4, Index5, Index6, Index7, Index8, Index9, Toc1, Toc2, Toc3, Toc4, Toc5, Toc6, Toc7, Toc8, Toc9, NormalIndent, FootnoteText, CommentText, Header, Footer, IndexHeading, Caption, TableOfFigures, EnvelopeAddress, EnvelopeReturn, FootnoteReference, CommentReference, LineNumber, PageNumber, EndnoteReference, EndnoteText, TableOfAuthorities, Macro, ToaHeading, List, ListBullet, ListNumber, List2, List3, List4, List5, ListBullet2, ListBullet3, ListBullet4, ListBullet5, ListNumber2, ListNumber3, ListNumber4, ListNumber5, Title, Closing, Signature, DefaultParagraphFont, BodyText, BodyTextInd, ListContinue, ListContinue2, ListContinue3, ListContinue4, ListContinue5, MessageHeader, Subtitle, Salutation, Date, BodyText1I, BodyText1I2, NoteHeading, BodyText2, BodyText3, BodyTextInd2, BodyTextInd3, BlockText, Hyperlink, FollowedHyperlink, Strong, Emphasis, DocumentMap, PlainText, EmailSignature, HtmlTopOfForm, HtmlBottomOfForm, NormalWeb, HtmlAcronym, HtmlAddress, HtmlCite, HtmlCode, HtmlDefinition, HtmlKeyboard, HtmlPreformatted, HtmlSample, HtmlTypewriter, HtmlVariable, TableNormal, CommentSubject, NoList, OutlineList1, OutlineList2, OutlineList3, TableSimple1, TableSimple2, TableSimple3, TableClassic1, TableClassic2, TableClassic3, TableClassic4, TableColorful1, TableColorful2, TableColorful3, TableColumns1, TableColumns2, TableColumns3, TableColumns4, TableColumns5, TableGrid1, TableGrid2, TableGrid3, TableGrid4, TableGrid5, TableGrid6, TableGrid7, TableGrid8, TableList1, TableList2, TableList3, TableList4, TableList5, TableList6, TableList7, TableList8, Table3DEffects1, Table3DEffects2, Table3DEffects3, TableContemporary, TableElegant, TableProfessional, TableSubtle1, TableSubtle2, TableWeb1, TableWeb2, TableWeb3, BalloonText, TableGrid, TableTheme, PlaceholderText, NoSpacing, LightShading, LightList, LightGrid, MediumShading1, MediumShading2, MediumList1, MediumList2, MediumGrid1, MediumGrid2, MediumGrid3, DarkList, ColorfulShading, ColorfulList, ColorfulGrid, LightShadingAccent1, LightListAccent1, LightGridAccent1, MediumShading1Accent1, MediumShading2Accent1, MediumList1Accent1, Revision, ListParagraph, Quote, IntenseQuote, MediumList2Accent1, MediumGrid1Accent1, MediumGrid2Accent1, MediumGrid3Accent1, DarkListAccent1, ColorfulShadingAccent1, ColorfulListAccent1, ColorfulGridAccent1, LightShadingAccent2, LightListAccent2, LightGridAccent2, MediumShading1Accent2, MediumShading2Accent2, MediumList1Accent2, MediumList2Accent2, MediumGrid1Accent2, MediumGrid2Accent2, MediumGrid3Accent2, DarkListAccent2, ColorfulShadingAccent2, ColorfulListAccent2, ColorfulGridAccent2, LightShadingAccent3, LightListAccent3, LightGridAccent3, MediumShading1Accent3, MediumShading2Accent3, MediumList1Accent3, MediumList2Accent3, MediumGrid1Accent3, MediumGrid2Accent3, MediumGrid3Accent3, DarkListAccent3, ColorfulShadingAccent3, ColorfulListAccent3, ColorfulGridAccent3, LightShadingAccent4, LightListAccent4, LightGridAccent4, MediumShading1Accent4, MediumShading2Accent4, MediumList1Accent4, MediumList2Accent4, MediumGrid1Accent4, MediumGrid2Accent4, MediumGrid3Accent4, DarkListAccent4, ColorfulShadingAccent4, ColorfulListAccent4, ColorfulGridAccent4, LightShadingAccent5, LightListAccent5, LightGridAccent5, MediumShading1Accent5, MediumShading2Accent5, MediumList1Accent5, MediumList2Accent5, MediumGrid1Accent5, MediumGrid2Accent5, MediumGrid3Accent5, DarkListAccent5, ColorfulShadingAccent5, ColorfulListAccent5, ColorfulGridAccent5, LightShadingAccent6, LightListAccent6, LightGridAccent6, MediumShading1Accent6, MediumShading2Accent6, MediumList1Accent6, MediumList2Accent6, MediumGrid1Accent6, MediumGrid2Accent6, MediumGrid3Accent6, DarkListAccent6, ColorfulShadingAccent6, ColorfulListAccent6, ColorfulGridAccent6, SubtleEmphasis, IntenseEmphasis, SubtleReference, IntenseReference, BookTitle, Bibliography, TocHeading, PlainTable1, PlainTable2, PlainTable3, PlainTable4, PlainTable5, TableGridLight, GridTable1Light, GridTable2, GridTable3, GridTable4, GridTable5Dark, GridTable6Colorful, GridTable7Colorful, GridTable1LightAccent1, GridTable2Accent1, GridTable3Accent1, GridTable4Accent1, GridTable5DarkAccent1, GridTable6ColorfulAccent1, GridTable7ColorfulAccent1, GridTable1LightAccent2, GridTable2Accent2, GridTable3Accent2, GridTable4Accent2, GridTable5DarkAccent2, GridTable6ColorfulAccent2, GridTable7ColorfulAccent2, GridTable1LightAccent3, GridTable2Accent3, GridTable3Accent3, GridTable4Accent3, GridTable5DarkAccent3, GridTable6ColorfulAccent3, GridTable7ColorfulAccent3, GridTable1LightAccent4, GridTable2Accent4, GridTable3Accent4, GridTable4Accent4, GridTable5DarkAccent4, GridTable6ColorfulAccent4, GridTable7ColorfulAccent4, GridTable1LightAccent5, GridTable2Accent5, GridTable3Accent5, GridTable4Accent5, GridTable5DarkAccent5, GridTable6ColorfulAccent5, GridTable7ColorfulAccent5, GridTable1LightAccent6, GridTable2Accent6, GridTable3Accent6, GridTable4Accent6, GridTable5DarkAccent6, GridTable6ColorfulAccent6, GridTable7ColorfulAccent6, ListTable1Light, ListTable2, ListTable3, ListTable4, ListTable5Dark, ListTable6Colorful, ListTable7Colorful, ListTable1LightAccent1, ListTable2Accent1, ListTable3Accent1, ListTable4Accent1, ListTable5DarkAccent1, ListTable6ColorfulAccent1, ListTable7ColorfulAccent1, ListTable1LightAccent2, ListTable2Accent2, ListTable3Accent2, ListTable4Accent2, ListTable5DarkAccent2, ListTable6ColorfulAccent2, ListTable7ColorfulAccent2, ListTable1LightAccent3, ListTable2Accent3, ListTable3Accent3, ListTable4Accent3, ListTable5DarkAccent3, ListTable6ColorfulAccent3, ListTable7ColorfulAccent3, ListTable1LightAccent4, ListTable2Accent4, ListTable3Accent4, ListTable4Accent4, ListTable5DarkAccent4, ListTable6ColorfulAccent4, ListTable7ColorfulAccent4, ListTable1LightAccent5, ListTable2Accent5, ListTable3Accent5, ListTable4Accent5, ListTable5DarkAccent5, ListTable6ColorfulAccent5, ListTable7ColorfulAccent5, ListTable1LightAccent6, ListTable2Accent6, ListTable3Accent6, ListTable4Accent6, ListTable5DarkAccent6, ListTable6ColorfulAccent6, ListTable7ColorfulAccent6, SmartLink, User, Nil.


## TableProperties.StyleOptionsEnum

The following values are defined: None, FirstRow, LastRow, FirstColumn, LastColumn, RowBands, Default, ColumnBands, Default2003.

