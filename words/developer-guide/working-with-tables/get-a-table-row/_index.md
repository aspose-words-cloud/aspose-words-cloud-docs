---
title: "Get a Table Row"
type: docs
url: /get-a-table-row/
weight: 70
---

## **Introduction**
This REST API allows you to get a table row. The API returns a JSON/XML representation of one of the table rows.
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Tables/GetTableRow) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there.
## **cURL Example**
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

// cURL example to get a table row

curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Row": {

    "TableCellList": [

      {

        "ChildNodes": [

          {

            "Text": "31",

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

      {

        "ChildNodes": [

          {

            "Text": "32",

            "NodeId": "0.4.0.1.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/1/paragraphs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          }

        ],

        "NodeId": "0.4.0.1",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/1",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "ChildNodes": [

          {

            "Text": "33",

            "NodeId": "0.4.0.2.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/2/paragraphs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          }

        ],

        "NodeId": "0.4.0.2",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/cells/2",

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

        "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/rowformat",

        "Rel": "self",

        "Type": null,

        "Title": null

      }

    },

    "NodeId": "0.4.0",

    "link": {

      "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0",

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
## **SDK Source**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
{{< tabs tabTotal="7" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetTableRow.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetTableRow.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_table_row.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_table_row.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetTableRow.go" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetTableRow.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetTableRow.swift" >}}

{{< /tab >}}

{{< /tabs >}}
