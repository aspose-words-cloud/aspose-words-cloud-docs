---
title: "Font"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/font/
description: "Font"
notoc: true
weight: 240
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
    <td style="vertical-align:middle;" class="bg-white"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getavailablefontsrequest">GetAvailableFontsRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#availablefontsresponse">AvailableFontsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#fontinfo">FontInfo</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><strong><i>Reset</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#resetcacherequest">ResetCacheRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">void</span></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  </tbody>
</table>


## Font

Represents a dTO container with a font element.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [FontResponse](/words/spec/run#fontresponse), [ListLevel](/words/spec/list#listlevel), [Style](/words/spec/style#style), [UpdateRunFontOnlineRequest](/words/spec/run#updaterunfontonlinerequest), [UpdateRunFontRequest](/words/spec/run#updaterunfontrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| AllCaps              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as all capital letters. |
| Bidi                 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the contents of this run shall have right-to-left characteristics. |
| Bold                 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as bold. |
| BoldBi               | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the right-to-left text is formatted as bold. |
| Border               | [Border](/words/spec/border#border)           | Gets or sets the border object, that specifies border for the font. |
| Color                | [XmlColor](/words/spec/style#xmlcolor)        | Gets or sets the color of the font. |
| ComplexScript        | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the contents of this run shall be treated as complex script text regardless of their Unicode character values when determining the formatting for this run. |
| DoubleStrikeThrough  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as double strikethrough text. |
| Emboss               | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as embossed. |
| Engrave              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as engraved. |
| Hidden               | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as hidden text. |
| HighlightColor       | [XmlColor](/words/spec/style#xmlcolor)        | Gets or sets the highlight (marker) color. |
| Italic               | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as italic. |
| ItalicBi             | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the right-to-left text is formatted as italic. |
| Kerning              | <span style="color:SteelBlue;">double</span>  | Gets or sets the font size at which kerning starts. |
| LocaleId             | <span style="color:SteelBlue;">int</span>     | Gets or sets the locale identifier (language) of the formatted characters. |
| LocaleIdBi           | <span style="color:SteelBlue;">int</span>     | Gets or sets the locale identifier (language) of the formatted right-to-left characters. |
| LocaleIdFarEast      | <span style="color:SteelBlue;">int</span>     | Gets or sets the locale identifier (language) of the formatted Asian characters. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the font. |
| NameAscii            | <span style="color:SteelBlue;">string</span>  | Gets or sets the font used for Latin text (characters with character codes from 0 (zero) through 127) . |
| NameBi               | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the font in a right-to-left language document. |
| NameFarEast          | <span style="color:SteelBlue;">string</span>  | Gets or sets the East Asian font name. |
| NameOther            | <span style="color:SteelBlue;">string</span>  | Gets or sets the font used for characters with character codes from 128 through 255. |
| NoProofing           | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the formatted characters are not to be spell checked. |
| Outline              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as outline. |
| Position             | <span style="color:SteelBlue;">double</span>  | Gets or sets the position of text (in points) relative to the base line. A positive number raises the text, and a negative number lowers it. |
| Scaling              | <span style="color:SteelBlue;">int</span>     | Gets or sets character width scaling in percent. |
| Shadow               | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as shadowed. |
| Size                 | <span style="color:SteelBlue;">double</span>  | Gets or sets the font size in points. |
| SizeBi               | <span style="color:SteelBlue;">double</span>  | Gets or sets the font size in points used in a right-to-left document. |
| SmallCaps            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as small capital letters. |
| Spacing              | <span style="color:SteelBlue;">double</span>  | Gets or sets the spacing (in points) between characters. |
| StrikeThrough        | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as strikethrough text. |
| StyleIdentifier      | [StyleIdentifierEnum](#font.styleidentifierenum) | Gets or sets the locale independent style identifier of the character style applied to this formatting. |
| StyleName            | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the character style applied to this formatting. |
| Subscript            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as subscript. |
| Superscript          | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the font is formatted as superscript. |
| TextEffect           | [TextEffectEnum](#font.texteffectenum)        | Gets or sets the font animation effect. |
| Underline            | [UnderlineEnum](#font.underlineenum)          | Gets or sets the type of underline applied to the font. |
| UnderlineColor       | [XmlColor](/words/spec/style#xmlcolor)        | Gets or sets the color of the underline applied to the font. |


## FontDto

Represents a fontDto.


## FontInfo

Represents a dTO container with font info.

This class is used in [AvailableFontsResponse](#availablefontsresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FilePath             | <span style="color:SteelBlue;">string</span>  | Gets or sets the path to the font file if any. |
| FontFamilyName       | <span style="color:SteelBlue;">string</span>  | Gets or sets the family name of the font. |
| FullFontName         | <span style="color:SteelBlue;">string</span>  | Gets or sets the full name of the font. |
| Version              | <span style="color:SteelBlue;">string</span>  | Gets or sets the version string of the font. |


## AvailableFontsResponse

Represents a REST response with data on system, additional and custom fonts, available for document processing.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| AdditionalFonts      | List&lt;[FontInfo](#fontinfo)&gt;             | Gets or sets the list of additional fonts, provided by Aspose team. |
| CustomFonts          | List&lt;[FontInfo](#fontinfo)&gt;             | Gets or sets the list of custom user fonts from user cloud storage. To use them, you should specify "fontsLocation" parameter in any request. |
| SystemFonts          | List&lt;[FontInfo](#fontinfo)&gt;             | Gets or sets the list of system fonts, available on the server. |


## GetAvailableFontsRequest

Represents a request model for [WordsApi.GetAvailableFonts()](/words/fonts/gets-the-list-of-fonts/) operation.

An object of the **GetAvailableFontsRequest** class is created by the following constructor methods:

- GetAvailableFontsRequest()
- GetAvailableFontsRequest(<span style="color:SteelBlue;">string</span> *fontsLocation*)

### Properties

A single `FontsLocation` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FontsLocation        | <span style="color:SteelBlue;">string</span>  | The folder in cloud storage with custom fonts. |


## ResetCacheRequest

Represents a request model for [WordsApi.ResetCache()](/words/fonts/reset-fonts-cache/) operation.


## Font.StyleIdentifierEnum

The following values are defined: Normal, Heading1, Heading2, Heading3, Heading4, Heading5, Heading6, Heading7, Heading8, Heading9, Index1, Index2, Index3, Index4, Index5, Index6, Index7, Index8, Index9, Toc1, Toc2, Toc3, Toc4, Toc5, Toc6, Toc7, Toc8, Toc9, NormalIndent, FootnoteText, CommentText, Header, Footer, IndexHeading, Caption, TableOfFigures, EnvelopeAddress, EnvelopeReturn, FootnoteReference, CommentReference, LineNumber, PageNumber, EndnoteReference, EndnoteText, TableOfAuthorities, Macro, ToaHeading, List, ListBullet, ListNumber, List2, List3, List4, List5, ListBullet2, ListBullet3, ListBullet4, ListBullet5, ListNumber2, ListNumber3, ListNumber4, ListNumber5, Title, Closing, Signature, DefaultParagraphFont, BodyText, BodyTextInd, ListContinue, ListContinue2, ListContinue3, ListContinue4, ListContinue5, MessageHeader, Subtitle, Salutation, Date, BodyText1I, BodyText1I2, NoteHeading, BodyText2, BodyText3, BodyTextInd2, BodyTextInd3, BlockText, Hyperlink, FollowedHyperlink, Strong, Emphasis, DocumentMap, PlainText, EmailSignature, HtmlTopOfForm, HtmlBottomOfForm, NormalWeb, HtmlAcronym, HtmlAddress, HtmlCite, HtmlCode, HtmlDefinition, HtmlKeyboard, HtmlPreformatted, HtmlSample, HtmlTypewriter, HtmlVariable, TableNormal, CommentSubject, NoList, OutlineList1, OutlineList2, OutlineList3, TableSimple1, TableSimple2, TableSimple3, TableClassic1, TableClassic2, TableClassic3, TableClassic4, TableColorful1, TableColorful2, TableColorful3, TableColumns1, TableColumns2, TableColumns3, TableColumns4, TableColumns5, TableGrid1, TableGrid2, TableGrid3, TableGrid4, TableGrid5, TableGrid6, TableGrid7, TableGrid8, TableList1, TableList2, TableList3, TableList4, TableList5, TableList6, TableList7, TableList8, Table3DEffects1, Table3DEffects2, Table3DEffects3, TableContemporary, TableElegant, TableProfessional, TableSubtle1, TableSubtle2, TableWeb1, TableWeb2, TableWeb3, BalloonText, TableGrid, TableTheme, PlaceholderText, NoSpacing, LightShading, LightList, LightGrid, MediumShading1, MediumShading2, MediumList1, MediumList2, MediumGrid1, MediumGrid2, MediumGrid3, DarkList, ColorfulShading, ColorfulList, ColorfulGrid, LightShadingAccent1, LightListAccent1, LightGridAccent1, MediumShading1Accent1, MediumShading2Accent1, MediumList1Accent1, Revision, ListParagraph, Quote, IntenseQuote, MediumList2Accent1, MediumGrid1Accent1, MediumGrid2Accent1, MediumGrid3Accent1, DarkListAccent1, ColorfulShadingAccent1, ColorfulListAccent1, ColorfulGridAccent1, LightShadingAccent2, LightListAccent2, LightGridAccent2, MediumShading1Accent2, MediumShading2Accent2, MediumList1Accent2, MediumList2Accent2, MediumGrid1Accent2, MediumGrid2Accent2, MediumGrid3Accent2, DarkListAccent2, ColorfulShadingAccent2, ColorfulListAccent2, ColorfulGridAccent2, LightShadingAccent3, LightListAccent3, LightGridAccent3, MediumShading1Accent3, MediumShading2Accent3, MediumList1Accent3, MediumList2Accent3, MediumGrid1Accent3, MediumGrid2Accent3, MediumGrid3Accent3, DarkListAccent3, ColorfulShadingAccent3, ColorfulListAccent3, ColorfulGridAccent3, LightShadingAccent4, LightListAccent4, LightGridAccent4, MediumShading1Accent4, MediumShading2Accent4, MediumList1Accent4, MediumList2Accent4, MediumGrid1Accent4, MediumGrid2Accent4, MediumGrid3Accent4, DarkListAccent4, ColorfulShadingAccent4, ColorfulListAccent4, ColorfulGridAccent4, LightShadingAccent5, LightListAccent5, LightGridAccent5, MediumShading1Accent5, MediumShading2Accent5, MediumList1Accent5, MediumList2Accent5, MediumGrid1Accent5, MediumGrid2Accent5, MediumGrid3Accent5, DarkListAccent5, ColorfulShadingAccent5, ColorfulListAccent5, ColorfulGridAccent5, LightShadingAccent6, LightListAccent6, LightGridAccent6, MediumShading1Accent6, MediumShading2Accent6, MediumList1Accent6, MediumList2Accent6, MediumGrid1Accent6, MediumGrid2Accent6, MediumGrid3Accent6, DarkListAccent6, ColorfulShadingAccent6, ColorfulListAccent6, ColorfulGridAccent6, SubtleEmphasis, IntenseEmphasis, SubtleReference, IntenseReference, BookTitle, Bibliography, TocHeading, PlainTable1, PlainTable2, PlainTable3, PlainTable4, PlainTable5, TableGridLight, GridTable1Light, GridTable2, GridTable3, GridTable4, GridTable5Dark, GridTable6Colorful, GridTable7Colorful, GridTable1LightAccent1, GridTable2Accent1, GridTable3Accent1, GridTable4Accent1, GridTable5DarkAccent1, GridTable6ColorfulAccent1, GridTable7ColorfulAccent1, GridTable1LightAccent2, GridTable2Accent2, GridTable3Accent2, GridTable4Accent2, GridTable5DarkAccent2, GridTable6ColorfulAccent2, GridTable7ColorfulAccent2, GridTable1LightAccent3, GridTable2Accent3, GridTable3Accent3, GridTable4Accent3, GridTable5DarkAccent3, GridTable6ColorfulAccent3, GridTable7ColorfulAccent3, GridTable1LightAccent4, GridTable2Accent4, GridTable3Accent4, GridTable4Accent4, GridTable5DarkAccent4, GridTable6ColorfulAccent4, GridTable7ColorfulAccent4, GridTable1LightAccent5, GridTable2Accent5, GridTable3Accent5, GridTable4Accent5, GridTable5DarkAccent5, GridTable6ColorfulAccent5, GridTable7ColorfulAccent5, GridTable1LightAccent6, GridTable2Accent6, GridTable3Accent6, GridTable4Accent6, GridTable5DarkAccent6, GridTable6ColorfulAccent6, GridTable7ColorfulAccent6, ListTable1Light, ListTable2, ListTable3, ListTable4, ListTable5Dark, ListTable6Colorful, ListTable7Colorful, ListTable1LightAccent1, ListTable2Accent1, ListTable3Accent1, ListTable4Accent1, ListTable5DarkAccent1, ListTable6ColorfulAccent1, ListTable7ColorfulAccent1, ListTable1LightAccent2, ListTable2Accent2, ListTable3Accent2, ListTable4Accent2, ListTable5DarkAccent2, ListTable6ColorfulAccent2, ListTable7ColorfulAccent2, ListTable1LightAccent3, ListTable2Accent3, ListTable3Accent3, ListTable4Accent3, ListTable5DarkAccent3, ListTable6ColorfulAccent3, ListTable7ColorfulAccent3, ListTable1LightAccent4, ListTable2Accent4, ListTable3Accent4, ListTable4Accent4, ListTable5DarkAccent4, ListTable6ColorfulAccent4, ListTable7ColorfulAccent4, ListTable1LightAccent5, ListTable2Accent5, ListTable3Accent5, ListTable4Accent5, ListTable5DarkAccent5, ListTable6ColorfulAccent5, ListTable7ColorfulAccent5, ListTable1LightAccent6, ListTable2Accent6, ListTable3Accent6, ListTable4Accent6, ListTable5DarkAccent6, ListTable6ColorfulAccent6, ListTable7ColorfulAccent6, SmartLink, User, Nil.


## Font.TextEffectEnum

The following values are defined: None, LasVegasLights, BlinkingBackground, SparkleText, MarchingBlackAnts, MarchingRedAnts, Shimmer.


## Font.UnderlineEnum

The following values are defined: None, Single, Words, Double, Dotted, Thick, Dash, DotDash, DotDotDash, Wavy, DottedHeavy, DashHeavy, DotDashHeavy, DotDotDashHeavy, WavyHeavy, DashLong, WavyDouble, DashLongHeavy.

