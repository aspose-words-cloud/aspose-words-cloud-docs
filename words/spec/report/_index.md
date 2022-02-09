---
title: "Report"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/report/
description: "Report"
notoc: true
weight: 410
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Build</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#buildreportonlinerequest">BuildReportOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><span style="color:SteelBlue;">System.IO.Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#reportenginesettings">ReportEngineSettings</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#buildreportrequest">BuildReportRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></br><a href="#reportenginesettings">ReportEngineSettings</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Execute</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#executemailmergeonlinerequest">ExecuteMailMergeOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><span style="color:SteelBlue;">System.IO.Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#fieldoptions">FieldOptions</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#executemailmergerequest">ExecuteMailMergeRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></br><a href="#fieldoptions">FieldOptions</a></td>
  </tr>
  </tbody>
</table>


## CsvDataLoadOptions

Represents a options for parsing CSV data.

This class is used in [ReportEngineSettings](#reportenginesettings).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| CommentChar          | <span style="color:SteelBlue;">string</span>  | Gets or sets the character that is used to comment lines of CSV data. |
| Delimiter            | <span style="color:SteelBlue;">string</span>  | Gets or sets the character to be used as a column delimiter. |
| HasHeaders           | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the first record of CSV data contains column names. |
| QuoteChar            | <span style="color:SteelBlue;">string</span>  | Gets or sets the character that is used to quote field values. |


## FieldOptions

Represents a dTO for field options.

This class is used in [ExecuteMailMergeOnlineRequest](#executemailmergeonlinerequest), [ExecuteMailMergeRequest](#executemailmergerequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| BuiltInTemplatesPaths | List&lt;<span style="color:SteelBlue;">string</span>&gt; | Gets or sets BuiltIn Templates Paths. |
| CurrentUser          | [UserInformation](#userinformation)           | Gets or sets Curren tUser. |
| CustomTocStyleSeparator | <span style="color:SteelBlue;">string</span>  | Gets or sets Custom Toc Style Separator. |
| DefaultDocumentAuthor | <span style="color:SteelBlue;">string</span>  | Gets or sets Default Document Author. |
| FieldIndexFormat     | [FieldIndexFormatEnum](/words/spec/field#fieldoptions.fieldindexformatenum) | Gets or sets Field Index Format. |
| FieldUpdateCultureName | <span style="color:SteelBlue;">string</span>  | Gets or sets Field Update Culture Name. It is used for all fields if FieldUpdateCultureSource is FieldCode. |
| FieldUpdateCultureSource | [FieldUpdateCultureSourceEnum](/words/spec/field#fieldoptions.fieldupdateculturesourceenum) | Gets or sets Field Update Culture Source. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets File Name. |
| IsBidiTextSupportedOnUpdate | <span style="color:SteelBlue;">bool</span>    | Gets or sets if Bidi Text Supported OnUpdate. |
| LegacyNumberFormat   | <span style="color:SteelBlue;">bool</span>    | Gets or sets if Legacy Number Format. |
| PreProcessCultureName | <span style="color:SteelBlue;">string</span>  | Gets or sets PreProcess Culture Name. It is a culture code for DOC fields. |
| TemplateName         | <span style="color:SteelBlue;">string</span>  | Gets or sets Template Name. |
| UseInvariantCultureNumberFormat | <span style="color:SteelBlue;">bool</span>    | Gets or sets if Use Invariant Culture Number Format. |


## JsonDataLoadOptions

Represents a options for parsing JSON data.

This class is used in [ReportEngineSettings](#reportenginesettings).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AlwaysGenerateRootObject | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether a generated data source will always contain an object for a JSON root element. If a JSON root element contains a single complex property, such an object is not created by default. |
| ExactDateTimeParseFormats | List&lt;<span style="color:SteelBlue;">string</span>&gt; | Gets or sets exact formats for parsing JSON date-time values while loading JSON. The default is null. |
| SimpleValueParseMode | [SimpleValueParseModeEnum](#jsondataloadoptions.simplevalueparsemodeenum) | Gets or sets a mode for parsing JSON simple values (null, boolean, number, integer, and string) while loading JSON. Such a mode does not affect parsing of date-time values. The default is Aspose.Words.Reporting.JsonSimpleValueParseMode.Loose. |


## ReportBuildOptions

This class is used in [ReportEngineSettings](#reportenginesettings).

The following values are defined: None, AllowMissingMembers, RemoveEmptyParagraphs, InlineErrorMessages, UseLegacyHeaderFooterVisiting.


## ReportEngineSettings

Represents a report engine settings.

This class is used in [BuildReportOnlineRequest](#buildreportonlinerequest), [BuildReportRequest](#buildreportrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| CsvDataLoadOptions   | [CsvDataLoadOptions](#csvdataloadoptions)     | Gets or sets the options for parsing CSV data. |
| DataSourceName       | <span style="color:SteelBlue;">string</span>  | Gets or sets the name to reference the data source object in the template. |
| DataSourceType       | [DataSourceTypeEnum](#reportenginesettings.datasourcetypeenum) | Gets or sets type of datasource. |
| JsonDataLoadOptions  | [JsonDataLoadOptions](#jsondataloadoptions)   | Gets or sets the options for parsing JSON data. |
| ReportBuildOptions   | List&lt;[ReportBuildOptions](#reportbuildoptions)&gt; | Gets or sets type of options to build report. |
| XmlDataLoadOptions   | [XmlDataLoadOptions](#xmldataloadoptions)     | Gets or sets the options for parsing XML data. |


## UserInformation

Represents a dTO for user information.

This class is used in [FieldOptions](#fieldoptions).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Address              | <span style="color:SteelBlue;">string</span>  | Gets or sets user address. |
| Initials             | <span style="color:SteelBlue;">string</span>  | Gets or sets user initials. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets user name. |


## XmlDataLoadOptions

Represents a options for XML data loading.

This class is used in [ReportEngineSettings](#reportenginesettings).

A single `AlwaysGenerateRootObject` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AlwaysGenerateRootObject | <span style="color:SteelBlue;">bool</span>    | Gets or sets a flag indicating whether a generated data source will always contain an object for an XML root element. If an XML root element has no attributes and all its child elements have same names, such an object is not created by default. |


## BuildReportOnlineRequest

Represents a request model for [WordsApi.BuildReportOnline()](/words/report/build/) operation.

An object of the **BuildReportOnlineRequest** class is created by the following constructor methods:

- BuildReportOnlineRequest()
- BuildReportOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***template***, <span style="color:SteelBlue;">string</span> ***data***, [ReportEngineSettings](#reportenginesettings) ***reportEngineSettings***, <span style="color:SteelBlue;">string</span> *documentFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***template***       | Template             | <span style="color:SteelBlue;">Stream</span>  | File with template. |
| ***data***           | Data                 | <span style="color:SteelBlue;">string</span>  | A string providing a data to populate the specified template. The string must be of one of the following types: xml, json, csv. |
| ***reportEngineSettings*** | ReportEngineSettings | [ReportEngineSettings](#reportenginesettings) | An object providing a settings of report engine. |
| *documentFileName*   | DocumentFileName     | <span style="color:SteelBlue;">string</span>  | The filename of the output document, that will be used when the resulting document has a dynamic field {filename}. If it is not set, the "template" will be used instead. |



## BuildReportRequest

Represents a request model for [WordsApi.BuildReport()](/words/report/build/) operation.

An object of the **BuildReportRequest** class is created by the following constructor methods:

- BuildReportRequest()
- BuildReportRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***data***, [ReportEngineSettings](#reportenginesettings) ***reportEngineSettings***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***data***           | Data                 | <span style="color:SteelBlue;">string</span>  | A string providing a data to populate the specified template. The string must be of one of the following types: xml, json, csv. |
| ***reportEngineSettings*** | ReportEngineSettings | [ReportEngineSettings](#reportenginesettings) | An object providing a settings of report engine. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | The filename of the output document. If this parameter is omitted, the result will be saved with autogenerated name. |



## ExecuteMailMergeOnlineRequest

Represents a request model for [WordsApi.ExecuteMailMergeOnline()](/words/mail-merge/populate-with-data/) operation.

An object of the **ExecuteMailMergeOnlineRequest** class is created by the following constructor methods:

- ExecuteMailMergeOnlineRequest()
- ExecuteMailMergeOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***template***, <span style="color:SteelBlue;">Stream</span> ***data***, [FieldOptions](#fieldoptions) *options*, <span style="color:SteelBlue;">bool?</span> *withRegions*, <span style="color:SteelBlue;">string</span> *cleanup*, <span style="color:SteelBlue;">string</span> *documentFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***template***       | Template             | <span style="color:SteelBlue;">Stream</span>  | File with template. |
| ***data***           | Data                 | <span style="color:SteelBlue;">Stream</span>  | File with mailmerge data. |
| *options*            | Options              | [FieldOptions](#fieldoptions)                 | Field options. |
| *withRegions*        | WithRegions          | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to execute Mail Merge operation with regions. |
| *cleanup*            | Cleanup              | <span style="color:SteelBlue;">string</span>  | The cleanup options. |
| *documentFileName*   | DocumentFileName     | <span style="color:SteelBlue;">string</span>  | The filename of the output document, that will be used when the resulting document has a dynamic field {filename}. If it is not set, the "template" will be used instead. |



## ExecuteMailMergeRequest

Represents a request model for [WordsApi.ExecuteMailMerge()](/words/mail-merge/populate-with-data/) operation.

An object of the **ExecuteMailMergeRequest** class is created by the following constructor methods:

- ExecuteMailMergeRequest()
- ExecuteMailMergeRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *data*, [FieldOptions](#fieldoptions) *options*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">bool?</span> *withRegions*, <span style="color:SteelBlue;">string</span> *mailMergeDataFile*, <span style="color:SteelBlue;">string</span> *cleanup*, <span style="color:SteelBlue;">bool?</span> *useWholeParagraphAsRegion*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *data*               | Data                 | <span style="color:SteelBlue;">string</span>  | Mail merge data. |
| *options*            | Options              | [FieldOptions](#fieldoptions)                 | Field options. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *withRegions*        | WithRegions          | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to execute Mail Merge operation with regions. |
| *mailMergeDataFile*  | MailMergeDataFile    | <span style="color:SteelBlue;">string</span>  | The data file. |
| *cleanup*            | Cleanup              | <span style="color:SteelBlue;">string</span>  | The cleanup options. |
| *useWholeParagraphAsRegion* | UseWholeParagraphAsRegion | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether paragraph with TableStart or TableEnd field should be fully included into mail merge region or particular range between TableStart and TableEnd fields. The default value is true. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | The filename of the output document. If this parameter is omitted, the result will be saved with autogenerated name. |



## JsonDataLoadOptions.SimpleValueParseModeEnum

The following values are defined: Loose, Strict.


## ReportEngineSettings.DataSourceTypeEnum

The following values are defined: Xml, Json, Csv.

