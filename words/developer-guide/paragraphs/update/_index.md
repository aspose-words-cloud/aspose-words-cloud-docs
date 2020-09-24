---
title: "Update Paragraph Format Properties"
type: docs
url: /paragraphs/update/
aliases: [/update-paragraph-format-properties/]
weight: 60
---

This REST API allows you to update paragraph page formatting properties. The API returns updated data in the XML/JSON format. The resource properties are:

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

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/UpdateParagraphFormat) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to update paragraph's page formatting properties
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/paragraphs/0/format" \
-X PUT \
-d "{ 'Alignment': 'Right' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

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

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "UpdateParagraphFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostDocumentParagraphFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "post_document_paragraph_format.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "post_document_paragraph_format.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postDocumentParagraphFormat.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostDocumentParagraphFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostDocumentParagraphFormat.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "UpdateParagraphFormat.go" >}}
{{< /tab >}}
{{< /tabs >}}
