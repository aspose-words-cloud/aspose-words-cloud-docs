---
title: "Get a Table"
type: docs
url: /tables/get/
aliases: [/get-a-table/]
weight: 100
---

This REST API allows you to get JSON/XML representation of one of the tables.

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/GetTable) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL. You can use a sample **Input Document** [TablesGet.docx](/words/tables/TablesGet.docx).

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a table
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

To get a JWT-token, please, follow these [instructions](/words/getting-started/available-sdks/#curl).

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
                "Text": "21",
                "NodeId": "0.3.0.0.0",
                "link": {
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/0/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.3.0.0",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/0",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          },
          {
            "ChildNodes": [
              {
                "Text": "22",
                "NodeId": "0.3.0.1.0",
                "link": {
                  "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/1/paragraphs/0",
                  "Rel": "self",
                  "Type": null,
                  "Title": null
                }
              }
            ],
            "NodeId": "0.3.0.1",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/1",
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
            "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/rowformat",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        },
        "NodeId": "0.3.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0",
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
        "Type": "Auto",
        "Value": 0.0
      },
      "RightPadding": 5.4,
      "StyleIdentifier": "TableGrid",
      "StyleName": "Table Grid",
      "StyleOptions": "Default",
      "TextWrapping": "None",
      "TopPadding": 0.0,
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/properties",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "NodeId": "0.3",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1",
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
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetTable.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetTable.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_table.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_table.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getTable.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetTable.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetTable.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetTable.go" >}}
{{< /tab >}}
{{< /tabs >}}
