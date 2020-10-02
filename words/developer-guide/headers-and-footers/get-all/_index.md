---
title: "Get all"
second_title: "Headers and Footers in a Document"
type: docs
url: /headers-and-footers/get-all/
aliases: [/get-all-header-and-footers-in-a-document/]
description: "Get all headers and footers in a Word document"
weight: 50
---

This REST API retrieves all Headers and Footers.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/HeadersFooters/GetHeaderFooters) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get all Header and Footers in a Document
curl -v "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/headersfooters" \
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
  "HeaderFooters": {
    "List": [
      {
        "Type": "HeaderEven",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "HeaderPrimary",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "FooterEven",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/2",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "FooterPrimary",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/3",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "HeaderFirst",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/4",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "FooterFirst",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/5",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/headersfooters",
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

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetHeadersFooters.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetAllHeaderFooters.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetAllHeaderFooters.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetAllHeaderFooters.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetAllHeaderFooters.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetAllHeaderFooters.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetAllHeaderFooters.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetAllHeaderFooters.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetHeaderFooters.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
