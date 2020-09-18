---
title: "Update Properties of a Form Field"
type: docs
url: /update-properties-of-a-form-field/
aliases: [/update-properties-of-a-form-field/]
weight: 40
---

This REST API allows you to update properties of a form field, returns updated form field data in XML/JSON format. The resource properties are:

|**Property Name**|**Type**|**Description**|
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

|**Property Name**|**Type**|**Description**|
| :- | :- | :- |
|TextInputFormat|string|Specifies the text formatting for a text form field.|
|TextInputType|TextFormFieldType|Specifies the type of a text form field.|
|TextInputDefault|string|Specifies the default string or a calculation expression of a text form field.|
|MaxLength|int|The maximum length for the text field. Zero when the length is not limited.|
**Checkbox properties**

|**Property Name**|**Type**|**Description**|
| :- | :- | :- |
|IsCheckBoxExactSize|bool|Specifies the boolean value that indicates whether the size of the textbox is automatic or specified explicitly.|
|CheckBoxSize|double|Specifies the size of the checkbox in points. Has effect only when "IsCheckBoxExactSize" is true.|
|Checked|bool|Specifies the checked status of the checkbox form field.|
**DropDown properties**

|**Property Name**|**Type**|**Description**|
| :- | :- | :- |
|DropDownSelectedIndex|int|Specifies the index specifying the currently selected item in a dropdown form field.|
|DropDownItems|string[]|Provides access to the items of a dropdown form field.|
The **Request Parameters** are:

|**Parameter Name**|**Type**|**Query String/HTTPBody**|**Description**|
| :- | :- | :- | :- |
|insertBeforeNode|string|Query String: insertBeforeNode="nodeId"|Form field will be inserted before node with id="nodeId".|
## Resource URI
```html

~/{paragraph}/formfields/{formFieldIndex}

```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to a specific node in the document. If this URI is used, only elements contained within a specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

[Swagger UI](https://apireference.aspose.cloud/words/#/FormFields/UpdateFormField) lets you call this REST API directly from the browser.  
## cURL Example
**Input Document:** [FormFilled.docx](attachments/885421/1180128.docx)

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to update form fields properties

curl -v "https://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/formfields/0" \
-X PUT \
-d "{'Name': 'FullName', 'Enabled': true, 'StatusText': '', 'CalculateOnExit': true, 'TextInputType': 'Regular', 'TextInputDefault': '' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

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

    "TextInputDefault": "",

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
## SDKs
Using an SDK is the best way to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## SDK Examples
{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "UpdatePropertiesOfFormField.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostFormField.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "post_form_field.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "post_form_field.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postFormField.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostFormField.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostFormField.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "PostFormField.go" >}}

{{< /tab >}}

{{< /tabs >}}
