---
title: "Get All Document Properties"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /documents/properties/get-all/
aliases: [/get-all-document-properties/]
description: "Get all document properties from a Word document"
weight: 40
---

This REST API retrieves all built-in and custom properties of a document.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DocumentProperties/GetDocumentProperties) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get document properties
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties" \
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
  "DocumentProperties": {
    "List": [
      {
        "Name": "Bytes",
        "Value": "58687",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Bytes",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "Characters",
        "Value": "52",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Characters",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "CharactersWithSpaces",
        "Value": "60",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/CharactersWithSpaces",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "Company",
        "Value": "",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Company",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "CreateTime",
        "Value": "04/29/2015 05:01:00",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/CreateTime",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "HeadingPairs",
        "Value": "#ObjectArray",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/HeadingPairs",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "LastSavedBy",
        "Value": "Екимов Я.Н.",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/LastSavedBy",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "LastSavedTime",
        "Value": "10/21/2017 13:28:00",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/LastSavedTime",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "Lines",
        "Value": "1",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Lines",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "NameOfApplication",
        "Value": "Microsoft Office Word",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/NameOfApplication",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "Pages",
        "Value": "3",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Pages",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "Paragraphs",
        "Value": "1",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Paragraphs",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "RevisionNumber",
        "Value": "13",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/RevisionNumber",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "Security",
        "Value": "0",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Security",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "Template",
        "Value": "Normal.dotm",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Template",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "TitlesOfParts",
        "Value": "#StringArray",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/TitlesOfParts",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "TotalEditingTime",
        "Value": "11",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/TotalEditingTime",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "Version",
        "Value": "1048576",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Version",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "Words",
        "Value": "9",
        "BuiltIn": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Words",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Name": "testProp",
        "Value": "1",
        "BuiltIn": false,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/testProp",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties",
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
{{< tabs tabTotal="9" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetDocumentProperties.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetDocumentProperties.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetDocumentProperties.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetDocumentProperties.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetDocumentProperties.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetDocumentProperties.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetDocumentProperties.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetDocumentProperties.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetDocumentProperties.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
