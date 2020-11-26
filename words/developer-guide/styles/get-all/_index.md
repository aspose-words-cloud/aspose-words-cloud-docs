---
title: "Get Styles from Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /styles/get-all/
aliases: [/get-styles-from-document/]
keywords: ""
description: "Get styles in a Word document"
weight: 40
---

This REST API retrieves all `Style` items from a document.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Styles/GetStyles) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X GET "https://api.aspose.cloud/v4.0/words/TestGetStyleFromDocumentElement.docx/paragraphs%2F1%2FparagraphFormat/style?storage=First%20Storage"

-H  "accept: application/json" -H  "Authorization: Bearer <jwt tokon>" 

-H  "Content-Type: application/json" 
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Style": {
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
        "DistanceFromText": 0,
        "LineStyle": "None",
        "LineWidth": 0,
        "Shadow": false
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
      "Italic": false,
      "ItalicBi": false,
      "Kerning": 0,
      "LocaleId": 1033,
      "LocaleIdBi": 1025,
      "LocaleIdFarEast": 1033,
      "Name": "Times New Roman",
      "NameAscii": "Times New Roman",
      "NameBi": "Times New Roman",
      "NameFarEast": "Arial Unicode MS",
      "NameOther": "Times New Roman",
      "NoProofing": false,
      "Outline": false,
      "Position": 0,
      "Scaling": 100,
      "Shadow": false,
      "Size": 12,
      "SizeBi": 12,
      "SmallCaps": false,
      "Spacing": 0,
      "StrikeThrough": false,
      "StyleIdentifier": "DefaultParagraphFont",
      "StyleName": "Default Paragraph Font",
      "Subscript": false,
      "Superscript": false,
      "TextEffect": "None",
      "Underline": "None",
      "UnderlineColor": {
        "Web": "",
        "Alpha": 0
      }
    },
    "BuiltIn": true,
    "NextParagraphStyleName": "Footer",
    "BaseStyleName": "Normal",
    "IsQuickStyle": false,
    "LinkedStyleName": "Нижний колонтитул Знак",
    "Type": "Paragraph",
    "IsHeading": false,
    "StyleIdentifier": "Footer",
    "Name": "Footer",
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyleFromDocumentElement.docx/styles/Footer",
      "Rel": "self"
    }
  },
  "RequestId": "Root=1-5ee50baf-bac5086414fbf000c808a528"
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="4" tabName1="C#" tabName2="PHP" tabName3="Golang" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetStyles.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetStyles.php" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "get-styles.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
