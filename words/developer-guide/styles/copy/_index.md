---
title: "Copy Style from Document Element"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /styles/copy/
aliases: [/copy-style-from-document-element/]
keywords: ""
description: "Copy a style from an element in a Word document"
weight: 20
---

This REST API copies a `Style` from a document element.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Styles/CopyStyle) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X POST "https://api.aspose.cloud/v4.0/words/TestCopyStyle.docx/styles/copy?storage=First%20Storage" 

-H  "accept: application/json" 

-H  "Authorization: Bearer  

-H  "Content-Type: application/json" -d "{\"StyleName\":\"Heading 1\"}"
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
      "Bold": true,
      "BoldBi": true,
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
      "Kerning": 16,
      "LocaleId": 1033,
      "LocaleIdBi": 1025,
      "LocaleIdFarEast": 1033,
      "Name": "Cambria",
      "NameAscii": "Cambria",
      "NameBi": "Times New Roman",
      "NameFarEast": "Times New Roman",
      "NameOther": "Cambria",
      "NoProofing": false,
      "Outline": false,
      "Position": 0,
      "Scaling": 100,
      "Shadow": false,
      "Size": 16,
      "SizeBi": 16,
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
    "BuiltIn": false,
    "NextParagraphStyleName": "Normal",
    "BaseStyleName": "Normal",
    "IsQuickStyle": true,
    "LinkedStyleName": "Heading 1 Char_1",
    "Type": "Paragraph",
    "IsHeading": false,
    "StyleIdentifier": "User",
    "Name": "Heading 1_1",
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/TestCopyStyle.docx/styles/Heading 1_1",
      "Rel": "self"
    }
  },
  "RequestId": "Root=1-5ee50c07-f937b2b8a85579585f700c2c"
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="0" tabID="4" >}}
{{< /tabs >}}
{{< /nosnippet >}}
