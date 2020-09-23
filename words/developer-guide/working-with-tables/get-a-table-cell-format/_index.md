---
title: "Get a Table Cell Format"
type: docs
url: /get-a-table-cell-format/
aliases: [/get-a-table-cell-format/]
weight: 150
---

This REST API allows you to access the formatting properties of a table cell. The description of important cell properties is:

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

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/GetTableCellFormat) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

*Input Document:** [TablesGet.docx](attachments/885355/1180119.docx)

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to get table cell's properties
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0/cells/0/cellformat" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
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
## SDK Source

Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetTableCellFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetTableCellFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_table_cell_format.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_table_cell_format.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getTableCellFormat.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetTableCellFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetTableCellFormat.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetTableCellFormat.go" >}}
{{< /tab >}}
{{< /tabs >}}
