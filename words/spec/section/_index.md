---
title: "Section"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/section/
description: "Section"
notoc: true
weight: 420
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
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletesectiononlinerequest">DeleteSectionOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletesectionrequest">DeleteSectionRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">void</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="6"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getsectiononlinerequest">GetSectionOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#sectionresponse">SectionResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#section">Section</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getsectionpagesetuponlinerequest">GetSectionPageSetupOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#sectionpagesetupresponse">SectionPageSetupResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#pagesetup">PageSetup</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getsectionpagesetuprequest">GetSectionPageSetupRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getsectionrequest">GetSectionRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#sectionresponse">SectionResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#section">Section</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getsectionsonlinerequest">GetSectionsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#sectionlinkcollectionresponse">SectionLinkCollectionResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#sectionlinkcollection">SectionLinkCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getsectionsrequest">GetSectionsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatesectionpagesetuponlinerequest">UpdateSectionPageSetupOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatesectionpagesetuponlineresponse">UpdateSectionPageSetupOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#pagesetup">PageSetup</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatesectionpagesetuprequest">UpdateSectionPageSetupRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#sectionpagesetupresponse">SectionPageSetupResponse</a></td>
  </tr>
  </tbody>
</table>


## PageSetup

Represents a page setup properties of a section.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [SectionPageSetupResponse](#sectionpagesetupresponse), [UpdateSectionPageSetupOnlineRequest](#updatesectionpagesetuponlinerequest), [UpdateSectionPageSetupRequest](#updatesectionpagesetuprequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| Bidi                 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this section contains bidirectional (complex scripts) text. |
| BorderAlwaysInFront  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the page border is positioned relative to intersecting texts and objects. |
| BorderAppliesTo      | [BorderAppliesToEnum](/words/spec/page#pagesetup.borderappliestoenum) | Gets or sets the option that controls which pages the page border is printed on. |
| BorderDistanceFrom   | [BorderDistanceFromEnum](/words/spec/page#pagesetup.borderdistancefromenum) | Gets or sets the value, that indicates whether the specified page border is measured from the edge of the page or from the text it surrounds. |
| BottomMargin         | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance (in points) between the bottom edge of the page and the bottom boundary of the body text. |
| DifferentFirstPageHeaderFooter | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether a different header or footer is used on the first page. |
| FirstPageTray        | <span style="color:SteelBlue;">int</span>     | Gets or sets the paper tray (bin) to use for the first page of a section. The value is implementation (printer) specific. |
| FooterDistance       | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance (in points) between the footer and the bottom of the page. |
| Gutter               | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of extra space added to the margin for document binding. |
| HeaderDistance       | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance (in points) between the header and the top of the page. |
| LeftMargin           | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance (in points) between the left edge of the page and the left boundary of the body text. |
| LineNumberCountBy    | <span style="color:SteelBlue;">int</span>     | Gets or sets the numeric increment for line numbers. |
| LineNumberDistanceFromText | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance between the right edge of line numbers and the left edge of the document. |
| LineNumberRestartMode | [LineNumberRestartModeEnum](/words/spec/page#pagesetup.linenumberrestartmodeenum) | Gets or sets the way line numbering runs that is, whether it starts over at the beginning of a new page or section or runs continuously. |
| LineStartingNumber   | <span style="color:SteelBlue;">int</span>     | Gets or sets the starting line number. |
| Orientation          | [OrientationEnum](/words/spec/page#pagesetup.orientationenum) | Gets or sets the orientation of the page. |
| OtherPagesTray       | <span style="color:SteelBlue;">int</span>     | Gets or sets the paper tray (bin) to be used for all but the first page of a section. The value is implementation (printer) specific. |
| PageHeight           | <span style="color:SteelBlue;">double</span>  | Gets or sets the height of the page in points. |
| PageNumberStyle      | [PageNumberStyleEnum](/words/spec/page#pagesetup.pagenumberstyleenum) | Gets or sets the page number format. |
| PageStartingNumber   | <span style="color:SteelBlue;">int</span>     | Gets or sets the starting page number of the section. |
| PageWidth            | <span style="color:SteelBlue;">double</span>  | Gets or sets the width of the page in points. |
| PaperSize            | [PaperSizeEnum](/words/spec/page#pagesetup.papersizeenum) | Gets or sets the paper size. |
| RestartPageNumbering | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether page numbering restarts at the beginning of the section. |
| RightMargin          | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance (in points) between the right edge of the page and the right boundary of the body text. |
| RtlGutter            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether Microsoft Word uses gutters for the section based on a right-to-left language or a left-to-right language. |
| SectionStart         | [SectionStartEnum](/words/spec/page#pagesetup.sectionstartenum) | Gets or sets the type of section break for the specified object. |
| SuppressEndnotes     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether endnotes are printed at the end of the next section that doesn't suppress endnotes. Suppressed endnotes are printed before the endnotes in that section. |
| TopMargin            | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance (in points) between the top edge of the page and the top boundary of the body text. |
| VerticalAlignment    | [VerticalAlignmentEnum](/words/spec/page#pagesetup.verticalalignmentenum) | Gets or sets the vertical alignment of text on each page in the document.or section. |


## Section

Represents a dTO container with a section element.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [SectionResponse](#sectionresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| ChildNodes           | List&lt;[NodeLink](/words/spec/link#nodelink)&gt; | Gets or sets the list of child nodes. |
| HeaderFooters        | [LinkElement](/words/spec/link#linkelement)   | Gets or sets the link to HeaderFooters resource. |
| PageSetup            | [LinkElement](/words/spec/link#linkelement)   | Gets or sets the link to PageSetup resource. |
| Paragraphs           | [LinkElement](/words/spec/link#linkelement)   | Gets or sets the link to Paragraphs resource. |
| Tables               | [LinkElement](/words/spec/link#linkelement)   | Gets or sets the link to Tables resource. |


## SectionLink

Represents a section link element.

This class is inherited from [NodeLink](/words/spec/link#nodelink) and used in [SectionLinkCollection](#sectionlinkcollection).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |


## SectionLinkCollection

Represents a collection of section's links.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [SectionLinkCollectionResponse](#sectionlinkcollectionresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| SectionLinkList      | List&lt;[SectionLink](#sectionlink)&gt;       | Gets or sets the collection of section's links. |


## SectionResponse

Represents a REST response with a section.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Section              | [Section](#section)                           | Gets or sets the section. |


## DeleteSectionOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **DeleteSectionOnlineRequest** class is created by the following constructor methods:

- DeleteSectionOnlineRequest()
- DeleteSectionOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteSectionRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **DeleteSectionRequest** class is created by the following constructor methods:

- DeleteSectionRequest()
- DeleteSectionRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## GetSectionOnlineRequest

Represents a request model for [WordsApi.GetSectionOnline()](/words/sections/get/) operation.

An object of the **GetSectionOnlineRequest** class is created by the following constructor methods:

- GetSectionOnlineRequest()
- GetSectionOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetSectionPageSetupOnlineRequest

Represents a request model for [WordsApi.GetSectionPageSetupOnline()](/words/sections/read/) operation.

An object of the **GetSectionPageSetupOnlineRequest** class is created by the following constructor methods:

- GetSectionPageSetupOnlineRequest()
- GetSectionPageSetupOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetSectionPageSetupRequest

Represents a request model for [WordsApi.GetSectionPageSetup()](/words/sections/read/) operation.

An object of the **GetSectionPageSetupRequest** class is created by the following constructor methods:

- GetSectionPageSetupRequest()
- GetSectionPageSetupRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetSectionRequest

Represents a request model for [WordsApi.GetSection()](/words/sections/get/) operation.

An object of the **GetSectionRequest** class is created by the following constructor methods:

- GetSectionRequest()
- GetSectionRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetSectionsOnlineRequest

Represents a request model for [WordsApi.GetSectionsOnline()](/words/sections/get-all/) operation.

An object of the **GetSectionsOnlineRequest** class is created by the following constructor methods:

- GetSectionsOnlineRequest()
- GetSectionsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetSectionsRequest

Represents a request model for [WordsApi.GetSections()](/words/sections/get-all/) operation.

An object of the **GetSectionsRequest** class is created by the following constructor methods:

- GetSectionsRequest()
- GetSectionsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## SectionLinkCollectionResponse

Represents a REST response with a collection of sections.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Sections             | [SectionLinkCollection](#sectionlinkcollection) | Gets or sets the collection of sections. |


## SectionPageSetupResponse

Represents a REST response with a page setup of a section.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [UpdateSectionPageSetupOnlineResponse](#updatesectionpagesetuponlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| PageSetup            | [PageSetup](#pagesetup)                       | Gets or sets the page setup of a section. |


## UpdateSectionPageSetupOnlineRequest

Represents a request model for [WordsApi.UpdateSectionPageSetupOnline()](/words/sections/update/) operation.

An object of the **UpdateSectionPageSetupOnlineRequest** class is created by the following constructor methods:

- UpdateSectionPageSetupOnlineRequest()
- UpdateSectionPageSetupOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, [PageSetup](#pagesetup) ***pageSetup***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| ***pageSetup***      | PageSetup            | [PageSetup](#pagesetup)                       | Page setup properties dto. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateSectionPageSetupOnlineResponse

Represents a response model for [WordsApi.UpdateSectionPageSetupOnline()](/words/sections/update/) operation.

An object of the **UpdateSectionPageSetupOnlineResponse** class is created by the following constructor methods:

- UpdateSectionPageSetupOnlineResponse([SectionPageSetupResponse](#sectionpagesetupresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [SectionPageSetupResponse](#sectionpagesetupresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateSectionPageSetupRequest

Represents a request model for [WordsApi.UpdateSectionPageSetup()](/words/sections/update/) operation.

An object of the **UpdateSectionPageSetupRequest** class is created by the following constructor methods:

- UpdateSectionPageSetupRequest()
- UpdateSectionPageSetupRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***sectionIndex***, [PageSetup](#pagesetup) ***pageSetup***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***sectionIndex***   | SectionIndex         | <span style="color:SteelBlue;">int</span>     | The index of the section. |
| ***pageSetup***      | PageSetup            | [PageSetup](#pagesetup)                       | Page setup properties dto. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |


