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

## REST API calls using cURL and Postman

The following URI is used to address the REST resource:

```HTML
~/{paragraph}/formfields/{formFieldIndex}
```

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

Download sample [FormFilled.docx](/words/formfields/FormFilled.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="2" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "InsertFormFieldOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "InsertFormFieldOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
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
      "Href": "https://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/tables/0/rows/0/cells/0/paragraphs/0/formfields/0",
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

## Code samples in Python, Java, C#, etc.

The following code samples show how to interact with REST API using almost any mainstream programming language (Python, Java, C#, JavaScript, PHP, C++, Golang, Ruby, Swift, Dart):

{{< nosnippet >}}
{{< tabs tabTotal="11" tabID="5" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" tabName11="Curl" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "InsertFormFieldOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "InsertFormFieldOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "InsertFormFieldOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "InsertFormFieldOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "InsertFormFieldOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "InsertFormFieldOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "InsertFormFieldOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "InsertFormFieldOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "InsertFormFieldOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "InsertFormFieldOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
