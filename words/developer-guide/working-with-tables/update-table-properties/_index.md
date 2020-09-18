---
title: "Update Table Properties"
type: docs
url: /update-table-properties/
aliases: [/update-table-properties/]
weight: 60
---

## Introduction
This REST API allows you to update table properties and returns updated data in XML/JSON format. The description of the important table properties is given below:

|**Property Name**|**Type**|**Description**|
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
|TopPadding|double|Specifies the amount of space (in points) to add above the contents of cells.|
## Resource URI
[Swagger UI](https://apireference.aspose.cloud/words/#/Tables/UpdateTableProperties) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there.
## cURL Example
**Input Document:** [TablesGet.docx](attachments/885355/1180119.docx)

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to update table's properties

curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/properties" \
-X PUT \
-d "{ 'Alignment': 'Right', 'AllowAutoFit': 'false', 'Bidi': 'true', 'BottomPadding': '1', 'CellSpacing': '2', 'LeftIndent': '3', 'LeftPadding': '4', 'RightPadding': '5', 'StyleOptions': 'ColumnBands', 'TopPadding': '6' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Properties": {

    "Alignment": "Right",

    "AllowAutoFit": false,

    "Bidi": true,

    "BottomPadding": 1.0,

    "CellSpacing": 2.0,

    "LeftIndent": 3.0,

    "LeftPadding": 4.0,

    "PreferredWidth": {

      "Type": "Auto",

      "Value": 0.0

    },

    "RightPadding": 5.0,

    "StyleIdentifier": "TableGrid",

    "StyleName": "Table Grid",

    "StyleOptions": "ColumnBands",

    "TextWrapping": "None",

    "TopPadding": 6.0,

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
## SDK Source
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## SDK Examples
{{< tabs tabTotal="7" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "UpdateTableProperties.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "UpdateTableProperties.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "update_table_properties.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "update_table_properties.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "updateTableProperties.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_UpdateTableProperties.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetTableProperties.swift" >}}

{{< /tab >}}

{{< /tabs >}}
