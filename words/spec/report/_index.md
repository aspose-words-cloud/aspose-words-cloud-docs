---
title: "Report"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/report/
description: "Report"
notoc: true
weight: 400
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
    <td style="vertical-align:middle;" class="bg-white"><span style="color:SteelBlue;">Stream</span></td>
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
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#executemailmergerequest">ExecuteMailMergeRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></td>
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


## ReportBuildOptions

This class is used in [ReportEngineSettings](#reportenginesettings).

The following values are defined: None, AllowMissingMembers, RemoveEmptyParagraphs, InlineErrorMessages.


## ReportEngineSettings

Represents a report engine settings.

This class is used in [BuildReportOnlineRequest](#buildreportonlinerequest), [BuildReportRequest](#buildreportrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| CsvDataLoadOptions   | [CsvDataLoadOptions](#csvdataloadoptions)     | Gets or sets the options for parsing CSV data. |
| DataSourceName       | <span style="color:SteelBlue;">string</span>  | Gets or sets the name to reference the data source object in the template. |
| DataSourceType       | [DataSourceTypeEnum](#reportenginesettings.datasourcetypeenum) | Gets or sets type of datasource. |
| ReportBuildOptions   | List&lt;[ReportBuildOptions](#reportbuildoptions)&gt; | Gets or sets type of options to build report. |


## BuildReportOnlineRequest

Represents a request model for [WordsApi.BuildReportOnline()](/words/report/build-online/) operation.

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

Represents a request model for [WordsApi.BuildReport()](/words/report/build-online/) operation.

An object of the **BuildReportRequest** class is created by the following constructor methods:

- BuildReportRequest()
- BuildReportRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***data***, [ReportEngineSettings](#reportenginesettings) ***reportEngineSettings***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***data***           | Data                 | <span style="color:SteelBlue;">string</span>  | A string providing a data to populate the specified template. The string must be of one of the following types: xml, json, csv. |
| ***reportEngineSettings*** | ReportEngineSettings | [ReportEngineSettings](#reportenginesettings) | An object providing a settings of report engine. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | The filename of the output document. If this parameter is omitted, the result will be saved with autogenerated name. |



## ExecuteMailMergeOnlineRequest

Represents a request model for [WordsApi.ExecuteMailMergeOnline()](/words/mail-merge/populate-with-data-online/) operation.

An object of the **ExecuteMailMergeOnlineRequest** class is created by the following constructor methods:

- ExecuteMailMergeOnlineRequest()
- ExecuteMailMergeOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***template***, <span style="color:SteelBlue;">Stream</span> ***data***, <span style="color:SteelBlue;">bool?</span> *withRegions*, <span style="color:SteelBlue;">string</span> *cleanup*, <span style="color:SteelBlue;">string</span> *documentFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***template***       | Template             | <span style="color:SteelBlue;">Stream</span>  | File with template. |
| ***data***           | Data                 | <span style="color:SteelBlue;">Stream</span>  | File with mailmerge data. |
| *withRegions*        | WithRegions          | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to execute Mail Merge operation with regions. |
| *cleanup*            | Cleanup              | <span style="color:SteelBlue;">string</span>  | The cleanup options. |
| *documentFileName*   | DocumentFileName     | <span style="color:SteelBlue;">string</span>  | The filename of the output document, that will be used when the resulting document has a dynamic field {filename}. If it is not set, the "template" will be used instead. |



## ExecuteMailMergeRequest

Represents a request model for [WordsApi.ExecuteMailMerge()](/words/mail-merge/populate-with-data-online/) operation.

An object of the **ExecuteMailMergeRequest** class is created by the following constructor methods:

- ExecuteMailMergeRequest()
- ExecuteMailMergeRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *data*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">bool?</span> *withRegions*, <span style="color:SteelBlue;">string</span> *mailMergeDataFile*, <span style="color:SteelBlue;">string</span> *cleanup*, <span style="color:SteelBlue;">bool?</span> *useWholeParagraphAsRegion*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *data*               | Data                 | <span style="color:SteelBlue;">string</span>  | Mail merge data. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *withRegions*        | WithRegions          | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to execute Mail Merge operation with regions. |
| *mailMergeDataFile*  | MailMergeDataFile    | <span style="color:SteelBlue;">string</span>  | The data file. |
| *cleanup*            | Cleanup              | <span style="color:SteelBlue;">string</span>  | The cleanup options. |
| *useWholeParagraphAsRegion* | UseWholeParagraphAsRegion | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether paragraph with TableStart or TableEnd field should be fully included into mail merge region or particular range between TableStart and TableEnd fields. The default value is true. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | The filename of the output document. If this parameter is omitted, the result will be saved with autogenerated name. |



## ReportEngineSettings.DataSourceTypeEnum

The following values are defined: Xml, Json, Csv.

