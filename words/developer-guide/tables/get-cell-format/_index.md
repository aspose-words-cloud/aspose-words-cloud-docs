---
title: "Get a Table Cell Format"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /tables/get-cell-format/
aliases: [/get-a-table-cell-format/]
description: "Get table's cell formatting properties in a Word document"
weight: 120
---

This REST API retrieves table's `Cell` formatting properties.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|BottomPadding|double|Specifies the amount of space (in points) to add below the contents of the cell.|
|FitText|bool|If true, fits text in the cell, compressing each paragraph to the width of the cell.|
|HorizontalMerge|CellMerge|Specifies how the cell is merged horizontally with other cells in the row.|
|LeftPadding|double|Specifies the amount of space (in points) to add to the left of the contents of the cell.|
|Orientation|TextOrientation|Specifies the orientation of text in a table cell.|
|PreferredWidth|PreferredWidth|Specifies the preferred width of the cell.|
|RightPadding|double|Specifies the amount of space (in points) to add to the right of the contents of the cell.|
|TopPadding|double|Specifies the amount of space (in points) to add above the contents of the cell.|
|VerticalAlignment|CellVerticalAlignment|Specifies the vertical alignment of text in the cell.|
|VerticalMerge|CellMerge|Specifies how the cell is merged with other cells vertically.|
|Width|double|Gets the width of the cell in points.|
|WrapText|bool|If true, wrap the text for the cell.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/GetTableCellFormat) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [TablesGet.docx](/words/tables/TablesGet.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get table cell's properties
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0/cells/0/cellformat" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "CellFormat": {
    "BottomPadding": 1.0,
    "FitText": false,
    "HorizontalMerge": "None",
    "LeftPadding": 4.0,
    "Orientation": "Horizontal",
    "PreferredWidth": {
      "Type": "Points",
      "Value": 165.1
    },
    "RightPadding": 5.0,
    "TopPadding": 6.0,
    "VerticalAlignment": "Top",
    "VerticalMerge": "None",
    "Width": 165.05,
    "WrapText": true,
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/0/cellformat",
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
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetTableCellFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetTableCellFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetTableCellFormat.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetTableCellFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetTableCellFormat.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
