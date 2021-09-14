---
title: "Get Representation of a Form Field"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /formfields/get/
aliases: [/get-representation-of-a-form-field/]
description: "Get a form field from a paragraph in a Word document"
weight: 30
---

This REST API retrieves a form field from a paragraph.

## REST API

The following URI is used to address the REST resource:

```HTML
~/{paragraph}/formfields/{formFieldIndex}
```

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/FormFields/GetFormField) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [FormFilled.docx](/words/formfields/FormFilled.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get one of the form field
curl -v "https://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/formfields/0" \
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
  "FormField": {
    "NodeId": "0.1.0.0.0.1",
    "Name": "FullName",
    "Enabled": true,
    "StatusText": "",
    "OwnStatus": false,
    "HelpText": "",
    "OwnHelp": false,
    "CalculateOnExit": true,
    "EntryMacro": "",
    "ExitMacro": "",
    "TextInputFormat": "UPPERCASE",
    "TextInputType": "Regular",
    "TextInputDefault": "123",
    "MaxLength": 0,
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/tables/0/rows/0/cells/0/paragraphs/0/formfields/0",
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
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetFormField.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetFormField.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetFormField.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "GetFormField.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetFormField.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
