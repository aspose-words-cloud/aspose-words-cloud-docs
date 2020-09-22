---
title: "Update Font Properties of the Text"
type: docs
url: /update-font-properties-of-the-text/
aliases: [/update-font-properties-of-the-text/]
weight: 70
---

This article explains how to format the text. Using [PUT /words/{name}/{paragraphPath}/runs/{index}/font](https://apireference.aspose.cloud/words/#/Runs/UpdateRunFont) API you can update font properties of the text.

## Resource URI

~/{file-name}/{paragraphPath}/runs/{index}/font

*{file-name}* is the name of the Word document containing elements.

*{paragraphPath}* is the path to specific paragraph in the document. Supported syntax:

- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

*{index}* is the index of specific run.

## Resource Properties

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

## cURL Example

Input Document: [SampleWordDocument.docx](attachments/885279/1180112.docx)

Output Document: [ResultWordDocument.docx](attachments/885279/1180113.docx)

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to update Font Properties

curl -v "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/2/runs/0/font?destFileName=ResultWordDocument.docx" \
-X PUT \
-d "{'Bold':true, 'Size': 31.0, 'Name': 'Calibri'}" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
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
         "Href":"http://api.aspose.cloud/v4.0/words/ResultWordDocument.docx/sections/0/paragraphs/2/runs/0/font",
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
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
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
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "UpdateDocumentParagraphRunFont.go" >}}
{{< /tab >}}
{{< /tabs >}}
