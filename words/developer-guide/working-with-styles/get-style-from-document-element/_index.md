---
title: "Get Style from Document Element"
type: docs
url: /get-style-from-document-element/
aliases: [/get-style-from-document-element/]
keywords: "List of Sections,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents,Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "This REST API allows you to Get Style from Document Element. Please note that the SDKs of this cloud API are available in Python, C#, Java, Ruby, PHP, Node.js, Android, Swift, and Go languages."
weight: 30
---

This REST API allows you to Get Style from Document Element. Please note that the SDKs of this cloud API are available in *Python, C#, Java, Ruby, PHP, Node.js, Android, Swift,* and *Go* languages.

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Styles/GetStyle) lets you call this REST API directly from the browser.  

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

curl -X GET "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/style/Heading%201/update?storage=First%20Storage" 

-H  "accept: application/json" -H  "Authorization: Bearer <jwt tokon>" 

-H  "Content-Type: application/json" 

```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
{
  "Styles": [
    {
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
        "Name": "Segoe UI",
        "NameAscii": "Segoe UI",
        "NameBi": "Segoe UI",
        "NameFarEast": "Arial Unicode MS",
        "NameOther": "Segoe UI",
        "NoProofing": false,
        "Outline": false,
        "Position": 0,
        "Scaling": 100,
        "Shadow": false,
        "Size": 9,
        "SizeBi": 9,
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
      "NextParagraphStyleName": "Balloon Text",
      "BaseStyleName": "Normal",
      "IsQuickStyle": false,
      "LinkedStyleName": "Balloon Text Char",
      "Type": "Paragraph",
      "IsHeading": false,
      "StyleIdentifier": "BalloonText",
      "Name": "Balloon Text",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Balloon Text",
        "Rel": "self"

      }
    },
    {
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
        "Name": "Segoe UI",
        "NameAscii": "Segoe UI",
        "NameBi": "Segoe UI",
        "NameFarEast": "Arial Unicode MS",
        "NameOther": "Segoe UI",
        "NoProofing": false,
        "Outline": false,
        "Position": 0,
        "Scaling": 100,
        "Shadow": false,
        "Size": 9,
        "SizeBi": 9,
        "SmallCaps": false,
        "Spacing": 0,
        "StrikeThrough": false,
        "StyleIdentifier": "User",
        "StyleName": "Balloon Text Char",
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
      "NextParagraphStyleName": "Balloon Text Char",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "Balloon Text",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "User",
      "Name": "Balloon Text Char",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Balloon Text Char",
        "Rel": "self"

      }
    },
    {
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
          "Web": "#000000"

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
        "Name": "Helvetica",
        "NameAscii": "Helvetica",
        "NameBi": "Arial Unicode MS",
        "NameFarEast": "Times New Roman",
        "NameOther": "Arial Unicode MS",
        "NoProofing": false,
        "Outline": false,
        "Position": 0,
        "Scaling": 100,
        "Shadow": false,
        "Size": 11,
        "SizeBi": 11,
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
      "NextParagraphStyleName": "Body",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "",
      "Type": "Paragraph",
      "IsHeading": false,
      "StyleIdentifier": "User",
      "Name": "Body",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Body",
        "Rel": "self"

      }
    },
    {
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
        "Size": 8,
        "SizeBi": 8,
        "SmallCaps": false,
        "Spacing": 0,
        "StrikeThrough": false,
        "StyleIdentifier": "CommentReference",
        "StyleName": "Comment Reference",
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
      "NextParagraphStyleName": "Comment Reference",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "CommentReference",
      "Name": "Comment Reference",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Comment Reference",
        "Rel": "self"

      }
    },
    {
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
        "Size": 10,
        "SizeBi": 10,
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
      "NextParagraphStyleName": "Comment Text",
      "BaseStyleName": "Comment Text",
      "IsQuickStyle": false,
      "LinkedStyleName": "Comment Subject Char",
      "Type": "Paragraph",
      "IsHeading": false,
      "StyleIdentifier": "CommentSubject",
      "Name": "Comment Subject",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Comment Subject",
        "Rel": "self"

      }
    },
    {
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
        "Size": 10,
        "SizeBi": 10,
        "SmallCaps": false,
        "Spacing": 0,
        "StrikeThrough": false,
        "StyleIdentifier": "User",
        "StyleName": "Comment Subject Char",
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
      "NextParagraphStyleName": "Comment Subject Char",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "Comment Subject",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "User",
      "Name": "Comment Subject Char",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Comment Subject Char",
        "Rel": "self"

      }
    },
    {
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
        "Size": 10,
        "SizeBi": 10,
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
      "NextParagraphStyleName": "Comment Text",
      "BaseStyleName": "Normal",
      "IsQuickStyle": false,
      "LinkedStyleName": "Comment Text Char",
      "Type": "Paragraph",
      "IsHeading": false,
      "StyleIdentifier": "CommentText",
      "Name": "Comment Text",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Comment Text",
        "Rel": "self"

      }
    },
    {
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
        "Size": 10,
        "SizeBi": 10,
        "SmallCaps": false,
        "Spacing": 0,
        "StrikeThrough": false,
        "StyleIdentifier": "User",
        "StyleName": "Comment Text Char",
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
      "NextParagraphStyleName": "Comment Text Char",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "Comment Text",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "User",
      "Name": "Comment Text Char",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Comment Text Char",
        "Rel": "self"

      }
    },
    {
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
        "Size": 10,
        "SizeBi": 10,
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
      "NextParagraphStyleName": "Default Paragraph Font",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "DefaultParagraphFont",
      "Name": "Default Paragraph Font",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Default Paragraph Font",
        "Rel": "self"

      }
    },
    {
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
      "LinkedStyleName": "Footer Char",
      "Type": "Paragraph",
      "IsHeading": false,
      "StyleIdentifier": "Footer",
      "Name": "Footer",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Footer",
        "Rel": "self"

      }
    },
    {
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
        "StyleIdentifier": "User",
        "StyleName": "Footer Char",
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
      "NextParagraphStyleName": "Footer Char",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "Footer",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "User",
      "Name": "Footer Char",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Footer Char",
        "Rel": "self"

      }
    },
    {
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
      "NextParagraphStyleName": "Header",
      "BaseStyleName": "Normal",
      "IsQuickStyle": false,
      "LinkedStyleName": "Header Char",
      "Type": "Paragraph",
      "IsHeading": false,
      "StyleIdentifier": "Header",
      "Name": "Header",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Header",
        "Rel": "self"

      }
    },
    {
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
        "StyleIdentifier": "User",
        "StyleName": "Header Char",
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
      "NextParagraphStyleName": "Header Char",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "Header",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "User",
      "Name": "Header Char",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Header Char",
        "Rel": "self"

      }
    },
    {
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
      "BuiltIn": true,
      "NextParagraphStyleName": "Normal",
      "BaseStyleName": "Normal",
      "IsQuickStyle": true,
      "LinkedStyleName": "Heading 1 Char",
      "Type": "Paragraph",
      "IsHeading": true,
      "StyleIdentifier": "Heading1",
      "Name": "Heading 1",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Heading 1",
        "Rel": "self"

      }
    },
    {
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
        "StyleIdentifier": "User",
        "StyleName": "Heading 1 Char",
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
      "NextParagraphStyleName": "Heading 1 Char",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "Heading 1",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "User",
      "Name": "Heading 1 Char",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Heading 1 Char",
        "Rel": "self"

      }
    },
    {
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
        "Size": 10,
        "SizeBi": 10,
        "SmallCaps": false,
        "Spacing": 0,
        "StrikeThrough": false,
        "StyleIdentifier": "Hyperlink",
        "StyleName": "Hyperlink",
        "Subscript": false,
        "Superscript": false,
        "TextEffect": "None",
        "Underline": "Single",
        "UnderlineColor": {
          "Web": "",
          "Alpha": 0

        }
      },
      "BuiltIn": true,
      "NextParagraphStyleName": "Hyperlink",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "Hyperlink",
      "Name": "Hyperlink",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Hyperlink",
        "Rel": "self"

      }
    },
    {
      "BuiltIn": true,
      "NextParagraphStyleName": "No List",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "",
      "Type": "List",
      "IsHeading": false,
      "StyleIdentifier": "NoList",
      "Name": "No List",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/No List",
        "Rel": "self"

      }
    },
    {
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
      "NextParagraphStyleName": "Normal",
      "BaseStyleName": "",
      "IsQuickStyle": true,
      "LinkedStyleName": "",
      "Type": "Paragraph",
      "IsHeading": false,
      "StyleIdentifier": "Normal",
      "Name": "Normal",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Normal",
        "Rel": "self"

      }
    },
    {
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
        "Size": 10,
        "SizeBi": 10,
        "SmallCaps": false,
        "Spacing": 0,
        "StrikeThrough": false,
        "StyleIdentifier": "PageNumber",
        "StyleName": "Page Number",
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
      "NextParagraphStyleName": "Page Number",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "",
      "Type": "Character",
      "IsHeading": false,
      "StyleIdentifier": "PageNumber",
      "Name": "Page Number",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Page Number",
        "Rel": "self"

      }
    },
    {
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
        "Size": 10,
        "SizeBi": 10,
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
      "NextParagraphStyleName": "Table Normal",
      "BaseStyleName": "",
      "IsQuickStyle": false,
      "LinkedStyleName": "",
      "Type": "Table",
      "IsHeading": false,
      "StyleIdentifier": "TableNormal",
      "Name": "Table Normal",
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/styles/Table Normal",
        "Rel": "self"

      }
    }
  ],
  "RequestId": "Root=1-5ee50b16-18036ec0d0b34f0c1810c8e0"

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
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "GetStyle.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetStyle.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetStyle.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetStyle.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "GetStyle.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "GetStyle.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "GetStyle.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "GetStyle.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetStyle.go" >}}
{{< /tab >}}
{{< /tabs >}}
