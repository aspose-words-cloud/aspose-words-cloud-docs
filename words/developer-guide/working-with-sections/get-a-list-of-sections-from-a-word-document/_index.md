---
title: "Get a List of Sections from a Word Document"
type: docs
url: /get-a-list-of-sections-from-a-word-document/
aliases: [/get-a-list-of-sections-from-a-word-document/]
keywords: "List of Sections,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents,Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "This REST API allows you to get a list of sections or section breaks that are contained in the document. Please note that the SDKs of this cloud API are available in Python, C#, Java, Ruby, PHP, Node.js, Android, Swift and Go languages."
weight: 10
---

This REST API allows you to get a list of sections or section breaks that are contained in the document.

Please note that the SDKs of this Cloud API are available in Python, C#, Java, C++, Ruby, PHP, Node.js, Swift and Go programming languages.

## Resource URI

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Sections/GetSections) lets you call this REST API directly from a browser.

## cURL Example

cUrl is a popular command-line utility for transferring data and a perfect tool for testing REST APIs. The following are a few examples of using cURL.

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get a list of sections
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
{
  "Sections": {
    "SectionLinkList": [
      {
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections",
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
## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "GetSections.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetSections.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetSections.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetSections.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetSections.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetSections.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetSections.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetSections.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetSections.go" >}}
{{< /tab >}}
{{< /tabs >}}
