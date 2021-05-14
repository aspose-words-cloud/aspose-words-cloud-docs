---
title: "DocumentStatistics"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/documentstatistics/
description: "DocumentStatistics"
notoc: true
weight: 200
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentstatisticsonlinerequest">GetDocumentStatisticsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#statdataresponse">StatDataResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#documentstatdata">DocumentStatData</a></br><a href="/words/spec/link#filelink">FileLink</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentstatisticsrequest">GetDocumentStatisticsRequest</a></td>
  </tr>
  </tbody>
</table>


## DocumentStatData

Represents a container for the document's statistical data.

This class is used in [StatDataResponse](#statdataresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FootnotesStatData    | [FootnotesStatData](#footnotesstatdata)       | Gets or sets the detailed statistics on footnotes. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the total count of pages in the document. |
| PageStatData         | List&lt;[PageStatData](#pagestatdata)&gt;     | Gets or sets the detailed statistics on all pages. |
| ParagraphCount       | <span style="color:SteelBlue;">int</span>     | Gets or sets the total count of paragraphs in the document. |
| WordCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the total count of words in the document. |


## FootnotesStatData

Represents a container for the footnotes statistical data.

This class is used in [DocumentStatData](#documentstatdata), [PageStatData](#pagestatdata).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ParagraphCount       | <span style="color:SteelBlue;">int</span>     | Gets or sets the total count of paragraphs in footnotes. |
| WordCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the total count of words in footnotes. |


## PageStatData

Represents a container for the page's statistical data.

This class is used in [DocumentStatData](#documentstatdata).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| FootnotesStatData    | [FootnotesStatData](#footnotesstatdata)       | Gets or sets the detailed statistics on the footnotes. |
| PageNumber           | <span style="color:SteelBlue;">int</span>     | Gets or sets the page number. |
| ParagraphCount       | <span style="color:SteelBlue;">int</span>     | Gets or sets the total count of paragraphs in the page. |
| WordCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the total count of words in the page. |


## StatDataResponse

Represents a REST response with document's statistical data.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| DocumentLink         | [FileLink](/words/spec/link#filelink)         | Gets or sets the link to the document. |
| StatData             | [DocumentStatData](#documentstatdata)         | Gets or sets the statistical data of the document. |


## GetDocumentStatisticsOnlineRequest

Represents a request model for [WordsApi.GetDocumentStatisticsOnline()](/words/documents/statistics/) operation.

An object of the **GetDocumentStatisticsOnlineRequest** class is created by the following constructor methods:

- GetDocumentStatisticsOnlineRequest()
- GetDocumentStatisticsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">bool?</span> *includeComments*, <span style="color:SteelBlue;">bool?</span> *includeFootnotes*, <span style="color:SteelBlue;">bool?</span> *includeTextInShapes*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *includeComments*    | IncludeComments      | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to include comments from the WordCount. The default value is "false". |
| *includeFootnotes*   | IncludeFootnotes     | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to include footnotes from the WordCount. The default value is "false". |
| *includeTextInShapes* | IncludeTextInShapes  | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to include shape's text from the WordCount. The default value is "false". |



## GetDocumentStatisticsRequest

Represents a request model for [WordsApi.GetDocumentStatistics()](/words/documents/statistics/) operation.

An object of the **GetDocumentStatisticsRequest** class is created by the following constructor methods:

- GetDocumentStatisticsRequest()
- GetDocumentStatisticsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">bool?</span> *includeComments*, <span style="color:SteelBlue;">bool?</span> *includeFootnotes*, <span style="color:SteelBlue;">bool?</span> *includeTextInShapes*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *includeComments*    | IncludeComments      | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to include comments from the WordCount. The default value is "false". |
| *includeFootnotes*   | IncludeFootnotes     | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to include footnotes from the WordCount. The default value is "false". |
| *includeTextInShapes* | IncludeTextInShapes  | <span style="color:SteelBlue;">bool?</span>   | The flag indicating whether to include shape's text from the WordCount. The default value is "false". |


