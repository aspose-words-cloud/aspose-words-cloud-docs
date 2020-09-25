---
title: "Get a Table Cell"
type: docs
url: /tables/get-cell/
aliases: [/get-a-table-cell/]
weight: 110
---

This REST API allows you to get a table cell. The API returns a JSON/XML representation of one of the cells contained in the table.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Tables/GetTableCell) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL, supplied with a sample **Input Document** [TablesGet.docx](/words/tables/TablesGet.docx).

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a table cell
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0/cells/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Cell": {
    "ChildNodes": [
      {
        "Text": "34",
        "NodeId": "0.4.0.0.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/0/paragraphs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "NodeId": "0.4.0.0",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/0",
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

Using an SDK is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetTableCell.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetTableCell.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_table_cell.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_table_cell.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getTableCell.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetTableCell.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetTableCell.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetTableCell.go" >}}
{{< /tab >}}
{{< /tabs >}}
