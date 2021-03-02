---
title: "Update Properties"
second_title: "Paragraphs in a Document"
type: docs
url: /paragraphs/update/
aliases: [/update-paragraph-format-properties/]
description: "Update paragraph formatting properties in a Word document"
weight: 130
---

This REST API updates `Paragraph` formatting properties.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|AddSpaceBetweenFarEastAndAlpha|bool|Specifies a flag indicating whether inter-character spacing is automatically adjusted between regions of Latin text and regions of East Asian text in the current paragraph.|
|AddSpaceBetweenFarEastAndDigit|bool|Specifies a flag indicating whether inter-character spacing is automatically adjusted between regions of numbers and regions of East Asian text in the current paragraph.|
|Alignment|Aspose.Words.ParagraphAlignment|Specifies text alignment for the paragraph.|
|Bidi|bool|Specifies whether this is a right-to-left paragraph.|
|DropCapPosition|Aspose.Words.DropCapPosition|Specifies the position for a drop cap text.|
|FirstLineIndent|double|Specifies the value (in points) for a first-line or hanging indent. Use a positive value to set the first-line indent, and use a negative value to set a hanging indent.|
|KeepTogether|bool|True if all lines in the paragraph are to remain on the same page.|
|KeepWithNext|bool|True if the paragraph is to remains on the same page as the paragraph that follows it.|
|LeftIndent|double|Specifies the value (in points) that represents the left indent for a paragraph.|
|LineSpacing|double|Specifies the line spacing (in points) for the paragraph.|
|LineSpacingRule|Aspose.Words.LineSpacingRule|Specifies the line spacing for the paragraph.|
|LinesToDrop|int|Specifies the number of lines of the paragraph text used to calculate the drop cap-height.|
|NoSpaceBetweenParagraphsOfSameStyle|bool|When true, "SpaceBefore" and "SpaceAfter" will be ignored between the paragraphs of the same style.|
|OutlineLevel|Aspose.Words.OutlineLevel|Specifies the outline level of the paragraph in the document.|
|PageBreakBefore|bool|True if a page break is forced before the paragraph.|
|RightIndent|bool|Specifies the value (in points) that represents the right indent for a paragraph.|
|SpaceAfter|double|Specifies the amount of spacing (in points) after the paragraph.|
|SpaceAfterAuto|bool|True if the amount of spacing after the paragraph is set automatically.|
|SpaceBefore|double|Specifies the amount of spacing (in points) before the paragraph.|
|SpaceBeforeAuto|bool|True if the amount of spacing before the paragraph is set automatically.|
|StyleIdentifier|Aspose.Words.StyleIdentifier|Specifies the locale-independent style identifier of the paragraph style applied to this formatting.|
|StyleName|string|Specifies the name of the paragraph style applied to this formatting.|
|SuppressAutoHyphens|bool|Specifies whether the current paragraph should be exempted from any hyphenation which is applied in the document settings.|
|SuppressLineNumbers|bool|Specifies whether the current paragraph's lines should be exempted from line numbering which is applied in the parent section.|
|WidowControl|bool|True if the first and last lines in the paragraph are to remain on the same page as the rest of the paragraph.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/UpdateParagraphFormat) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to update paragraph's page formatting properties
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/paragraphs/0/format" \
-X PUT \
-d "{ 'Alignment': 'Right' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "ParagraphFormat": {
    "AddSpaceBetweenFarEastAndAlpha": true,
    "AddSpaceBetweenFarEastAndDigit": true,
    "Alignment": "Right",
    "Bidi": false,
    "DropCapPosition": "None",
    "FirstLineIndent": 0.0,
    "KeepTogether": false,
    "KeepWithNext": false,
    "LeftIndent": 0.0,
    "LineSpacing": 12.0,
    "LineSpacingRule": "Multiple",
    "LinesToDrop": 0,
    "NoSpaceBetweenParagraphsOfSameStyle": false,
    "OutlineLevel": "BodyText",
    "PageBreakBefore": false,
    "RightIndent": 0.0,
    "SpaceAfter": 0.0,
    "SpaceAfterAuto": false,
    "SpaceBefore": 0.0,
    "SpaceBeforeAuto": false,
    "StyleIdentifier": "Normal",
    "StyleName": "Normal",
    "SuppressAutoHyphens": false,
    "SuppressLineNumbers": false,
    "WidowControl": true,
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/0/paragraphs/0/format",
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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="5" tabID="4" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "PostDocumentParagraphFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateParagraphFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateParagraphFormat.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_PostDocumentParagraphFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_PostDocumentParagraphFormat.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
