---
title: "Update Font Properties of the Text"
second_title: "Paragraphs in a Document"
type: docs
url: /paragraphs/update-font-properties/
aliases: [/update-font-properties/]
description: "Update text paragraph font properties in a Word document"
weight: 120
---

This article explains how to format the text. Using [PUT /words/{name}/{paragraphPath}/runs/{index}/font](https://apireference.aspose.cloud/words/#/Runs/UpdateRunFont) API you can update font properties of the text.

## REST API

```JAVA
~/{file-name}/{paragraphPath}/runs/{index}/font
```
, where:

- *{file-name}* is a name of a document.
- *{paragraphPath}* is a path to a paragraph in a document:
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.
- *{index}* is an index of a run.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|AllCaps|bool|True if the font is formatted as all capital letters.|
|Bidi|bool|Specifies whether the contents of this run shall have right-to-left characteristics.|
|Bold|bool|True if the font is formatted as bold.|
|BoldBi|bool|True if the right-to-left text is formatted as bold.|
|Border|Border|Border object that specifies border for the font.|
|Color|Color|Specifies the color of the font.|
|ComplexScript|bool|Specifies whether the contents of this run shall be treated as complex script text regardless of their Unicode character values when determining the formatting for this run.|
|DoubleStrikeThrough|bool|True if the font is formatted as double strikethrough text.|
|Emboss|bool|True if the font is formatted as embossed.|
|Engrave|bool|True if the font is formatted as engraved.|
|Hidden|bool|True if the font is formatted as hidden text.|
|HighlightColor|Color|Specifies the highlight (marker) color.|
|Italic|bool|True if the font is formatted as italic.|
|ItalicBi|bool|True if the right-to-left text is formatted as italic.|
|Kerning|double|Specifies the font size at which kerning starts.|
|LocaleId|int|Specifies the locale identifier (language) of the formatted characters. For the list of locale identifiers see <http://www.microsoft.com/globaldev/reference/lcid-all.mspx>|
|LocaleIdBi|int|Specifies the locale identifier (language) of the formatted right-to-left characters. For the list of locale identifiers see <http://www.microsoft.com/globaldev/reference/lcid-all.mspx>|
|LocaleIdFarEast|int|Specifies the locale identifier (language) of the formatted Asian characters. For the list of locale identifiers see <http://www.microsoft.com/globaldev/reference/lcid-all.mspx>|
|Name|string|Specifies the name of the font.|
|NameAscii|bool|Specifies the font used for Latin text (characters with character codes from 0 (zero) through 127).|
|NameBi|bool|Specifies the name of the font in a right-to-left language document.|
|NameFarEast|bool|Specifies an East Asian font name.|
|NameOther|bool|Specifies the font used for characters with character codes from 128 through 255.|
|NoProofing|bool|True when the formatted characters are not to be spell checked.|
|Outline|bool|True if the font is formatted as an outline.|
|Position|double|Specifies the position of the text (in points) relative to the baseline. A positive number raises the text, and a negative number lowers it.|
|Scaling|int|Specifies character width scaling in percent.|
|Shadow|bool|True if the font is formatted as shadowed.|
|Size|double|Specifies the font size in points.|
|SizeBi|double|Specifies the font size in points used in a right-to-left document.|
|SmallCaps|bool|True if the font is formatted as small capital letters.|
|Spacing|double|Specifies the spacing (in points) between characters.|
|StrikeThrough|bool|True if the font is formatted as strikethrough text.|
|StyleIdentifier|StyleIdentifier|Specifies the locale independent style identifier of the character style applied to this formatting.|
|StyleName|string|Specifies the name of the character style applied to this formatting.|
|Subscript|bool|True if the font is formatted as a subscript.|
|Superscript|bool|True if the font is formatted as superscript.|
|TextEffect|TextEffect|Specifies the font animation effect.|
|Underline|Underline|Specifies the type of underline applied to the font.|
|UnderlineColor|Color|Specifies the color of the underline applied to the font.|

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [SampleWordDocument.docx](SampleWordDocument.docx) and output [ResultWordDocument.docx](ResultWordDocument.docx) files designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "UpdateRunFontOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "UpdateRunFontOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
   "Font":{
      "AllCaps":false,
      "Bidi":false,
      "Bold":true,
      "BoldBi":false,
      "Border":{
         "Color":{
            "Web":"",
            "Alpha":0
         },
         "DistanceFromText":0.0,
         "LineStyle":"None",
         "LineWidth":0.0,
         "Shadow":false,
         "link":null
      },
      "Color":{
         "Web":"",
         "Alpha":0
      },
      "ComplexScript":false,
      "DoubleStrikeThrough":false,
      "Emboss":false,
      "Engrave":false,
      "Hidden":false,
      "HighlightColor":{
         "Web":"",
         "Alpha":0
      },
      "Italic":false,
      "ItalicBi":false,
      "Kerning":0.0,
      "LocaleId":1033,
      "LocaleIdBi":1025,
      "LocaleIdFarEast":1033,
      "Name":"Calibri",
      "NameAscii":"Calibri",
      "NameBi":"Calibri",
      "NameFarEast":"Calibri",
      "NameOther":"Calibri",
      "NoProofing":false,
      "Outline":false,
      "Position":0.0,
      "Scaling":100,
      "Shadow":false,
      "Size":31.0,
      "SizeBi":14.0,
      "SmallCaps":false,
      "Spacing":0.0,
      "StrikeThrough":false,
      "StyleIdentifier":"DefaultParagraphFont",
      "StyleName":"Default Paragraph Font",
      "Subscript":false,
      "Superscript":false,
      "TextEffect":"None",
      "Underline":"None",
      "UnderlineColor":{
         "Web":"",
         "Alpha":0
      },
      "link":{
         "Href":"https://api.aspose.cloud/v4.0/words/ResultWordDocument.docx/sections/0/paragraphs/2/runs/0/font",
         "Rel":"self",
         "Type":null,
         "Title":null
      }
   },
   "Code":200,
   "Status":"OK"
}
```
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "UpdateRunFontOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "UpdateRunFontOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "UpdateRunFontOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateRunFontOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "UpdateRunFontOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "UpdateRunFontOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateRunFontOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "UpdateRunFontOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "UpdateRunFontOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "UpdateRunFontOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
