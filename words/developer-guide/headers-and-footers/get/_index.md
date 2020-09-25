---
title: "Get"
second_title: "Headers and Footers in a Document"
type: docs
url: /headers-and-footers/get/
aliases: [/get-a-header-or-footer-in-a-document/]
weight: 40
---

This REST API allows you to get a header/footer that is contained in a document.

## REST API

```JAVA
~/{file-name}/headersFooters/{index}
~/{file-name}/sections/{sectionIndex}/headersFooters/{index}
```

- *{file-name}* is the name of a Word document containing elements.
- *{sectionIndex}* is the index of a section that contains headers and footers. If this syntax is used, only elements within a specified section are returned.
- *{index}* is the index of specific header/footer.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/HeadersFooters/GetHeaderFooter) lets you call this REST API directly from a browser. 

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

**Case 1**: Get a Header or Footer in a Document

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get an individual header/footer in a document
curl -v "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/headersfooters/0" \
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
  "HeaderFooter": {
    "Paragraphs": {
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/0/paragraphs",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "DrawingObjects": {
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/0/drawingObjects",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "Type": "HeaderEven",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/0",
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

**Case 2**: Get a Header or Footer in a Section

{{< tabs tabTotal="2" tabID="5" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to get an individual header/footer in a section
curl -v "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
{
  "HeaderFooter": {
    "Paragraphs": {
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/0/paragraphs",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "DrawingObjects": {
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/0/drawingObjects",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "Type": "HeaderEven",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/0",
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

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

**Case 1: Get a Header or Footer in a Document**

{{< tabs tabTotal="9" tabID="8" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetHeaderFooter.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetHeaderFooter.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetHeaderFooter.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetHeaderFooter.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetHeaderFooter.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetHeaderFooter.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetHeaderFooter.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetHeaderFooter.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetHeaderFooters.go" >}}
{{< /tab >}}
{{< /tabs >}}

**Case 2: Get a Header or Footer in a Section**

{{< tabs tabTotal="9" tabID="9" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetHeaderFooterOfSection.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetHeaderFooterOfSection.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetHeaderFooterOfSection.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetHeaderFooterOfSection.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetHeaderFooterOfSection.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetHeaderFooterOfSection.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetHeaderFooterOfSection.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetHeaderFooterOfSection.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetHeaderFooterOfSection.go" >}}
{{< /tab >}}
{{< /tabs >}}
