---
title: "Reset Borders Properties to Default Values"
type: docs
url: /reset-borders-properties-to-default-values/
aliases: [/reset-borders-properties-to-default-values/]
weight: 200
---

## **Introduction**
The REST API allows you to reset borders properties to default values. 
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Borders/DeleteBorders) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there.
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

// cURL example to reset border properties

curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0/borders" \
-X DELETE \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Borders": {

    "List": [

      {

        "BorderType": "Top",

        "Color": {

          "Web": "",

          "Alpha": 0

        },

        "DistanceFromText": 0.0,

        "LineStyle": "None",

        "LineWidth": 0.0,

        "Shadow": false,

        "link": null

      },

      {

        "BorderType": "Left",

        "Color": {

          "Web": "",

          "Alpha": 0

        },

        "DistanceFromText": 0.0,

        "LineStyle": "None",

        "LineWidth": 0.0,

        "Shadow": false,

        "link": null

      },

      {

        "BorderType": "Bottom",

        "Color": {

          "Web": "",

          "Alpha": 0

        },

        "DistanceFromText": 0.0,

        "LineStyle": "None",

        "LineWidth": 0.0,

        "Shadow": false,

        "link": null

      },

      {

        "BorderType": "Right",

        "Color": {

          "Web": "",

          "Alpha": 0

        },

        "DistanceFromText": 0.0,

        "LineStyle": "None",

        "LineWidth": 0.0,

        "Shadow": false,

        "link": null

      },

      {

        "BorderType": "Horizontal",

        "Color": {

          "Web": "",

          "Alpha": 0

        },

        "DistanceFromText": 0.0,

        "LineStyle": "None",

        "LineWidth": 0.0,

        "Shadow": false,

        "link": null

      },

      {

        "BorderType": "Vertical",

        "Color": {

          "Web": "",

          "Alpha": 0

        },

        "DistanceFromText": 0.0,

        "LineStyle": "None",

        "LineWidth": 0.0,

        "Shadow": false,

        "link": null

      }

    ],

    "link": {

      "Href": "http://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/borders",

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
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "DeleteTableBorders.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "DeleteBorders.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "reset_table_borders_properties.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "delete_borders.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "deleteBorders.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_DeleteBorders.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_DeleteBorders.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "DeleteBorders.go" >}}

{{< /tab >}}

{{< /tabs >}}
