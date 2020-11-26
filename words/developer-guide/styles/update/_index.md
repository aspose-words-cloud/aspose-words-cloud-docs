---
title: "Update Style on Document Element"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /styles/update/
aliases: [/update-style-on-document-element/]
keywords: ""
description: "Update a style of a document element in a Word document"
weight: 60
---

This REST API updates a `Style` of a document element.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Styles/UpdateStyle) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X PUT "https://api.aspose.cloud/v4.0/words/Run.doc/styles/Heading%201/update?storage=First%20Storage" 

-H  "accept: application/json" -H  "Authorization: Bearer <jwt tokon>" 

-H  "Content-Type: application/json" 

-d "{\"IsQuickStyle\":true,\"Name\":\"My Style\"}"
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
      "LocaleId": 1049,
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
    "LinkedStyleName": "Heading 1 Char",
    "Type": "Paragraph",
    "IsHeading": false,
    "StyleIdentifier": "User",
    "Name": "My Style",
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/Run.doc/styles/My Style",
      "Rel": "self"
    }
  },
  "RequestId": "Root=1-5ee50a9c-d4e9c3549c123c5088b36aa0"
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
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateStyle.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "UpdateStyle.php" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "updateStyle.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

