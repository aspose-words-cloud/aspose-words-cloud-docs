---
title: "FormField"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/formfield/
description: "FormField"
notoc: true
weight: 270
---


<table>
  <thead>
    <tr>
      <th style="text-align:center;"></th>
      <th><i>Request</i></th>
      <th><i>Response</i></th>
      <th><i>Model</i></th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Delete</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteformfieldonlinerequest">DeleteFormFieldOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deleteformfieldrequest">DeleteFormFieldRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getformfieldonlinerequest">GetFormFieldOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#formfieldresponse">FormFieldResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#formfield">FormField</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getformfieldrequest">GetFormFieldRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getformfieldsonlinerequest">GetFormFieldsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#formfieldsresponse">FormFieldsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#formfieldcollection">FormFieldCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getformfieldsrequest">GetFormFieldsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertformfieldonlinerequest">InsertFormFieldOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertformfieldonlineresponse">InsertFormFieldOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><a href="#formfield">FormField</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertformfieldrequest">InsertFormFieldRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#formfieldresponse">FormFieldResponse</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updateformfieldonlinerequest">UpdateFormFieldOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updateformfieldonlineresponse">UpdateFormFieldOnlineResponse</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updateformfieldrequest">UpdateFormFieldRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#formfieldresponse">FormFieldResponse</a></td>
  </tr>
  </tbody>
</table>


## FormField

Represents a fromField.

This class is inherited from [NodeLink](/words/spec/link#nodelink) and used in [FormFieldCollection](#formfieldcollection), [FormFieldResponse](#formfieldresponse), [InsertFormFieldOnlineRequest](#insertformfieldonlinerequest), [InsertFormFieldRequest](#insertformfieldrequest), [UpdateFormFieldOnlineRequest](#updateformfieldonlinerequest), [UpdateFormFieldRequest](#updateformfieldrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| CalculateOnExit      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited. |
| Enabled              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether a form field is enabled. |
| EntryMacro           | <span style="color:SteelBlue;">string</span>  | Gets or sets the entry macro name for the form field. |
| ExitMacro            | <span style="color:SteelBlue;">string</span>  | Gets or sets the exit macro name for the form field. |
| HelpText             | <span style="color:SteelBlue;">string</span>  | Gets or sets text, displayed in a message box when the form field has the focus and the user presses F1. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the form field name. |
| OwnHelp              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the source of the text that's displayed in a message box when a form field has the focus and the user presses F1. |
| OwnStatus            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus. |
| StatusText           | <span style="color:SteelBlue;">string</span>  | Gets or sets text, displayed in the status bar when a form field has the focus. |


## FormFieldCheckbox

Represents a formField checkbox element.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| CalculateOnExit      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited. |
| Enabled              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether a form field is enabled. |
| EntryMacro           | <span style="color:SteelBlue;">string</span>  | Gets or sets the entry macro name for the form field. |
| ExitMacro            | <span style="color:SteelBlue;">string</span>  | Gets or sets the exit macro name for the form field. |
| HelpText             | <span style="color:SteelBlue;">string</span>  | Gets or sets text, displayed in a message box when the form field has the focus and the user presses F1. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the form field name. |
| OwnHelp              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the source of the text that's displayed in a message box when a form field has the focus and the user presses F1. |
| OwnStatus            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus. |
| StatusText           | <span style="color:SteelBlue;">string</span>  | Gets or sets text, displayed in the status bar when a form field has the focus. |
| CheckBoxSize         | <span style="color:SteelBlue;">double</span>  | Gets or sets the size of the checkbox in points. Has effect only when IsCheckBoxExactSize is true. |
| Checked              | <span style="color:SteelBlue;">bool</span>    | Gets or sets the checked status of the check box form field. |
| IsCheckBoxExactSize  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the size of the textbox is automatic or specified explicitly. |


## FormFieldCollection

Represents a dTO container with a collection of form fields.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [FormFieldsResponse](#formfieldsresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| List                 | List&lt;[FormField](#formfield)&gt;           | Gets or sets the collection of form fields. |


## FormFieldDropDown

Represents a formField dropdownlist element.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| CalculateOnExit      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited. |
| Enabled              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether a form field is enabled. |
| EntryMacro           | <span style="color:SteelBlue;">string</span>  | Gets or sets the entry macro name for the form field. |
| ExitMacro            | <span style="color:SteelBlue;">string</span>  | Gets or sets the exit macro name for the form field. |
| HelpText             | <span style="color:SteelBlue;">string</span>  | Gets or sets text, displayed in a message box when the form field has the focus and the user presses F1. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the form field name. |
| OwnHelp              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the source of the text that's displayed in a message box when a form field has the focus and the user presses F1. |
| OwnStatus            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus. |
| StatusText           | <span style="color:SteelBlue;">string</span>  | Gets or sets text, displayed in the status bar when a form field has the focus. |
| DropDownItems        | List&lt;<span style="color:SteelBlue;">string</span>&gt; | Gets or sets the items array of a dropdown form field. |
| DropDownSelectedIndex | <span style="color:SteelBlue;">int</span>     | Gets or sets the index specifying the currently selected item in a dropdown form field. |


## FormFieldTextInput

Represents a formField text input element.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| CalculateOnExit      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited. |
| Enabled              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether a form field is enabled. |
| EntryMacro           | <span style="color:SteelBlue;">string</span>  | Gets or sets the entry macro name for the form field. |
| ExitMacro            | <span style="color:SteelBlue;">string</span>  | Gets or sets the exit macro name for the form field. |
| HelpText             | <span style="color:SteelBlue;">string</span>  | Gets or sets text, displayed in a message box when the form field has the focus and the user presses F1. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the form field name. |
| OwnHelp              | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the source of the text that's displayed in a message box when a form field has the focus and the user presses F1. |
| OwnStatus            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus. |
| StatusText           | <span style="color:SteelBlue;">string</span>  | Gets or sets text, displayed in the status bar when a form field has the focus. |
| MaxLength            | <span style="color:SteelBlue;">int</span>     | Gets or sets the maximum length for the text field. Zero when the length is not limited. |
| TextInputDefault     | <span style="color:SteelBlue;">string</span>  | Gets or sets the default string or a calculation expression of the text form field. |
| TextInputFormat      | <span style="color:SteelBlue;">string</span>  | Gets or sets text formatting for the text form field. |
| TextInputType        | [TextInputTypeEnum](#formfieldtextinput.textinputtypeenum) | Gets or sets the type of the text form field. |


## DeleteFormFieldOnlineRequest

Represents a request model for [WordsApi.DeleteFormFieldOnline()](/words/formfields/remove/) operation.

An object of the **DeleteFormFieldOnlineRequest** class is created by the following constructor methods:

- DeleteFormFieldOnlineRequest()
- DeleteFormFieldOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteFormFieldRequest

Represents a request model for [WordsApi.DeleteFormField()](/words/formfields/remove/) operation.

An object of the **DeleteFormFieldRequest** class is created by the following constructor methods:

- DeleteFormFieldRequest()
- DeleteFormFieldRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## FormFieldResponse

Represents a REST response with a form field.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertFormFieldOnlineResponse](#insertformfieldonlineresponse), [UpdateFormFieldOnlineResponse](#updateformfieldonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| FormField            | [FormField](#formfield)                       | Gets or sets the form field. |


## FormFieldsResponse

Represents a REST response with a collection of form fields.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| FormFields           | [FormFieldCollection](#formfieldcollection)   | Gets or sets the collection of form fields. |


## GetFormFieldOnlineRequest

Represents a request model for [WordsApi.GetFormFieldOnline()](/words/formfields/get/) operation.

An object of the **GetFormFieldOnlineRequest** class is created by the following constructor methods:

- GetFormFieldOnlineRequest()
- GetFormFieldOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetFormFieldRequest

Represents a request model for [WordsApi.GetFormField()](/words/formfields/get/) operation.

An object of the **GetFormFieldRequest** class is created by the following constructor methods:

- GetFormFieldRequest()
- GetFormFieldRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetFormFieldsOnlineRequest

Represents a request model for [WordsApi.GetFormFieldsOnline()](/words/formfields/get-all/) operation.

An object of the **GetFormFieldsOnlineRequest** class is created by the following constructor methods:

- GetFormFieldsOnlineRequest()
- GetFormFieldsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetFormFieldsRequest

Represents a request model for [WordsApi.GetFormFields()](/words/formfields/get-all/) operation.

An object of the **GetFormFieldsRequest** class is created by the following constructor methods:

- GetFormFieldsRequest()
- GetFormFieldsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## InsertFormFieldOnlineRequest

Represents a request model for [WordsApi.InsertFormFieldOnline()](/words/formfields/add/) operation.

An object of the **InsertFormFieldOnlineRequest** class is created by the following constructor methods:

- InsertFormFieldOnlineRequest()
- InsertFormFieldOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [FormField](#formfield) ***formField***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">string</span> *insertBeforeNode*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***formField***      | FormField            | [FormField](#formfield)                       | From field data. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *insertBeforeNode*   | InsertBeforeNode     | <span style="color:SteelBlue;">string</span>  | The index of the node. A new form field will be inserted before the node with the specified node Id. |



## InsertFormFieldOnlineResponse

Represents a response model for [WordsApi.InsertFormFieldOnline()](/words/formfields/add/) operation.

An object of the **InsertFormFieldOnlineResponse** class is created by the following constructor methods:

- InsertFormFieldOnlineResponse([FormFieldResponse](#formfieldresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [FormFieldResponse](#formfieldresponse)       | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## InsertFormFieldRequest

Represents a request model for [WordsApi.InsertFormField()](/words/formfields/add/) operation.

An object of the **InsertFormFieldRequest** class is created by the following constructor methods:

- InsertFormFieldRequest()
- InsertFormFieldRequest(<span style="color:SteelBlue;">string</span> ***name***, [FormField](#formfield) ***formField***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*, <span style="color:SteelBlue;">string</span> *insertBeforeNode*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***formField***      | FormField            | [FormField](#formfield)                       | From field data. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |
| *insertBeforeNode*   | InsertBeforeNode     | <span style="color:SteelBlue;">string</span>  | The index of the node. A new form field will be inserted before the node with the specified node Id. |



## UpdateFormFieldOnlineRequest

Represents a request model for [WordsApi.UpdateFormFieldOnline()](/words/formfields/update/) operation.

An object of the **UpdateFormFieldOnlineRequest** class is created by the following constructor methods:

- UpdateFormFieldOnlineRequest()
- UpdateFormFieldOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [FormField](#formfield) ***formField***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***formField***      | FormField            | [FormField](#formfield)                       | From field data. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateFormFieldOnlineResponse

Represents a response model for [WordsApi.UpdateFormFieldOnline()](/words/formfields/update/) operation.

An object of the **UpdateFormFieldOnlineResponse** class is created by the following constructor methods:

- UpdateFormFieldOnlineResponse([FormFieldResponse](#formfieldresponse) ***model***, Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [FormFieldResponse](#formfieldresponse)       | The response model. |
| ***document***       | Document             | Dictionary&lt;<span style="color:SteelBlue;">string,Stream</span>&gt; | The document after modification. |



## UpdateFormFieldRequest

Represents a request model for [WordsApi.UpdateFormField()](/words/formfields/update/) operation.

An object of the **UpdateFormFieldRequest** class is created by the following constructor methods:

- UpdateFormFieldRequest()
- UpdateFormFieldRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, [FormField](#formfield) ***formField***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| ***formField***      | FormField            | [FormField](#formfield)                       | From field data. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## FormFieldTextInput.TextInputTypeEnum

The following values are defined: Regular, Number, Date, CurrentDate, CurrentTime, Calculated.

