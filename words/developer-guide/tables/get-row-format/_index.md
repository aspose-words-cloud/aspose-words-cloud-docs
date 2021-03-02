---
title: "Get a Table Row Format"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /tables/get-row-format/
aliases: [/get-a-table-row-format/]
description: "Get table's `Row` formatting properties in a Word document"
weight: 140
---

This REST API retrieves table's `Row` formatting properties.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|Height|double|Specifies the height of the table row in points.|
|HeightRule|HeightRule|Specifies the rule for determining the height of the table row.|
|AllowBreakAcrossPages|bool|True if the text in a table row is allowed to split across a page break.|
|HeadingFormat|bool|True if the row is repeated as a table heading on every page when the table spans more than one page.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/GetTableRowFormat) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [TablesGet.docx](/words/tables/TablesGet.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a table row format
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0/rowformat" \
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
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetTableRow.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetTableRowFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetTableRowFormat.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetTableRow.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetTableRowFormat.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
