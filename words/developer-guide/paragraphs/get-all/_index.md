---
title: "Get all"
second_title: "Paragraphs in a Document"
type: docs
url: /paragraphs/get-all/
aliases: [/get-all-paragraphs-from-a-word-document/]
description: "Get all paragraphs in a Word document"
weight: 40
---

This REST API retrieves a collection `Paragraph` items from a document.

## REST API

```JAVA
~/{file-name}/paragraphs

~/{file-name}/sections/{sectionIndex}/paragraphs

~/{file-name}/sections/{sectionIndex}/headersFooters/{headerFooterIndex}/paragraphs
```
, where:

- *{file-name}* is a filename of a document.
- *{sectionIndex}* is an index of a section. If this syntax is used, only elements within the specified section are returned.
- *{headerFooterIndex}* is an index of a section, that contains headers and footers. If this syntax is used, only elements within specified header/footer are returned.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Paragraphs/GetParagraphs) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of paragraphs that are contained in a document or in a section
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/paragraphs" \
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
  "Paragraphs": {
    "ParagraphLinkList": [
      {
        "Text": "3 of ",
        "NodeId": "0.0.0",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/0/paragraphs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "3 of ",
        "NodeId": "0.0.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/0/paragraphs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "3 of ",
        "NodeId": "0.0.2",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/0/paragraphs/2",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "Page  of ",
        "NodeId": "0.1.0",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/1/paragraphs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "3 of 3",
        "NodeId": "0.1.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/1/paragraphs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "3 of 3",
        "NodeId": "0.1.2",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/1/paragraphs/2",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "3 of ",
        "NodeId": "0.1.3",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/1/paragraphs/3",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "",
        "NodeId": "0.2.0",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/2/paragraphs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "",
        "NodeId": "0.2.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/2/paragraphs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "",
        "NodeId": "0.3.0",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/3/paragraphs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "",
        "NodeId": "0.3.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/3/paragraphs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "3 of ",
        "NodeId": "0.4.0",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/4/paragraphs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "3 of ",
        "NodeId": "0.4.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/4/paragraphs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "3 of ",
        "NodeId": "0.4.2",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/4/paragraphs/2",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "Testing Page 1A new Comment1",
        "NodeId": "0.0",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Text": "A new Comment1",
        "NodeId": "2.0",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0/paragraphs/0",
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
        "Text": "This will be the text for AsposeTesting Page 2",
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
      "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/paragraphs",
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
{{< tabs tabTotal="10" tabID="5" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetParagraphsOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetParagraphsOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetParagraphsOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetParagraphsOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetParagraphsOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetParagraphsOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetParagraphsOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetParagraphsOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetParagraphsOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetParagraphsOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
