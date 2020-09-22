---
title: "Get all Paragraphs from a Word Document"
type: docs
url: /get-all-paragraphs-from-a-word-document/
aliases: [/get-all-paragraphs-from-a-word-document/]
weight: 10
---

This REST API allows you to get all paragraphs that are contained in a document or in a section.

## Resource URI

```java

~/{file-name}/paragraphs

~/{file-name}/sections/{sectionIndex}/paragraphs

~/{file-name}/sections/{sectionIndex}/headersFooters/{headerFooterIndex}/paragraphs

```

*{file-name}* is the name of the Word document containing elements.
*{sectionIndex}* is the index of a section that contains paragraphs. If this syntax is used, only elements within the specified section are returned.
*{headerFooterIndex}* is the index of a section that contains headers and footers. If this syntax is used, only elements within specified header/footer are returned.

[Swagger UI](https://apireference.aspose.cloud/words/#/Paragraphs/GetParagraphs) lets you call this REST API directly from the browser.  

## cURL Example

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java



// Please get your App_Key and App_SID from https://dashboard.aspose.cloud/#/apps. Place your App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get a list of paragraphs that are contained in the document or in the section

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/paragraphs" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Paragraphs": {

    "ParagraphLinkList": [

      {

        "Text": "3 of ",

        "NodeId": "0.0.0",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/0/paragraphs/0",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "3 of ",

        "NodeId": "0.0.1",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/0/paragraphs/1",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "3 of ",

        "NodeId": "0.0.2",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/0/paragraphs/2",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "Page  of ",

        "NodeId": "0.1.0",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/1/paragraphs/0",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "3 of 3",

        "NodeId": "0.1.1",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/1/paragraphs/1",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "3 of 3",

        "NodeId": "0.1.2",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/1/paragraphs/2",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "3 of ",

        "NodeId": "0.1.3",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/1/paragraphs/3",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "",

        "NodeId": "0.2.0",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/2/paragraphs/0",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "",

        "NodeId": "0.2.1",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/2/paragraphs/1",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "",

        "NodeId": "0.3.0",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/3/paragraphs/0",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "",

        "NodeId": "0.3.1",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/3/paragraphs/1",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "3 of ",

        "NodeId": "0.4.0",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/4/paragraphs/0",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "3 of ",

        "NodeId": "0.4.1",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/4/paragraphs/1",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "3 of ",

        "NodeId": "0.4.2",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/headersfooters/4/paragraphs/2",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "Testing Page 1A new Comment1",

        "NodeId": "0.0",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/0",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      },

      {

        "Text": "A new Comment1",

        "NodeId": "2.0",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/comments/0/paragraphs/0",

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

        "Text": "This will be the text for AsposeTesting Page 2",

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

        "NodeId": "\* Connection #0 to host api.aspose.cloud left intact 0.7",

        "link": {

          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/paragraphs/7",

          "Rel": "self",

          "Type": null,

          "Title": null

        }

      }

    ],

    "link": {

      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/paragraphs",

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

Using an SDK is the best way to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetDocumentParagraphs.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentParagraphs.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_document_paragraphs.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_document_paragraphs.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getDocumentParagraphs.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentParagraphs.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentParagraphs.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "GetDocumentParagraphs.go" >}}

{{< /tab >}}

{{< /tabs >}}
