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

## REST API calls using cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetDocumentPropertiesOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetDocumentPropertiesOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
 {
  "DocumentProperties": {
    "List": [
      {
        "Name": "Bytes",
        "Value": "58687",
        "BuiltIn": true,
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Bytes",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Characters",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/CharactersWithSpaces",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Company",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/CreateTime",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/HeadingPairs",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/LastSavedBy",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/LastSavedTime",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Lines",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/NameOfApplication",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Pages",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Paragraphs",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/RevisionNumber",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Security",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Template",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/TitlesOfParts",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/TotalEditingTime",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Version",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/Words",
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
          "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties/testProp",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties",
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

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Code samples in Python, Java, C#, etc.

The following code samples show how to interact with REST API using almost any mainstream programming language (Python, Java, C#, JavaScript, PHP, C++, Golang, Ruby, Swift, Dart):

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetDocumentPropertiesOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetDocumentPropertiesOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetDocumentPropertiesOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetDocumentPropertiesOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetDocumentPropertiesOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetDocumentPropertiesOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetDocumentPropertiesOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetDocumentPropertiesOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetDocumentPropertiesOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetDocumentPropertiesOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
