---
title: "Add a Row To a Table"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /tables/add-row/
aliases: [/add-a-row-to-a-table/]
description: "Add a row to a table in a Word document"
weight: 10
---

This REST API adds a `Row` to a `Table`.

The description of important API parameters is given below:

|Parameter Name|Type|Description|
| :- | :- | :- |
|ColumnsCount|int|Count of columns. Default is 1.|
|InsertAfter|int?|Table row will be inserted after a row with specified 0-based index.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/InsertTableRow) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use `cURL` command-line tool to easily interact with Aspose.Words web services. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [TablesGet.docx](/words/tables/TablesGet.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to add a row to table
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows" \
-X POST \
-d "{ 'ColumnsCount': 3 }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Row": {
    "TableCellList": [
      {
        "ChildNodes": [
        ],
        "NodeId": "0.4.2.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/2/cells/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "ChildNodes": [
        ],
        "NodeId": "0.4.2.1",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/2/cells/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "ChildNodes": [
        ],
        "NodeId": "0.4.2.2",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/2/cells/2",
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
        "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/2/rowformat",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "NodeId": "0.4.2",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/2",
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
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "InsertTableRow.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "InsertTableRow.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "insert_table_row.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "insert_table_row.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "insertTableRow.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_InsertTableRow.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_InsertTableRow.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "InsertTableRow.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
