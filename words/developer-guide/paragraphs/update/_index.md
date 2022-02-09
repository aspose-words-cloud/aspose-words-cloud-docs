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

Important properties are the following:

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

## Usage examples with cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "UpdateParagraphFormatOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "UpdateParagraphFormatOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
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
      "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/0/paragraphs/0/format",
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

## Aspose.Words Cloud SDK Family

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Usage examples in Python, Java, C#, etc.

The following code samples show how to interact with the REST API using almost any mainstream programming language.

You can find a lot of other examples in [Python](https://gist.github.com/aspose-words-cloud-gists/e26813ced70692c544820cd8011ee7e0), [Java](https://gist.github.com/aspose-words-cloud-gists/caede439bfd2e57c3010befe504faff4), [C#](https://gist.github.com/aspose-words-cloud-gists/374e1e3dd4bca8f696f29d913645f549), [JavaScript](https://gist.github.com/aspose-words-cloud-gists/a9510e4b51613f1138e7c1ec09634c4a), [PHP](https://gist.github.com/aspose-words-cloud-gists/e2a72445b96362dc0117f06ab54bb94a), [C++](https://gist.github.com/aspose-words-cloud-gists/49aa5151a094849179bae8672c887a0e), [Golang](https://gist.github.com/aspose-words-cloud-gists/625ca80adffd779e8f6e3611551e14d5), [Ruby](https://gist.github.com/aspose-words-cloud-gists/339f3835a4c0a536c81ec941de29baf7), [Swift](https://gist.github.com/aspose-words-cloud-gists/790dbd2edd5d36f170732366f52cac4c), [Dart](https://gist.github.com/aspose-words-cloud-gists/6aae628cf2b878b78fea177c3171c6bf) on GitHub. All codes are thoroughly tested and ready for production use.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "UpdateParagraphFormatOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "UpdateParagraphFormatOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "UpdateParagraphFormatOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateParagraphFormatOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "UpdateParagraphFormatOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "UpdateParagraphFormatOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateParagraphFormatOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "UpdateParagraphFormatOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "UpdateParagraphFormatOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "UpdateParagraphFormatOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
