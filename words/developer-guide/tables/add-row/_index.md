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

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [TablesGet.docx](/words/tables/TablesGet.docx) file designed to act as a demonstration and let you figure out the details quickly.

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
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

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
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "InsertTableRowOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "InsertTableRowOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "InsertTableRowOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "InsertTableRowOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "InsertTableRowOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "InsertTableRowOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "InsertTableRowOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "InsertTableRowOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "InsertTableRowOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "InsertTableRowOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
