---
title: "Get"
second_title: "Headers and Footers in a Document"
type: docs
url: /headers-and-footers/get/
aliases: [/get-a-header-or-footer-in-a-document/]
description: "Get a headers or a footers from a Word document"
weight: 40
---

This REST API retrieves a Header or a Footer.

## REST API

```JAVA
~/{file-name}/headersFooters/{index}
~/{file-name}/sections/{sectionIndex}/headersFooters/{index}
```

- *{file-name}* is the name of a Word document containing elements.
- *{sectionIndex}* is the index of a section that contains headers and footers. If this syntax is used, only elements within a specified section are returned.
- *{index}* is the index of specific header/footer.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/HeadersFooters/GetHeaderFooter) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser. 

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

**Case 1**: Get a Header or Footer in a Document

{{< nosnippet >}}
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
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

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
{{< /nosnippet >}}

**Case 2**: Get a Header or Footer in a Section

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="5" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your `Client Id` and `Secret` credentials from https://dashboard.aspose.cloud/applications.
# Place `Client Id` in client_id argument. Place `Secret` in client_secret argument.
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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

**Case 1: Get a Header or Footer in a Document**

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="8" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetHeaderFooter.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetHeaderFooter.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetHeaderFooter.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetHeaderFooter.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetHeaderFooter.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetHeaderFooters.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetHeaderFooter.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetHeaderFooter.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetHeaderFooter.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

**Case 2: Get a Header or Footer in a Section**

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="9" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetHeaderFooterOfSection.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetHeaderFooterOfSection.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetHeaderFooterOfSection.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetHeaderFooterOfSection.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetHeaderFooterOfSection.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetHeaderFooterOfSection.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetHeaderFooterOfSection.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetHeaderFooterOfSection.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetHeaderFooterOfSection.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
