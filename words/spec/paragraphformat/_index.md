---
title: "ParagraphFormat"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/paragraphformat/
description: "ParagraphFormat"
notoc: true
weight: 360
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getparagraphformatonlinerequest">GetParagraphFormatOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#paragraphformatresponse">ParagraphFormatResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#paragraphformat">ParagraphFormat</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getparagraphformatrequest">GetParagraphFormatRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updateparagraphformatonlinerequest">UpdateParagraphFormatOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updateparagraphformatonlineresponse">UpdateParagraphFormatOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#paragraphformatupdate">ParagraphFormatUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updateparagraphformatrequest">UpdateParagraphFormatRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#paragraphformatresponse">ParagraphFormatResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#paragraphformat">ParagraphFormat</a></br><a href="#paragraphformatupdate">ParagraphFormatUpdate</a></td>
  </tr>
  </tbody>
</table>


## ParagraphFormatBase

Represents a paragraph format element base class.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| AddSpaceBetweenFarEastAndAlpha | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether inter-character spacing is automatically adjusted between regions of Latin text and regions of East Asian text in the current paragraph. |
| AddSpaceBetweenFarEastAndDigit | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether inter-character spacing is automatically adjusted between regions of numbers and regions of East Asian text in the current paragraph. |
| Alignment            | [AlignmentEnum](#paragraphformatbase.alignmentenum) | Gets or sets text alignment for the paragraph. |
| Bidi                 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this is a right-to-left paragraph. |
| DropCapPosition      | [DropCapPositionEnum](#paragraphformatbase.dropcappositionenum) | Gets or sets the position for a drop cap text. |
| FirstLineIndent      | <span style="color:SteelBlue;">double</span>  | Gets or sets the value (in points) for a first line or hanging indent. Use a positive value to set a first-line indent, and use a negative value to set a hanging indent. |
| KeepTogether         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether all lines in the paragraph are to remain on the same page. |
| KeepWithNext         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the paragraph is to remains on the same page as the paragraph that follows it. |
| LeftIndent           | <span style="color:SteelBlue;">double</span>  | Gets or sets the value (in points) , that represents the left indent for paragraph. |
| LineSpacing          | <span style="color:SteelBlue;">double</span>  | Gets or sets the line spacing (in points) for the paragraph. |
| LineSpacingRule      | [LineSpacingRuleEnum](#paragraphformatbase.linespacingruleenum) | Gets or sets the line spacing for the paragraph. |
| LinesToDrop          | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of lines of the paragraph text used to calculate the drop cap height. |
| NoSpaceBetweenParagraphsOfSameStyle | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether SpaceBefore and SpaceAfter will be ignored between the paragraphs of the same style. |
| OutlineLevel         | [OutlineLevelEnum](#paragraphformatbase.outlinelevelenum) | Gets or sets the outline level of the paragraph in the document. |
| PageBreakBefore      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether a page break is forced before the paragraph. |
| RightIndent          | <span style="color:SteelBlue;">double</span>  | Gets or sets the value (in points) that represents the right indent for paragraph. |
| Shading              | [Shading](#shading)                           | Gets or sets the Shading object, that refers to the shading formatting for the paragraph. |
| SpaceAfter           | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of spacing (in points) after the paragraph. |
| SpaceAfterAuto       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the amount of spacing after the paragraph is set automatically. |
| SpaceBefore          | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of spacing (in points) before the paragraph. |
| SpaceBeforeAuto      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the amount of spacing before the paragraph is set automatically. |
| StyleIdentifier      | [StyleIdentifierEnum](/words/spec/font#font.styleidentifierenum) | Gets or sets the locale independent style identifier of the paragraph style applied to this formatting. |
| StyleName            | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the paragraph style applied to this formatting. |
| SuppressAutoHyphens  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the current paragraph should be exempted from any hyphenation which is applied in the document settings. |
| SuppressLineNumbers  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the current paragraph's lines should be exempted from line numbering which is applied in the parent section. |
| WidowControl         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the first and last lines in the paragraph are to remain on the same page as the rest of the paragraph. |


## ParagraphFormat

Represents a paragraph format element.

This class is inherited from [ParagraphFormatBase](#paragraphformatbase) and used in [ParagraphFormatResponse](#paragraphformatresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| AddSpaceBetweenFarEastAndAlpha | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether inter-character spacing is automatically adjusted between regions of Latin text and regions of East Asian text in the current paragraph. |
| AddSpaceBetweenFarEastAndDigit | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether inter-character spacing is automatically adjusted between regions of numbers and regions of East Asian text in the current paragraph. |
| Alignment            | [AlignmentEnum](#paragraphformatbase.alignmentenum) | Gets or sets text alignment for the paragraph. |
| Bidi                 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this is a right-to-left paragraph. |
| DropCapPosition      | [DropCapPositionEnum](#paragraphformatbase.dropcappositionenum) | Gets or sets the position for a drop cap text. |
| FirstLineIndent      | <span style="color:SteelBlue;">double</span>  | Gets or sets the value (in points) for a first line or hanging indent. Use a positive value to set a first-line indent, and use a negative value to set a hanging indent. |
| KeepTogether         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether all lines in the paragraph are to remain on the same page. |
| KeepWithNext         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the paragraph is to remains on the same page as the paragraph that follows it. |
| LeftIndent           | <span style="color:SteelBlue;">double</span>  | Gets or sets the value (in points) , that represents the left indent for paragraph. |
| LineSpacing          | <span style="color:SteelBlue;">double</span>  | Gets or sets the line spacing (in points) for the paragraph. |
| LineSpacingRule      | [LineSpacingRuleEnum](#paragraphformatbase.linespacingruleenum) | Gets or sets the line spacing for the paragraph. |
| LinesToDrop          | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of lines of the paragraph text used to calculate the drop cap height. |
| NoSpaceBetweenParagraphsOfSameStyle | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether SpaceBefore and SpaceAfter will be ignored between the paragraphs of the same style. |
| OutlineLevel         | [OutlineLevelEnum](#paragraphformatbase.outlinelevelenum) | Gets or sets the outline level of the paragraph in the document. |
| PageBreakBefore      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether a page break is forced before the paragraph. |
| RightIndent          | <span style="color:SteelBlue;">double</span>  | Gets or sets the value (in points) that represents the right indent for paragraph. |
| Shading              | [Shading](#shading)                           | Gets or sets the Shading object, that refers to the shading formatting for the paragraph. |
| SpaceAfter           | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of spacing (in points) after the paragraph. |
| SpaceAfterAuto       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the amount of spacing after the paragraph is set automatically. |
| SpaceBefore          | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of spacing (in points) before the paragraph. |
| SpaceBeforeAuto      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the amount of spacing before the paragraph is set automatically. |
| StyleIdentifier      | [StyleIdentifierEnum](/words/spec/font#font.styleidentifierenum) | Gets or sets the locale independent style identifier of the paragraph style applied to this formatting. |
| StyleName            | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the paragraph style applied to this formatting. |
| SuppressAutoHyphens  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the current paragraph should be exempted from any hyphenation which is applied in the document settings. |
| SuppressLineNumbers  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the current paragraph's lines should be exempted from line numbering which is applied in the parent section. |
| WidowControl         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the first and last lines in the paragraph are to remain on the same page as the rest of the paragraph. |
| IsHeading            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the paragraph style is one of the built-in Heading styles. |
| IsListItem           | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the paragraph is an item in a bulleted or numbered list. |


## ParagraphFormatUpdate

Represents a paragraph format element update DTO.

This class is inherited from [ParagraphFormatBase](#paragraphformatbase) and used in [UpdateParagraphFormatOnlineRequest](#updateparagraphformatonlinerequest), [UpdateParagraphFormatRequest](#updateparagraphformatrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| AddSpaceBetweenFarEastAndAlpha | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether inter-character spacing is automatically adjusted between regions of Latin text and regions of East Asian text in the current paragraph. |
| AddSpaceBetweenFarEastAndDigit | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether inter-character spacing is automatically adjusted between regions of numbers and regions of East Asian text in the current paragraph. |
| Alignment            | [AlignmentEnum](#paragraphformatbase.alignmentenum) | Gets or sets text alignment for the paragraph. |
| Bidi                 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether this is a right-to-left paragraph. |
| DropCapPosition      | [DropCapPositionEnum](#paragraphformatbase.dropcappositionenum) | Gets or sets the position for a drop cap text. |
| FirstLineIndent      | <span style="color:SteelBlue;">double</span>  | Gets or sets the value (in points) for a first line or hanging indent. Use a positive value to set a first-line indent, and use a negative value to set a hanging indent. |
| KeepTogether         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether all lines in the paragraph are to remain on the same page. |
| KeepWithNext         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the paragraph is to remains on the same page as the paragraph that follows it. |
| LeftIndent           | <span style="color:SteelBlue;">double</span>  | Gets or sets the value (in points) , that represents the left indent for paragraph. |
| LineSpacing          | <span style="color:SteelBlue;">double</span>  | Gets or sets the line spacing (in points) for the paragraph. |
| LineSpacingRule      | [LineSpacingRuleEnum](#paragraphformatbase.linespacingruleenum) | Gets or sets the line spacing for the paragraph. |
| LinesToDrop          | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of lines of the paragraph text used to calculate the drop cap height. |
| NoSpaceBetweenParagraphsOfSameStyle | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether SpaceBefore and SpaceAfter will be ignored between the paragraphs of the same style. |
| OutlineLevel         | [OutlineLevelEnum](#paragraphformatbase.outlinelevelenum) | Gets or sets the outline level of the paragraph in the document. |
| PageBreakBefore      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether a page break is forced before the paragraph. |
| RightIndent          | <span style="color:SteelBlue;">double</span>  | Gets or sets the value (in points) that represents the right indent for paragraph. |
| Shading              | [Shading](#shading)                           | Gets or sets the Shading object, that refers to the shading formatting for the paragraph. |
| SpaceAfter           | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of spacing (in points) after the paragraph. |
| SpaceAfterAuto       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the amount of spacing after the paragraph is set automatically. |
| SpaceBefore          | <span style="color:SteelBlue;">double</span>  | Gets or sets the amount of spacing (in points) before the paragraph. |
| SpaceBeforeAuto      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the amount of spacing before the paragraph is set automatically. |
| StyleIdentifier      | [StyleIdentifierEnum](/words/spec/font#font.styleidentifierenum) | Gets or sets the locale independent style identifier of the paragraph style applied to this formatting. |
| StyleName            | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the paragraph style applied to this formatting. |
| SuppressAutoHyphens  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the current paragraph should be exempted from any hyphenation which is applied in the document settings. |
| SuppressLineNumbers  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the current paragraph's lines should be exempted from line numbering which is applied in the parent section. |
| WidowControl         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the first and last lines in the paragraph are to remain on the same page as the rest of the paragraph. |


## Shading

Represents a dTO container with a paragraph format shading element.

This class is used in [ParagraphFormat](#paragraphformat), [ParagraphFormatBase](#paragraphformatbase), [ParagraphFormatUpdate](#paragraphformatupdate).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| BackgroundPatternColor | [XmlColor](/words/spec/style#xmlcolor)        | Gets or sets the color that's applied to the background of the Shading object. |
| ForegroundPatternColor | [XmlColor](/words/spec/style#xmlcolor)        | Gets or sets the color that's applied to the foreground of the Shading object. |
| Texture              | [TextureEnum](/words/spec/style#shading.textureenum) | Gets or sets the shading texture. |


## GetParagraphFormatOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **GetParagraphFormatOnlineRequest** class is created by the following constructor methods:

- GetParagraphFormatOnlineRequest()
- GetParagraphFormatOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetParagraphFormatRequest

Represents a request model for [WordsApi.GetParagraphFormat()](/words/paragraphs/get-all-formatting/) operation.

An object of the **GetParagraphFormatRequest** class is created by the following constructor methods:

- GetParagraphFormatRequest()
- GetParagraphFormatRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

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



## ParagraphFormatResponse

Represents a REST response with the formatting properties of a paragraph.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [UpdateParagraphFormatOnlineResponse](#updateparagraphformatonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| ParagraphFormat      | [ParagraphFormat](#paragraphformat)           | Gets or sets the formatting properties of a paragraph. |


## UpdateParagraphFormatOnlineRequest

Represents a request model for [WordsApi.UpdateParagraphFormatOnline()](/words/paragraphs/update/) operation.

An object of the **UpdateParagraphFormatOnlineRequest** class is created by the following constructor methods:

- UpdateParagraphFormatOnlineRequest()
- UpdateParagraphFormatOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [ParagraphFormatUpdate](#paragraphformatupdate) ***paragraphFormatDto***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***paragraphFormatDto*** | ParagraphFormatDto   | [ParagraphFormatUpdate](#paragraphformatupdate) | Dto for paragraph format update. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateParagraphFormatOnlineResponse

Represents a response model for [WordsApi.UpdateParagraphFormatOnline()](/words/paragraphs/update/) operation.

An object of the **UpdateParagraphFormatOnlineResponse** class is created by the following constructor methods:

- UpdateParagraphFormatOnlineResponse([ParagraphFormatResponse](#paragraphformatresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [ParagraphFormatResponse](#paragraphformatresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateParagraphFormatRequest

Represents a request model for [WordsApi.UpdateParagraphFormat()](/words/paragraphs/update/) operation.

An object of the **UpdateParagraphFormatRequest** class is created by the following constructor methods:

- UpdateParagraphFormatRequest()
- UpdateParagraphFormatRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, [ParagraphFormatUpdate](#paragraphformatupdate) ***paragraphFormatDto***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***paragraphFormatDto*** | ParagraphFormatDto   | [ParagraphFormatUpdate](#paragraphformatupdate) | Dto for paragraph format update. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## ParagraphFormatBase.AlignmentEnum

The following values are defined: Left, Center, Right, Justify, Distributed, ArabicMediumKashida, ArabicHighKashida, ArabicLowKashida, ThaiDistributed.


## ParagraphFormatBase.DropCapPositionEnum

The following values are defined: None, Normal, Margin.


## ParagraphFormatBase.LineSpacingRuleEnum

The following values are defined: AtLeast, Exactly, Multiple.


## ParagraphFormatBase.OutlineLevelEnum

The following values are defined: Level1, Level2, Level3, Level4, Level5, Level6, Level7, Level8, Level9, BodyText.

