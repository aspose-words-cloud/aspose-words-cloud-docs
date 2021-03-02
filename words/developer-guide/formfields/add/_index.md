---
title: "Add Form Field to Paragraph"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /formfields/add/
aliases: [/add-form-field-to-paragraph/]
description: "Add a form field to a paragraph in a Word document"
weight: 10
---

This REST API adds a form field to a paragraph.

The resource properties are:

|Property Name|Type|Description|
| :- | :- | :- |
|Name|string|Specifies the form field name.|
|Enabled|bool|True if a form field is enabled.|
|StatusText|string|Specifies the text that is displayed in the status bar when a form field has the focus.|
|OwnStatus|bool|Specifies the source of the text that is displayed in the status bar when a form field has the focus.|
|HelpText|string|Specifies the text that is displayed in a message box when the form field has the focus and the user presses F1.|
|OwnHelp|bool|Specifies the source of the text that is displayed in a message box when a form field has the focus and the user presses F1.|
|CalculateOnExit|bool|True if references to the specified form field are automatically updated whenever the field is exited.|
|EntryMacro|string|Specifies an entry macro name for the form field.|
|ExitMacro|string|Specifies an exit macro name for the form field.|

**Text input properties**

|Property Name|Type|Description|
| :- | :- | :- |
|TextInputFormat|string|Specifies the text formatting for a text form field.|
|TextInputType|TextFormFieldType|Specifies the type of a text form field.|
|TextInputDefault|string|Specifies the default string or a calculation expression of a text form field.|
|MaxLength|int|The maximum length for the text field. Zero when the length is not limited.|

**Checkbox properties**

|Property Name|Type|Description|
| :- | :- | :- |
|IsCheckBoxExactSize|bool|Specifies the boolean value that indicates whether the size of the textbox is automatic or specified explicitly.|
|CheckBoxSize|double|Specifies the size of the checkbox in points. Has effect only when "IsCheckBoxExactSize" is true.|
|Checked|bool|Specifies the checked status of the checkbox form field.|

**DropDown properties**

|Property Name|Type|Description|
| :- | :- | :- |
|DropDownSelectedIndex|int|Specifies the index specifying the currently selected item in a dropdown form field.|
|DropDownItems|string[]|Provides access to the items of a dropdown form field.|

The **Request Parameters** are:

|Parameter Name|Type|Query String/HTTPBody|Description|
| :- | :- | :- | :- |
|insertBeforeNode|string|Query String: insertBeforeNode="nodeId"|Form field will be inserted before node with id="nodeId".|

## REST API

The following URI is used to address the REST resource:

```HTML
~/{paragraph}/formfields/{formFieldIndex}
```

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/FormFields/InsertFormField) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [FormFilled.docx](/words/formfields/FormFilled.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to add form field to paragraph
curl -v "https://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/paragraphs/1/formfields" \
-X POST \
-d "{ 'Name': 'FullName', 'Enabled': true, 'CalculateOnExit': true, 'StatusText': '', 'TextInputType': 'Regular', 'TextInputDefault': '123', 'TextInputFormat': 'UPPERCASE' }" \
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
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "PutFormField.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "AddFormFieldToParagraph.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "PutFormField.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_PutFormField.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_PutFormField.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
