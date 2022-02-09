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
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetBordersOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetBordersOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
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
      "Href": "https://api.aspose.cloud/v4.0/words/TablesGet.docx/sections/0/tables/1/rows/0/borders",
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
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetBordersOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetBordersOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetBordersOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetBordersOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetBordersOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetBordersOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetBordersOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetBordersOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetBordersOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetBordersOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
