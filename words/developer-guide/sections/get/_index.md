---
title: "Get a Particular Section from a Word Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /sections/get/
aliases: [/get-a-particular-section-from-a-word-document/]
keywords: ""
description: "Get a section from a Word document"
weight: 20
---

This REST API retrieves a `Section`.

Important properties are the following:

|Property Name|Type|Description|
| :- | :- | :- |
|Paragraphs|Link|Represents a link to a list of all paragraphs that are contained in the section.|
|PageSetup|Link|Represents a link to the section's page setup resource.|

## Usage examples with cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetSectionOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetSectionOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "Section": {
    "Paragraphs": {
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "PageSetup": {
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/pagesetup",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "HeaderFooters": {
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters",
        "Rel": "self",
        "Type": null,
        "Title": null
      }
    },
    "Tables": {
      "link": {
        "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/tables",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "",
        "NodeId": "0.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "",
        "NodeId": "0.2",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/2",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "Heading",
        "NodeId": "0.3",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/3",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "",
        "NodeId": "0.4",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/4",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "Testing Page 2",
        "NodeId": "0.5",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/5",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "",
        "NodeId": "0.6",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/6",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "Testing Page 3",
        "NodeId": "0.7",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0",
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

## Aspose.Words Cloud SDK Family

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Usage examples in Python, Java, C#, etc.

The following code samples show how to interact with REST API using almost any mainstream programming language. You can find a lot of other code examples in [Python](https://gist.github.com/aspose-words-cloud-gists/e26813ced70692c544820cd8011ee7e0), [Java](https://gist.github.com/aspose-words-cloud-gists/caede439bfd2e57c3010befe504faff4), [C#](https://gist.github.com/aspose-words-cloud-gists/374e1e3dd4bca8f696f29d913645f549), [JavaScript](https://gist.github.com/aspose-words-cloud-gists/a9510e4b51613f1138e7c1ec09634c4a), [PHP](https://gist.github.com/aspose-words-cloud-gists/e2a72445b96362dc0117f06ab54bb94a), [C++](https://gist.github.com/aspose-words-cloud-gists/49aa5151a094849179bae8672c887a0e), [Golang](https://gist.github.com/aspose-words-cloud-gists/625ca80adffd779e8f6e3611551e14d5), [Ruby](https://gist.github.com/aspose-words-cloud-gists/339f3835a4c0a536c81ec941de29baf7), [Swift](https://gist.github.com/aspose-words-cloud-gists/790dbd2edd5d36f170732366f52cac4c), [Dart](https://gist.github.com/aspose-words-cloud-gists/6aae628cf2b878b78fea177c3171c6bf) on GitHub. All codes are thoroughly tested and ready for production use.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetSectionOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetSectionOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetSectionOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetSectionOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetSectionOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetSectionOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetSectionOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetSectionOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetSectionOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetSectionOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
