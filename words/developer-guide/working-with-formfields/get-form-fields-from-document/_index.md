---
title: "Get Form Fields from Document"
type: docs
url: /get-form-fields-from-document/
aliases: [/get-form-fields-from-document/]
weight: 10
---

This REST API allows you to get form fields from a document or specific section/paragraph.

## Resource URI

```html

~/{file-name}/formfields

~/{file-name}/{nodePath}/formfields
```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to a specific node in the document. If this URI is used, only elements contained within a specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/FormFields/GetFormFields) lets you call this REST API directly from a browser.

## cURL Example

cUrl is a popular command-line utility for transferring data and a perfect tool for testing REST APIs. The following are a few examples of using cURL.

*Input Document:** [FormFilled.docx](attachments/885421/1180128.docx)

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get form fields from document
curl -v "https://api.aspose.cloud/v4.0/words/FormFilled.docx/formfields" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
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
## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetFormFields.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetFormFields.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_form_fields.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_form_fields.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getFormFields.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetFormFields.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetFormFields.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetFormFields.go" >}}
{{< /tab >}}
{{< /tabs >}}
