---
title: "Update a Table Row Format"
type: docs
url: /update-a-table-row-format/
aliases: [/update-a-table-row-format/]
weight: 110
---

This REST API allows you to update a table row format properties. The description of important row properties is:

|Property Name|Type|Description|
| :- | :- | :- |
|Height|double|Specifies the height of the table row in points.|
|HeightRule|HeightRule|Specifies the rule for determining the height of the table row.|
|AllowBreakAcrossPages|bool|True if the text in a table row is allowed to split across a page break.|
|HeadingFormat|bool|True if the row is repeated as a table heading on every page when the table spans more than one page.|

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Tables/UpdateTableRowFormat) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there.

## cURL Example

**Input Document:** [TablesGet.docx](attachments/885355/1180119.docx)

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to update a table row's format properties

curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0/rowformat" \
-X PUT \
-d "{ 'Height': '10', 'HeightRule': 'Exactly', 'AllowBreakAcrossPages': 'false', 'HeadingFormat': 'true' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
{
  "RowFormat": {
    "Height": 10.0,
    "HeightRule": "Exactly",
    "AllowBreakAcrossPages": false,
    "HeadingFormat": true,
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
## SDK Source

Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "UpdateTableRowFormat.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "UpdateTableRowFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "update_table_row_format.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "update_table_row_format.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "updateTableRowFormat.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_UpdateTableRowFormat.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_UpdateTableRowFormat.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "UpdateTableRowFormat.go" >}}
{{< /tab >}}
{{< /tabs >}}
