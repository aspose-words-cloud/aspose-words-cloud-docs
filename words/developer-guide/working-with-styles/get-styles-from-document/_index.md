---
title: "Get Styles from Document"
type: docs
url: /get-styles-from-document/
aliases: [/get-styles-from-document/]
keywords: "List of Sections,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents,Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "This REST API allows you to Get Styles from Document. Please note that the SDKs of this cloud API are available in Python, C#, Java, Ruby, PHP, Node.js, Android, Swift, and Go languages."
weight: 40
---

## Introduction


This REST API allows you to Get Styles from Document. Please note that the SDKs of this cloud API are available in *Python, C#, Java, Ruby, PHP, Node.js, Android, Swift,* and *Go* languages.
## Resource URI
[Swagger UI](https://apireference.aspose.cloud/words/#/Styles/GetStyles) lets you call this REST API directly from the browser.  
## cURL Example
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get a list of sections

curl -X GET "https://api.aspose.cloud/v4.0/words/TestGetStyleFromDocumentElement.docx/paragraphs%2F1%2FparagraphFormat/style?storage=First%20Storage"

-H  "accept: application/json" -H  "Authorization: Bearer <jwt tokon>" 

-H  "Content-Type: application/json" 

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

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
## SDKs
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## SDK Examples
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "GetStyles.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetStyles.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetStyles.php" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetStyles.py" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "GetStyles.rb" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "GetStyles.js" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "GetStyles.java" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "GetStyles.swift" >}}

{{< /tab >}}

{{< tab tabNum="9" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "get-styles.go" >}}

{{< /tab >}}

{{< /tabs >}}
