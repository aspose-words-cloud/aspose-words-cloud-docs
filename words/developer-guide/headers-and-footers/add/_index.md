---
title: "Add Header or Footer to a Document"
type: docs
url: /headers-and-footers/add/
aliases: [/add-header-or-footer-to-a-document/]
weight: 30
---

This REST API allows you to add Header or Footer to a document. The API returns the added object's data in XML/JSON format. 

The request body should contain a type of header/footer, and the allowed values of headerFooterType are:

|Value|Description|
| :- | :- |
|HeaderEven|The header for even-numbered pages.|
|HeaderPrimary|Primary header, also used for odd-numbered pages|
|FooterEven|Footer for even-numbered pages.|
|FooterPrimary|Primary footer, also used for odd-numbered pages.|
|HeaderFirst|The header for the first page of the section.|
|FooterFirst|Footer for the first page of the section.|

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/HeadersFooters/InsertHeaderFooter) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to add header/footer to a document
curl -v "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/headersfooters" \
-X PUT \
-d "'HeaderFirst'" \
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

Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "PutHeaderFooter.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PutHeaderFooter.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "PutHeaderFooter.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "PutHeaderFooter.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "PutHeaderFooter.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "PutHeaderFooter.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PutHeaderFooter.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetHeaderFooter.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "PutHeaderFooter.go" >}}
{{< /tab >}}
{{< /tabs >}}
