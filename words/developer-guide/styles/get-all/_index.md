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

You can use **cURL** and **Postman** to access Aspose.Words Cloud API. The following examples demonstate how to do it. Please refer to the <a href="/words/getting-started/quickstart/">instructions</a> to get a 'JWT_TOKEN' for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetStylesOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetStylesOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
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
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetStylesOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetStylesOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetStylesOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetStylesOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetStylesOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetStylesOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetStylesOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetStylesOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetStylesOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetStylesOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
