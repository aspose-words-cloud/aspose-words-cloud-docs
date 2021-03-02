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

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/InsertTable) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to add table to a document
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables" \
-X POST \
-d "{'ColumnsCount':3, 'RowsCount': 3}" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

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
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/0/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.0.0",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/0",
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
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/1/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.0.1",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/1",
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
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/2/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.0.2",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/cells/2",
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
            "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0/rowformat",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        },
        "NodeId": "0.9.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/0",
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
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/0/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.1.0",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/0",
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
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/1/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.1.1",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/1",
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
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/2/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.1.2",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/cells/2",
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
            "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1/rowformat",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        },
        "NodeId": "0.9.1",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/1",
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
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/0/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.2.0",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/0",
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
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/1/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.2.1",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/1",
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
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/2/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.9.2.2",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/cells/2",
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
            "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2/rowformat",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        },
        "NodeId": "0.9.2",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/rows/2",
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
        "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4/properties",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "NodeId": "0.9",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/4",
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

## Cloud SDK Family

Using an SDK is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="5" tabID="4" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "InsertTable.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "InsertTable.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "InsertTable.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_InsertTable.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_InsertTable.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
