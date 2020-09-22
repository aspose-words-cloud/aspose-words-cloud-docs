---
title: "Get a Particular Section from a Word Document"
type: docs
url: /get-a-particular-section-from-a-word-document/
aliases: [/get-a-particular-section-from-a-word-document/]
keywords: "List of Sections,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents,Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "This REST API allows you to get a specific section or section break that are contained in the document. Please note that The SDKs of this cloud API are available in Python, C#, Java, Ruby, PHP, Node.js, Android, Swift and Go languages."
weight: 20
---

This REST API allows you to get one of the sections contained in the document. The resource properties are the following:

|Property Name|Type|Description|
| :- | :- | :- |
|Paragraphs|Link|Represents a link to a list of all paragraphs that are contained in the section.|
|PageSetup|Link|Represents a link to the section's page setup resource.|
**Note**: The SDKs of this cloud API are available in *Python, C#, Java, Ruby, PHP, Node.js, Android, Swift* and *Go* languages.

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Sections/GetSection) lets you call this REST API directly from the browser.  

## cURL Example

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

// cURL example to get a particular section from a Word Document

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
{
  "Section": {
    "Paragraphs": {
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs",
        "Rel": "self",
        "Type": null,
        "Title": null

      }
    },
    "PageSetup": {
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/pagesetup",
        "Rel": "self",
        "Type": null,
        "Title": null

      }
    },
    "HeaderFooters": {
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters",
        "Rel": "self",
        "Type": null,
        "Title": null

      }
    },
    "Tables": {
      "link": {
        "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/tables",
        "Rel": "self",
        "Type": null,
        "Title": null

      }
    },
    "ChildNodes": [
      {
        "Text": "Testing Comment 1Page 1",
        "NodeId": "0.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      },
      {
        "Text": "",
        "NodeId": "0.1",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/1",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      },
      {
        "Text": "",
        "NodeId": "0.2",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/2",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      },
      {
        "Text": "Heading",
        "NodeId": "0.3",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/3",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      },
      {
        "Text": "",
        "NodeId": "0.4",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/4",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      },
      {
        "Text": "Testing Page 2",
        "NodeId": "0.5",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/5",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      },
      {
        "Text": "",
        "NodeId": "0.6",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/6",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      },
      {
        "Text": "Testing Page 3",
        "NodeId": "0.7",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0",
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
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "GetSection.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetSection.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetSection.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetSection.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetSection.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetSection.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetSection.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetSection.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetSection.go" >}}
{{< /tab >}}
{{< /tabs >}}
