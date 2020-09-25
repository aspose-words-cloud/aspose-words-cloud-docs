---
title: "Get a List of Borders"
type: docs
url: /tables/get-borders/
aliases: [/get-a-list-of-borders/]
weight: 80
---

The REST API allows you to get a list of borders.

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Borders/GetBorders) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL. To get a **JWT** token, please, follow these [instructions](/words/getting-started/available-sdks/#curl). You can use a sample **Input Document** [TablesGet.docx](/words/tables/TablesGet.docx).

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of borders
curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0/borders" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Borders": {
    "List": [
      {
        "BorderType": "Top",
        "Color": {
          "Web": "#000000"
        },
        "DistanceFromText": 0.0,
        "LineStyle": "Single",
        "LineWidth": 0.5,
        "Shadow": false,
        "link": null
      },
      {
        "BorderType": "Left",
        "Color": {
          "Web": "#000000"
        },
        "DistanceFromText": 0.0,
        "LineStyle": "Single",
        "LineWidth": 0.5,
        "Shadow": false,
        "link": null
      },
      {
        "BorderType": "Bottom",
        "Color": {
          "Web": "#000000"
        },
        "DistanceFromText": 0.0,
        "LineStyle": "Single",
        "LineWidth": 0.5,
        "Shadow": false,
        "link": null
      },
      {
        "BorderType": "Right",
        "Color": {
          "Web": "#000000"
        },
        "DistanceFromText": 0.0,
        "LineStyle": "Single",
        "LineWidth": 0.5,
        "Shadow": false,
        "link": null
      },
      {
        "BorderType": "Horizontal",
        "Color": {
          "Web": "#000000"
        },
        "DistanceFromText": 0.0,
        "LineStyle": "Single",
        "LineWidth": 0.5,
        "Shadow": false,
        "link": null
      },
      {
        "BorderType": "Vertical",
        "Color": {
          "Web": "#000000"
        },
        "DistanceFromText": 0.0,
        "LineStyle": "Single",
        "LineWidth": 0.5,
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

## Cloud SDK Family

Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetTableBorders.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetBorders.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_table_borders.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_borders.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getBorders.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetBorders.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetBorders.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetBorders.go" >}}
{{< /tab >}}
{{< /tabs >}}
