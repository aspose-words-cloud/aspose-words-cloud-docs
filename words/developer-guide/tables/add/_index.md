---
title: "Add Table to a Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /tables/add/
aliases: [/add-table-to-a-document/]
description: "Add a table to a Word document"
weight: 30
---

This REST API adds a `Table` to a document.

The important API parameters are:

|Parameter Name|Type|Description|
| :- | :- | :- |
|ColumnsCount|int|Count of columns. The default is 2.|
|RowsCount|int|Count of rows. The default is 2.|
|Position|DocumentPosition|A table will be inserted before the specified position.|

## Usage examples with cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "InsertTableOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "InsertTableOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "Table": {
    "TableRowList": [
      {
        "TableCellList": [
          {
            "ChildNodes": [
              {
                "Text": "",
                "NodeId": "0.9.0.0.0",
                "link": {
                  "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/0/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.0.0",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/0",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          },
          {
            "ChildNodes": [
              {
                "Text": "",
                "NodeId": "0.9.0.1.0",
                "link": {
                  "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/1/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.0.1",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/1",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          },
          {
            "ChildNodes": [
              {
                "Text": "",
                "NodeId": "0.9.0.2.0",
                "link": {
                  "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/2/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.0.2",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/2",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          }
        ],
        "RowFormat": {
          "Height": 0.0,
          "HeightRule": "Auto",
          "AllowBreakAcrossPages": true,
          "HeadingFormat": false,
          "link": {
            "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/rowformat",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        },
        "NodeId": "0.9.0",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "TableCellList": [
          {
            "ChildNodes": [
              {
                "Text": "",
                "NodeId": "0.9.1.0.0",
                "link": {
                  "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/0/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.1.0",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/0",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          },
          {
            "ChildNodes": [
              {
                "Text": "",
                "NodeId": "0.9.1.1.0",
                "link": {
                  "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/1/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.1.1",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/1",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          },
          {
            "ChildNodes": [
              {
                "Text": "",
                "NodeId": "0.9.1.2.0",
                "link": {
                  "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/2/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.1.2",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/2",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          }
        ],
        "RowFormat": {
          "Height": 0.0,
          "HeightRule": "Auto",
          "AllowBreakAcrossPages": true,
          "HeadingFormat": false,
          "link": {
            "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/rowformat",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        },
        "NodeId": "0.9.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "TableCellList": [
          {
            "ChildNodes": [
              {
                "Text": "",
                "NodeId": "0.9.2.0.0",
                "link": {
                  "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/0/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.2.0",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/0",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          },
          {
            "ChildNodes": [
              {
                "Text": "",
                "NodeId": "0.9.2.1.0",
                "link": {
                  "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/1/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.2.1",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/1",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          },
          {
            "ChildNodes": [
              {
                "Text": "",
                "NodeId": "0.9.2.2.0",
                "link": {
                  "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/2/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.2.2",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/2",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          }
        ],
        "RowFormat": {
          "Height": 0.0,
          "HeightRule": "Auto",
          "AllowBreakAcrossPages": true,
          "HeadingFormat": false,
          "link": {
            "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/rowformat",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        },
        "NodeId": "0.9.2",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "TableProperties": {
      "Alignment": "Left",
      "AllowAutoFit": true,
      "Bidi": false,
      "BottomPadding": 0.0,
      "CellSpacing": 0.0,
      "LeftIndent": 0.0,
      "LeftPadding": 5.4,
      "PreferredWidth": {
        "Type": "Percent",
        "Value": 100.0
      },
      "RightPadding": 5.4,
      "StyleIdentifier": "TableNormal",
      "StyleName": "Table Normal",
      "StyleOptions": "Default",
      "TextWrapping": "None",
      "TopPadding": 0.0,
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/properties",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "NodeId": "0.9",
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4",
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

Using SDK is the quickest way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Usage examples in Python, Java, C#, etc.

The following code samples show how to interact with REST API using almost any mainstream programming language. You can find a lot of other code examples in [Python](https://gist.github.com/aspose-words-cloud-gists/e26813ced70692c544820cd8011ee7e0), [Java](https://gist.github.com/aspose-words-cloud-gists/caede439bfd2e57c3010befe504faff4), [C#](https://gist.github.com/aspose-words-cloud-gists/374e1e3dd4bca8f696f29d913645f549), [JavaScript](https://gist.github.com/aspose-words-cloud-gists/a9510e4b51613f1138e7c1ec09634c4a), [PHP](https://gist.github.com/aspose-words-cloud-gists/e2a72445b96362dc0117f06ab54bb94a), [C++](https://gist.github.com/aspose-words-cloud-gists/49aa5151a094849179bae8672c887a0e), [Golang](https://gist.github.com/aspose-words-cloud-gists/625ca80adffd779e8f6e3611551e14d5), [Ruby](https://gist.github.com/aspose-words-cloud-gists/339f3835a4c0a536c81ec941de29baf7), [Swift](https://gist.github.com/aspose-words-cloud-gists/790dbd2edd5d36f170732366f52cac4c), [Dart](https://gist.github.com/aspose-words-cloud-gists/6aae628cf2b878b78fea177c3171c6bf) on GitHub. All codes are thoroughly tested and ready for production use.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "InsertTableOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "InsertTableOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "InsertTableOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "InsertTableOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "InsertTableOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "InsertTableOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "InsertTableOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "InsertTableOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "InsertTableOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "InsertTableOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
