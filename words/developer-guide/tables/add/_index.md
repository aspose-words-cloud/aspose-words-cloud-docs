---
title: "Add Table to a Document"
type: docs
url: /tables/add/
aliases: [/add-table-to-a-document/]
weight: 30
---

This REST API allows you to add a table to a document, and returns added table's data in XML/JSON format. The important API parameters are:

|Parameter Name|Type|Description|
| :- | :- | :- |
|ColumnsCount|int|Count of columns. The default is 2.|
|RowsCount|int|Count of rows. The default is 2.|
|Position|DocumentPosition|A table will be inserted before the specified position.|

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/InsertTable) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

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

<p style="margin:0;font-size:80%;font-style:italic">To get jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

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

## Cloud SDK Family

Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "InsertTable.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "InsertTable.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "insert_table.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "insert_table.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "insertTable.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_InsertTable.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_InsertTable.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "InsertTable.go" >}}
{{< /tab >}}
{{< /tabs >}}
