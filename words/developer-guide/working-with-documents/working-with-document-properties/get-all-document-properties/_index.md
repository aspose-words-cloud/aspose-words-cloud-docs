---
title: "Get All Document Properties"
type: docs
url: /get-all-document-properties/
aliases: [/get-all-document-properties/]
weight: 10
---

This REST API allows you to get all properties of a document. The API returns a JSON/XML representation of the document properties (built-in and custom).

## Resource URI

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/DocumentProperties/GetDocumentProperties) lets you call this REST API directly from a browser. The description of the API and its parameters is also given there.

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

// cURL example to get document properties
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/documentProperties" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
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
      "Re\* Connection #0 to host api.aspose.cloud left intact l": "self",
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
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "GetDocumentProperties.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentProperties.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetDocumentProperties.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetDocumentProperties.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetDocumentProperties.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetDocumentProperties.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentProperties.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentProperties.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentProperties.go" >}}
{{< /tab >}}
{{< /tabs >}}
