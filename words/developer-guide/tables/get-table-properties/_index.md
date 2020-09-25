---
title: "Get Table Properties"
type: docs
url: /tables/get-table-properties/
aliases: [/get-table-properties/]
weight: 150
---

This REST API allows you to get properties of a table. The description of the important table properties is given below:

|Property Name|Type|Description|
| :- | :- | :- |
|Alignment|TableAlignment|Specifies how an inline table is aligned in the document.|
|AllowAutoFit|bool|Allows Microsoft Word and Aspose.Words to automatically resize cells in a table to fit their contents.|
|Bidi|bool|Specifies whether this is a right-to-left table.|
|BottomPadding|double|Specifies the amount of space (in points) to add below the contents of cells.|
|CellSpacing|double|Specifies the amount of space (in points) between the cells.|
|LeftIndent|double|Specifies the value that represents the left indent of the table.|
|LeftPadding|double|Specifies the amount of space (in points) to add to the left of the contents of cells.|
|PreferredWidth|PreferredWidth|Specifies the table preferred width as a percentage, a number of points or a special "auto" value.|
|RightPadding|double|Specifies the amount of space (in points) to add to the right of the contents of cells.|
|StyleIdentifier|StyleIdentifier|Specifies the local independent style identifier of the table style applied to this table.|
|StyleName|string|Specifies the name of the table style applied to this table.|
|StyleOptions|TableStyleOptions|Specifies bit flags that specify how a table style is applied to this table.|
|TextWrapping|TextWrapping|Specifies TextWrapping for a table.|
|TopPadding|double|Specifies the amount of space (in points) to add above the contents of cells.|

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/GetTableProperties) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL. You can use a sample **Input Document** [TablesGet.docx](/words/tables/TablesGet.docx).

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get table's properties
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/properties" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

To get a **JWT** token, please, follow these [instructions](/words/getting-started/available-sdks/#curl).

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Properties": {
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
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetTableProperties.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetTableProperties.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_table_properties.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_table_properties.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getTableProperties.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetTableProperties.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetTableProperties.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetTableProperties.go" >}}
{{< /tab >}}
{{< /tabs >}}
