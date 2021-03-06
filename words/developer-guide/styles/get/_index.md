---
title: "Get Style from Document Element"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /styles/get/
aliases: [/get-style-from-document-element/]
keywords: ""
description: "Get a style from an element in a Word document"
weight: 30
---

This REST API retrieves a `Style` from a document element.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Styles/GetStyle) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -X GET "https://api.aspose.cloud/v4.0/words/TestGetStyles.docx/style/Heading%201/update?storage=First%20Storage" 

-H  "accept: application/json" -H  "Authorization: Bearer <jwt tokon>" 

-H  "Content-Type: application/json" 
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="0" tabID="4" >}}
{{< /tabs >}}
{{< /nosnippet >}}
