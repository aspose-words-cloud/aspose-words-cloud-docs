---
title: "Get Form Fields from Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /formfields/get-all/
aliases: [/get-form-fields-from-document/]
description: "Get all form fields from a Word document"
weight: 20
---

This REST API retrieves form fields from a document, a section or a paragraph.

## REST API

The following URIs are used to address REST resources:

```HTML
~/{file-name}/formfields
~/{file-name}/{nodePath}/formfields
```
, where:

- *{file-name}* is a filename of a document.
- *{nodePath}* is a path to a node in a document. If this parameter is used, elements contained within a specified node will be processed:
  - *sections/{sectionIndex}* - references a section.
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/FormFields/GetFormFields) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [FormFilled.docx](/words/formfields/FormFilled.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get form fields from document
curl -v "https://api.aspose.cloud/v4.0/words/FormFilled.docx/formfields" \
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
  "FormFields": {
    "List": [
      {
        "NodeId": "0.1.0.1.0.0",
        "Name": "FullName",
        "Enabled": true,
        "StatusText": "Enter your name and surname (trimmed to 50 characters).",
        "OwnStatus": true,
        "HelpText": "Enter your name and surname (trimmed to 50 characters).",
        "OwnHelp": true,
        "CalculateOnExit": false,
        "EntryMacro": "",
        "ExitMacro": "",
        "TextInputFormat": "TITLE CASE",
        "TextInputType": "Regular",
        "TextInputDefault": "",
        "MaxLength": 50,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/tables/0/rows/0/cells/1/paragraphs/0/formfields/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "NodeId": "0.1.1.1.0.0",
        "Name": "BirthDate",
        "Enabled": true,
        "StatusText": "Enter your date of birth.",
        "OwnStatus": true,
        "HelpText": "Enter your date of birth.",
        "OwnHelp": true,
        "CalculateOnExit": false,
        "EntryMacro": "",
        "ExitMacro": "",
        "TextInputFormat": "yyyy-MM-dd",
        "TextInputType": "Date",
        "TextInputDefault": "",
        "MaxLength": 0,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/tables/0/rows/1/cells/1/paragraphs/0/formfields/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "NodeId": "0.1.2.1.0.1",
        "Name": "Salary",
        "Enabled": true,
        "StatusText": "Enter your monthly salary in USD.",
        "OwnStatus": true,
        "HelpText": "Enter your monthly salary in USD.",
        "OwnHelp": true,
        "CalculateOnExit": false,
        "EntryMacro": "",
        "ExitMacro": "",
        "TextInputFormat": "#,##0.00",
        "TextInputType": "Number",
        "TextInputDefault": "",
        "MaxLength": 0,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/tables/0/rows/2/cells/1/paragraphs/0/formfields/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "NodeId": "0.1.3.1.0.0",
        "Name": "Married",
        "Enabled": true,
        "StatusText": "Mark as checked if you are married.",
        "OwnStatus": true,
        "HelpText": "Mark as checked if you are married.",
        "OwnHelp": true,
        "CalculateOnExit": false,
        "EntryMacro": "",
        "ExitMacro": "",
        "IsCheckBoxExactSize": false,
        "CheckBoxSize": 10.0,
        "Checked": true,
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/tables/0/rows/3/cells/1/paragraphs/0/formfields/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "NodeId": "0.1.4.1.0.0",
        "Name": "Gender",
        "Enabled": true,
        "StatusText": "Select your gender.",
        "OwnStatus": true,
        "HelpText": "Select your gender.",
        "OwnHelp": true,
        "CalculateOnExit": false,
        "EntryMacro": "",
        "ExitMacro": "",
        "DropDownSelectedIndex": 1,
        "DropDownItems": [
          "<Select gender>",
          "Male",
          "Female"

        ],
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/tables/0/rows/4/cells/1/paragraphs/0/formfields/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/FormFilled.docx/formfields",
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
{{< tabs tabTotal="5" tabID="5" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetFormFields.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetFormFields.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetFormFields.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "GetFormFields.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetFormFields.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
