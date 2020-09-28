---
title: "Update Font Properties"
second_title: "Paragraphs in a Document"
type: docs
url: /paragraphs/update-font-properties/
aliases: [/update-font-properties/]
weight: 110
---

This REST API updates font properties.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|AllCaps|bool|True if the font is formatted as all capital letters.|
|Bidi|bool|Specifies whether the contents of this run shall have right-to-left characteristics.|
|Bold|bool|True if the font is formatted as bold.|
|BoldBi|bool|True if the right-to-left text is formatted as bold.|
|Border|Border|Border object that specifies the border for the font.|
|Color|Color|Specifies the color of the font.|
|ComplexScript|bool|Specifies whether the contents of this run shall be treated as complex script text regardless of their Unicode character values when determining the formatting for this run.|
|DoubleStrikeThrough|bool|True if the font is formatted as double strikethrough text.|
|Emboss|bool|True if the font is formatted as embossed.|
|Engrave|bool|True if the font is formatted as engraved.|
|Hidden|bool|True if the font is formatted as hidden text.|
|HighlightColor|Color|Specifies the highlight (marker) color.|
|Italic|bool|True if the font is formatted as italic.|
|ItalicBi|bool|True if the right-to-left text is formatted as italic.|
|Kerning|double|Specifies the font size at which kerning starts.|
|LocaleId|int|Specifies the locale identifier (language) of the formatted characters. For the list of locale, identifiers see <http://www.microsoft.com/globaldev/reference/lcid-all.mspx>|
|LocaleIdBi|int|Specifies the locale identifier (language) of the formatted right-to-left characters. For the list of locale, identifiers see <http://www.microsoft.com/globaldev/reference/lcid-all.mspx>|
|LocaleIdFarEast|int|Specifies the locale identifier (language) of the formatted Asian characters. For the list of locale, identifiers see <http://www.microsoft.com/globaldev/reference/lcid-all.mspx>|
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

## REST API

```JAVA
~/{file-name}/{paragraphPath}/runs/{index}/font
```
, where:

- *{file-name}* is a filename of a document.
- *{paragraphPath}* is a path to a specific paragraph in a document:
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.
- *{index}* is an index of a run.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Runs/UpdateRunFont) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to update font properties
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/paragraphs/0/runs/0/font" \
-X PUT \
-d "{ 'AllCaps': 'false', 'Bidi': 'false', 'Bold': 'false', 'BoldBi': 'false', 'Border': { 'LineStyle': 'None', 'LineWidth': '0', 'DistanceFromText': '0', 'Shadow': 'false' }, 'ComplexScript': 'false', 'DoubleStrikeThrough': 'false', 'Emboss': 'false', 'Engrave': 'false', 'Hidden': 'false', 'Italic': 'true', 'ItalicBi': 'false', 'Kerning': '0', 'LocaleId': '1033', 'LocaleIdBi': '1025', 'LocaleIdFarEast': '1033', 'Name': 'Calibri', 'NameAscii': 'Calibri', 'NameBi': 'Times New Roman', 'NameFarEast': 'Calibri', 'NameOther': 'Calibri', 'NoProofing': 'false', 'Outline': 'false, 'Position': '0', 'Scaling': '100', 'Shadow': 'false', 'Size': '11', 'SizeBi': '11', 'SmallCaps': 'false', 'Spacing': '0', 'StrikeThrough': 'false', 'StyleIdentifier': 'DefaultParagraphFont', 'StyleName': 'Default Paragraph Font', 'Subscript': 'false', 'Superscript': 'false', 'TextEffect': 'None', 'Underline': 'Dash' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Font": {
    "AllCaps": false,
    "Bidi": false,
    "Bold": false,
    "BoldBi": false,
    "Border": {
      "Color": {
        "Web": "",
        "Alpha": 0
      },
      "DistanceFromText": 0.0,
      "LineStyle": "None",
      "LineWidth": 0.0,
      "Shadow": false,
      "link": null
    },
    "Color": {
      "Web": "",
      "Alpha": 0
    },
    "ComplexScript": false,
    "DoubleStrikeThrough": false,
    "Emboss": false,
    "Engrave": false,
    "Hidden": false,
    "HighlightColor": {
      "Web": "",
      "Alpha": 0
    },
    "Italic": true,
    "ItalicBi": false,
    "Kerning": 0.0,
    "LocaleId": 1033,
    "LocaleIdBi": 1025,
    "LocaleIdFarEast": 1033,
    "Name": "Calibri",
    "NameAscii": "Calibri",
    "NameBi": "Times New Roman",
    "NameFarEast": "Calibri",
    "NameOther": "Calibri",
    "NoProofing": false,
    "Outline": false,
    "Position": 0.0,
    "Scaling": 100,
    "Shadow": false,
    "Size": 11.0,
    "SizeBi": 11.0,
    "SmallCaps": false,
    "Spacing": 0.0,
    "StrikeThrough": false,
    "StyleIdentifier": "DefaultParagraphFont",
    "StyleName": "Default Paragraph Font",
    "Subscript": false,
    "Superscript": false,
    "TextEffect": "None",
    "Underline": "Dash",
    "UnderlineColor": {
      "Web": "",
      "Alpha": 0
    },
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/0/paragraphs/0/runs/1/font",
      "Rel": "self",
      "Type": null,
      "Title": null
    }
  },
  "Code": 200,
  "Status": "OK"
}
```

{{< /tab >}}
{{< /tabs >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "UpdateDocumentParagraphRunFont.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostDocumentParagraphRunFont.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "post_document_paragraph_run_font.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "post_document_paragraph_run_font.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postDocumentParagraphRunFont.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostDocumentParagraphRunFont.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostDocumentParagraphRunFont.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "PostDocumentParagraphRunFont.go" >}}
{{< /tab >}}
{{< /tabs >}}
