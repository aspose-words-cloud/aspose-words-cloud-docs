---
title: "Update Style on Document Element"
type: docs
url: /update-style-on-document-element/
aliases: [/update-style-on-document-element/]
keywords: "List of Sections,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents,Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "This REST API allows you to Update Style on Document Element. Please note that the SDKs of this cloud API are available in Python, C#, Java, Ruby, PHP, Node.js, Android, Swift, and Go languages."
weight: 20
---

This REST API allows you to Update Style on Document Element. Please note that the SDKs of this cloud API are available in *Python, C#, Java, Ruby, PHP, Node.js, Android, Swift,* and *Go* languages.

## Resource URI

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Styles/UpdateStyle) lets you call this REST API directly from a browser.  

## cURL Example

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

// cURL example to get a list of sections
curl -X PUT "https://api.aspose.cloud/v4.0/words/Run.doc/styles/Heading%201/update?storage=First%20Storage" 

-H  "accept: application/json" -H  "Authorization: Bearer <jwt tokon>" 

-H  "Content-Type: application/json" 

-d "{\"IsQuickStyle\":true,\"Name\":\"My Style\"}"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
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
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "UpdateStyle.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "UpdateStyle.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "UpdateStyle.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "UpdateStyle.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "UpdateStyle.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "UpdateStyle.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "UpdateStyle.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "UpdateStyle.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "updateStyle.go" >}}
{{< /tab >}}
{{< /tabs >}}

