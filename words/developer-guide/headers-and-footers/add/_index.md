---
title: "Add"
second_title: "Headers and Footers in a Document"
type: docs
url: /headers-and-footers/add/
aliases: [/add-header-or-footer-to-a-document/]
description: "Add headers and footers into a Word document"
weight: 10
---

This REST API adds a Header or a Footer to a document.

The request body should contain a type of header/footer, and the allowed values of headerFooterType are:

|Value|Description|
| :- | :- |
|HeaderEven|The header for even-numbered pages.|
|HeaderPrimary|Primary header, also used for odd-numbered pages|
|FooterEven|Footer for even-numbered pages.|
|FooterPrimary|Primary footer, also used for odd-numbered pages.|
|HeaderFirst|The header for the first page of the section.|
|FooterFirst|Footer for the first page of the section.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/HeadersFooters/InsertHeaderFooter) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to add header/footer to a document
curl -v "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/headersfooters" \
-X PUT \
-d "'HeaderFirst'" \
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
        "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/4/paragraphs",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "DrawingObjects": {
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/4/drawingObjects",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "Type": "HeaderFirst",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/4",
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

{{< nosnippet >}}
{{< tabs tabTotal="8" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Ruby" tabName7="Android" tabName8="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "InsertHeaderFooter.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "InsertHeaderFooter.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "InsertHeaderFooter.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "InsertHeaderFooter.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "InsertHeaderFooter.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "InsertHeaderFooter.rb" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "InsertHeaderFooter.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetHeaderFooter.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
