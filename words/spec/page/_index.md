---
title: "Page"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/page/
description: "Page"
notoc: true
weight: 340
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertpagenumbersonlinerequest">InsertPageNumbersOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertpagenumbersonlineresponse">InsertPageNumbersOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#pagenumber">PageNumber</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertpagenumbersrequest">InsertPageNumbersRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></br><a href="#pagenumber">PageNumber</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Render</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#renderpageonlinerequest">RenderPageOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2" colspan="2"><span style="color:SteelBlue;">Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#renderpagerequest">RenderPageRequest</a></td>
  </tr>
  </tbody>
</table>


## PageNumber

Represents a class is used for insert page number request building.

This class is used in [InsertPageNumbersOnlineRequest](#insertpagenumbersonlinerequest), [InsertPageNumbersRequest](#insertpagenumbersrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Alignment            | <span style="color:SteelBlue;">string</span>  | Gets or sets text alignment, possible values are left, right, center or justify. |
| Format               | <span style="color:SteelBlue;">string</span>  | Gets or sets the page number format, e.g. "{PAGE} of {NUMPAGES}". |
| IsTop                | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether if true the page number is added at the top of the page, else at the bottom. |
| SetPageNumberOnFirstPage | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether if true the page number is added on first page too. |


## InsertPageNumbersOnlineRequest

Represents a request model for [WordsApi.InsertPageNumbersOnline()](/words/insert-page-numbers/) operation.

An object of the **InsertPageNumbersOnlineRequest** class is created by the following constructor methods:

- InsertPageNumbersOnlineRequest()
- InsertPageNumbersOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [PageNumber](#pagenumber) ***pageNumber***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***pageNumber***     | PageNumber           | [PageNumber](#pagenumber)                     | Page number dto. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertPageNumbersOnlineResponse

Represents a response model for [WordsApi.InsertPageNumbersOnline()](/words/insert-page-numbers/) operation.

An object of the **InsertPageNumbersOnlineResponse** class is created by the following constructor methods:

- InsertPageNumbersOnlineResponse([DocumentResponse](/words/spec/document#documentresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DocumentResponse](/words/spec/document#documentresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertPageNumbersRequest

Represents a request model for [WordsApi.InsertPageNumbers()](/words/insert-page-numbers/) operation.

An object of the **InsertPageNumbersRequest** class is created by the following constructor methods:

- InsertPageNumbersRequest()
- InsertPageNumbersRequest(<span style="color:SteelBlue;">string</span> ***name***, [PageNumber](#pagenumber) ***pageNumber***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***pageNumber***     | PageNumber           | [PageNumber](#pagenumber)                     | Page number dto. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## RenderPageOnlineRequest

Represents a request model for [WordsApi.RenderPageOnline()](/words/documents/render-into-image/) operation.

An object of the **RenderPageOnlineRequest** class is created by the following constructor methods:

- RenderPageOnlineRequest()
- RenderPageOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***pageIndex***, <span style="color:SteelBlue;">string</span> ***format***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *fontsLocation*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***pageIndex***      | PageIndex            | <span style="color:SteelBlue;">int</span>     | The index of the page. |
| ***format***         | Format               | <span style="color:SteelBlue;">string</span>  | The destination format. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *fontsLocation*      | FontsLocation        | <span style="color:SteelBlue;">string</span>  | Folder in filestorage with custom fonts. |



## RenderPageRequest

Represents a request model for [WordsApi.RenderPage()](/words/documents/render-into-image/) operation.

An object of the **RenderPageRequest** class is created by the following constructor methods:

- RenderPageRequest()
- RenderPageRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***pageIndex***, <span style="color:SteelBlue;">string</span> ***format***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *fontsLocation*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***pageIndex***      | PageIndex            | <span style="color:SteelBlue;">int</span>     | The index of the page. |
| ***format***         | Format               | <span style="color:SteelBlue;">string</span>  | The destination format. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *fontsLocation*      | FontsLocation        | <span style="color:SteelBlue;">string</span>  | Folder in filestorage with custom fonts. |



## PageSetup.BorderAppliesToEnum

The following values are defined: AllPages, FirstPage, OtherPages.


## PageSetup.BorderDistanceFromEnum

The following values are defined: Text, PageEdge.


## PageSetup.LineNumberRestartModeEnum

The following values are defined: RestartPage, RestartSection, Continuous.


## PageSetup.OrientationEnum

The following values are defined: Portrait, Landscape.


## PageSetup.PageNumberStyleEnum

The following values are defined: Arabic, UppercaseRoman, LowercaseRoman, UppercaseLetter, LowercaseLetter, Ordinal, Number, OrdinalText, Hex, ChicagoManual, Kanji, KanjiDigit, AiueoHalfWidth, IrohaHalfWidth, ArabicFullWidth, ArabicHalfWidth, KanjiTraditional, KanjiTraditional2, NumberInCircle, DecimalFullWidth, Aiueo, Iroha, LeadingZero, Bullet, Ganada, Chosung, GB1, GB2, GB3, GB4, Zodiac1, Zodiac2, Zodiac3, TradChinNum1, TradChinNum2, TradChinNum3, TradChinNum4, SimpChinNum1, SimpChinNum2, SimpChinNum3, SimpChinNum4, HanjaRead, HanjaReadDigit, Hangul, Hanja, Hebrew1, Arabic1, Hebrew2, Arabic2, HindiLetter1, HindiLetter2, HindiArabic, HindiCardinalText, ThaiLetter, ThaiArabic, ThaiCardinalText, VietCardinalText, NumberInDash, LowercaseRussian, UppercaseRussian, None, Custom.


## PageSetup.PaperSizeEnum

The following values are defined: A3, A4, A5, B4, B5, Executive, Folio, Ledger, Legal, Letter, EnvelopeDL, Quarto, Statement, Tabloid, Paper10x14, Paper11x17, Custom.


## PageSetup.SectionStartEnum

The following values are defined: Continuous, NewColumn, NewPage, EvenPage, OddPage.


## PageSetup.VerticalAlignmentEnum

The following values are defined: Top, Center, Justify, Bottom.

