---
title: "Update a Table Cell Format"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /tables/update-cell-format/
aliases: [/update-a-table-cell-format/]
description: "Update table's cell formatting properties in a Word document"
weight: 180
---

This REST API updates table's cell formatting properties.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|BottomPadding|double|Specifies the amount of space (in points) to add below the contents of the cell.|
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

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/UpdateTableCellFormat) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [TablesGet.docx](/words/tables/TablesGet.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to update table cell's format properties
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0/cells/0/cellformat" \
-X PUT \
-d "{ 'BottomPadding': '1', 'FitText': 'true', 'HorizontalMerge': 'First', 'LeftPadding': '2', 'Orientation': 'VerticalFarEast', 'RightPadding': '3', 'TopPadding': '4.5', 'VerticalAlignment': 'Center', 'VerticalMerge': 'Previous', 'Width': '11', 'WrapText': 'false' }" \
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
    "FitText": true,
    "HorizontalMerge": "First",
    "LeftPadding": 2.0,
    "Orientation": "VerticalFarEast",
    "PreferredWidth": {
      "Type": "Points",
      "Value": 11.0
    },
    "RightPadding": 3.0,
    "TopPadding": 4.5,
    "VerticalAlignment": "Center",
    "VerticalMerge": "Previous",
    "Width": 11.0,
    "WrapText": false,
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/0/cellformat",
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
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "UpdateTableCellFormatOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "UpdateTableCellFormatOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "UpdateTableCellFormatOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateTableCellFormatOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "UpdateTableCellFormatOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "UpdateTableCellFormatOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateTableCellFormatOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "UpdateTableCellFormatOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "UpdateTableCellFormatOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "UpdateTableCellFormatOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
