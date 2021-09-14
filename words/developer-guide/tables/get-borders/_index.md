---
title: "Get a List of Borders"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /tables/get-borders/
aliases: [/get-a-list-of-borders/]
description: "Get a list of table's borders in a Word document"
weight: 80
---

This REST API retrieves a collection of tables's `Border` items.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Borders/GetBorders) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [TablesGet.docx](/words/tables/TablesGet.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
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
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the quickest way for a developer to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="5" tabID="4" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetBorders.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetBorders.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetBorders.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "GetBorders.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetBorders.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
