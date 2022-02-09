---
title: "WordsApi"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/wordsapi/
description: "WordsApi"
notoc: true
weight: 510
---


## ApiError

Represents a api error.

This class is used in [WordsApiErrorResponse](#wordsapierrorresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Code                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the API error code. |
| DateTime             | <span style="color:SteelBlue;">DateTime</span> | Gets or sets the server DateTime. |
| Description          | <span style="color:SteelBlue;">string</span>  | Gets or sets the error description. |
| Message              | <span style="color:SteelBlue;">string</span>  | Gets or sets the error message. |


## WordsApiLink

Represents a provides information for the words API resource link.

This class is inherited from [Link](/words/spec/document#link) and used in [Bookmark](/words/spec/bookmark#bookmark), [Bookmarks](/words/spec/bookmark#bookmarks), [Border](/words/spec/border#border), [BordersCollection](/words/spec/border#borderscollection), [Comment](/words/spec/comment#comment), [CommentLink](/words/spec/comment#commentlink), [CommentsCollection](/words/spec/comment#commentscollection), [CustomXmlPart](/words/spec/customxmlpart#customxmlpart), [CustomXmlPartInsert](/words/spec/customxmlpart#customxmlpartinsert), [CustomXmlPartLink](/words/spec/customxmlpart#customxmlpartlink), [CustomXmlPartsCollection](/words/spec/customxmlpart#customxmlpartscollection), [CustomXmlPartUpdate](/words/spec/customxmlpart#customxmlpartupdate), [DocumentProperties](/words/spec/documentproperties#documentproperties), [DocumentProperty](/words/spec/documentproperties#documentproperty), [DrawingObject](/words/spec/drawingobject#drawingobject), [DrawingObjectCollection](/words/spec/drawingobject#drawingobjectcollection), [DrawingObjectLink](/words/spec/drawingobject#drawingobjectlink), [Field](/words/spec/field#field), [FieldCollection](/words/spec/field#fieldcollection), [FieldLink](/words/spec/field#fieldlink), [FieldNames](/words/spec/field#fieldnames), [Font](/words/spec/font#font), [Footnote](/words/spec/footnote#footnote), [FootnoteCollection](/words/spec/footnote#footnotecollection), [FootnoteLink](/words/spec/footnote#footnotelink), [FormField](/words/spec/formfield#formfield), [FormFieldCheckbox](/words/spec/formfield#formfieldcheckbox), [FormFieldCollection](/words/spec/formfield#formfieldcollection), [FormFieldDropDown](/words/spec/formfield#formfielddropdown), [FormFieldTextInput](/words/spec/formfield#formfieldtextinput), [HeaderFooter](/words/spec/headerfooter#headerfooter), [HeaderFooterLink](/words/spec/headerfooter#headerfooterlink), [HeaderFooterLinkCollection](/words/spec/headerfooter#headerfooterlinkcollection), [Hyperlink](/words/spec/hyperlink#hyperlink), [Hyperlinks](/words/spec/hyperlink#hyperlinks), [LinkElement](/words/spec/link#linkelement), [ListFormat](/words/spec/paragraphlist#listformat), [ListInfo](/words/spec/list#listinfo), [ListLevel](/words/spec/list#listlevel), [ListLevels](/words/spec/list#listlevels), [Lists](/words/spec/list#lists), [NodeLink](/words/spec/link#nodelink), [OfficeMathLink](/words/spec/link#officemathlink), [OfficeMathObject](/words/spec/mathobject#officemathobject), [OfficeMathObjectsCollection](/words/spec/mathobject#officemathobjectscollection), [PageSetup](/words/spec/section#pagesetup), [Paragraph](/words/spec/paragraph#paragraph), [ParagraphFormat](/words/spec/paragraphformat#paragraphformat), [ParagraphFormatBase](/words/spec/paragraphformat#paragraphformatbase), [ParagraphFormatUpdate](/words/spec/paragraphformat#paragraphformatupdate), [ParagraphLink](/words/spec/paragraph#paragraphlink), [ParagraphLinkCollection](/words/spec/paragraph#paragraphlinkcollection), [Run](/words/spec/run#run), [RunLink](/words/spec/run#runlink), [Runs](/words/spec/run#runs), [SearchResultsCollection](/words/spec/text#searchresultscollection), [Section](/words/spec/section#section), [SectionLink](/words/spec/section#sectionlink), [SectionLinkCollection](/words/spec/section#sectionlinkcollection), [Style](/words/spec/style#style), [Table](/words/spec/table#table), [TableCell](/words/spec/tablecell#tablecell), [TableCellFormat](/words/spec/tablecell#tablecellformat), [TableLink](/words/spec/table#tablelink), [TableLinkCollection](/words/spec/table#tablelinkcollection), [TableProperties](/words/spec/tableproperties#tableproperties), [TableRow](/words/spec/tablerow#tablerow), [TableRowFormat](/words/spec/tablerow#tablerowformat).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Href                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the "href" attribute with the link's IRI. atom:link elements MUST have an href attribute, whose value MUST be a IRI reference. |
| Rel                  | <span style="color:SteelBlue;">string</span>  | Gets or sets the option that controls whether atom:link elements MAY have a "rel" attribute that indicates the link relation type. If the "rel" attribute is not present, the link element MUST be interpreted as if the link relation type is "alternate". |
| Title                | <span style="color:SteelBlue;">string</span>  | Gets or sets the "title" attribute, that conveys human-readable information about the link. The content of the "title" attribute is Language-Sensitive. |
| Type                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the "type" attribute. The "type" attribute's value is an advisory media type: it is a hint about the type of the representation that is expected to be returned when the value of the href attribute is dereferenced. Note that the type attribute does not override the actual media type returned with the representation. |


## WordsApiErrorResponse

Represents a REST response with an API error.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Error                | [ApiError](#apierror)                         | Gets or sets the API error. |


## ApiException

Represents a aPI exception.

An object of the **ApiException** class is created by the following constructor methods:

- ApiException(<span style="color:SteelBlue;">int</span> ***errorCode***, <span style="color:SteelBlue;">string</span> ***message***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***errorCode***      | <span style="color:SteelBlue;">int</span>     | The error code. |
| ***message***        | <span style="color:SteelBlue;">string</span>  | The message. |


### Properties

A single `ErrorCode` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ErrorCode            | <span style="color:SteelBlue;">int</span>     | Error code. |


## Configuration

Represents a set of configuration settings.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ApiBaseUrl           | <span style="color:SteelBlue;">string</span>  | Aspose.Words for Cloud API base URL. |
| ClientId             | <span style="color:SteelBlue;">string</span>  | Gets or sets the client id. |
| ClientSecret         | <span style="color:SteelBlue;">string</span>  | Gets or sets the client secret. |
| Timeout              | <span style="color:SteelBlue;">int</span>     | Gets or sets a request timeout in seconds. Default is 100 seconds. |
| AuthType             | [AuthType](#authtype)                         | Authentication type. Default is OAuth 2.0 |


## WordsApi

Represents a aspose.Words for Cloud API.

An object of the **WordsApi** class is created by the following constructor methods:

- WordsApi(<span style="color:SteelBlue;">string</span> ***clientId***, <span style="color:SteelBlue;">string</span> ***clientSecret***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***clientId***       | <span style="color:SteelBlue;">string</span>  | The client id. |
| ***clientSecret***   | <span style="color:SteelBlue;">string</span>  | The client secret. |

- WordsApi([Configuration](#configuration) ***configuration***)

### Methods

- [RevisionsModificationResponse](/words/spec/documentrevision#revisionsmodificationresponse) **AcceptAllRevisions**([AcceptAllRevisionsRequest](/words/spec/documentrevision#acceptallrevisionsrequest) *request*) - accepts all revisions in the document.
- [AcceptAllRevisionsOnlineResponse](/words/spec/documentrevision#acceptallrevisionsonlineresponse) **AcceptAllRevisionsOnline**([AcceptAllRevisionsOnlineRequest](/words/spec/documentrevision#acceptallrevisionsonlinerequest) *request*) - accepts all revisions in the document.
- [DocumentResponse](/words/spec/document#documentresponse) **AppendDocument**([AppendDocumentRequest](/words/spec/document#appenddocumentrequest) *request*) - appends documents to the original document.
- [AppendDocumentOnlineResponse](/words/spec/document#appenddocumentonlineresponse) **AppendDocumentOnline**([AppendDocumentOnlineRequest](/words/spec/document#appenddocumentonlinerequest) *request*) - appends documents to the original document.
- [WordsResponse](/words/spec/style#wordsresponse) **ApplyStyleToDocumentElement**([ApplyStyleToDocumentElementRequest](/words/spec/style#applystyletodocumentelementrequest) *request*) - applies a style to the document node.
- [ApplyStyleToDocumentElementOnlineResponse](/words/spec/style#applystyletodocumentelementonlineresponse) **ApplyStyleToDocumentElementOnline**([ApplyStyleToDocumentElementOnlineRequest](/words/spec/style#applystyletodocumentelementonlinerequest) *request*) - applies a style to the document node.
- <span style="color:SteelBlue;">object</span> **Batch**([BatchPartRequest](/words/spec/batch#batchpartrequest)[] *requests*) - batch request.
-<span style="color:SteelBlue;">object</span> Batch(<span style="color:SteelBlue;">bool</span> ***displayIntermediateResults***, [BatchPartRequest](/words/spec/batch#batchpartrequest)[] ***requests***)</br>- batch request, where:

<table>
  <tr>
    <td style="vertical-align:top;text-align:right;"><b><i>displayIntermediateResults</i></b></td>
    <td style="vertical-align:top;text-align:center;color:SteelBlue;"><span style="color:SteelBlue;">bool</span></td>
    <td>Display intermediate results or not.</td>
  </tr>
  <tr>
    <td style="vertical-align:top;text-align:right;"><b><i>requests</i></b></td>
    <td style="vertical-align:top;text-align:center;color:SteelBlue;"><a href="/words/spec/batch#batchpartrequest">BatchPartRequest</a>[]</td>
    <td>Array of <see cref="BatchPartRequest" /> requests.</td>
  </tr>
</table>
- [DocumentResponse](/words/spec/document#documentresponse) **BuildReport**([BuildReportRequest](/words/spec/report#buildreportrequest) *request*) - executes the report generation process using the specified document template and the external data source in XML, JSON or CSV format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **BuildReportOnline**([BuildReportOnlineRequest](/words/spec/report#buildreportonlinerequest) *request*) - executes the report generation process online using the specified document template and the external data source in XML, JSON or CSV format.
- [ClassificationResponse](/words/spec/documentclassification#classificationresponse) **Classify**([ClassifyRequest](/words/spec/documentclassification#classifyrequest) *request*) - runs a multi-class text classification for the specified raw text.
- [ClassificationResponse](/words/spec/documentclassification#classificationresponse) **ClassifyDocument**([ClassifyDocumentRequest](/words/spec/documentclassification#classifydocumentrequest) *request*) - runs a multi-class text classification for the document.
- [ClassificationResponse](/words/spec/documentclassification#classificationresponse) **ClassifyDocumentOnline**([ClassifyDocumentOnlineRequest](/words/spec/documentclassification#classifydocumentonlinerequest) *request*) - runs a multi-class text classification for the document.
- [DocumentResponse](/words/spec/document#documentresponse) **CompareDocument**([CompareDocumentRequest](/words/spec/document#comparedocumentrequest) *request*) - compares two documents.
- [CompareDocumentOnlineResponse](/words/spec/document#comparedocumentonlineresponse) **CompareDocumentOnline**([CompareDocumentOnlineRequest](/words/spec/document#comparedocumentonlinerequest) *request*) - compares two documents.
- <span style="color:SteelBlue;">System.IO.Stream</span> **ConvertDocument**([ConvertDocumentRequest](/words/spec/document#convertdocumentrequest) *request*) - converts a document on a local drive to the specified format.
- <span style="color:SteelBlue;">Task</span> **CopyFile**([CopyFileRequest](/words/spec/file#copyfilerequest) *request*) - copy file.
- <span style="color:SteelBlue;">Task</span> **CopyFolder**([CopyFolderRequest](/words/spec/file#copyfolderrequest) *request*) - copy folder.
- [StyleResponse](/words/spec/style#styleresponse) **CopyStyle**([CopyStyleRequest](/words/spec/style#copystylerequest) *request*) - makes a copy of the style in the document.
- [CopyStyleOnlineResponse](/words/spec/style#copystyleonlineresponse) **CopyStyleOnline**([CopyStyleOnlineRequest](/words/spec/style#copystyleonlinerequest) *request*) - makes a copy of the style in the document.
- [DocumentResponse](/words/spec/document#documentresponse) **CreateDocument**([CreateDocumentRequest](/words/spec/document#createdocumentrequest) *request*) - supported extensions: ".doc", ".docx", ".docm", ".dot", ".dotm", ".dotx", ".flatopc", ".fopc", ".flatopc_macro", ".fopc_macro", ".flatopc_template", ".fopc_template", ".flatopc_template_macro", ".fopc_template_macro", ".wordml", ".wml", ".rtf".
- <span style="color:SteelBlue;">Task</span> **CreateFolder**([CreateFolderRequest](/words/spec/file#createfolderrequest) *request*) - create the folder.
- [DocumentPropertyResponse](/words/spec/documentproperties#documentpropertyresponse) **CreateOrUpdateDocumentProperty**([CreateOrUpdateDocumentPropertyRequest](/words/spec/documentproperties#createorupdatedocumentpropertyrequest) *request*) - adds a new or updates an existing document property.
- [CreateOrUpdateDocumentPropertyOnlineResponse](/words/spec/documentproperties#createorupdatedocumentpropertyonlineresponse) **CreateOrUpdateDocumentPropertyOnline**([CreateOrUpdateDocumentPropertyOnlineRequest](/words/spec/documentproperties#createorupdatedocumentpropertyonlinerequest) *request*) - adds a new or updates an existing document property.
- [TabStopsResponse](/words/spec/paragraphtabstop#tabstopsresponse) **DeleteAllParagraphTabStops**([DeleteAllParagraphTabStopsRequest](/words/spec/paragraphtabstop#deleteallparagraphtabstopsrequest) *request*) - removes paragraph tab stops from the document node.
- [DeleteAllParagraphTabStopsOnlineResponse](/words/spec/paragraphtabstop#deleteallparagraphtabstopsonlineresponse) **DeleteAllParagraphTabStopsOnline**([DeleteAllParagraphTabStopsOnlineRequest](/words/spec/paragraphtabstop#deleteallparagraphtabstopsonlinerequest) *request*) - removes paragraph tab stops from the document node.
- [BorderResponse](/words/spec/border#borderresponse) **DeleteBorder**([DeleteBorderRequest](/words/spec/border#deleteborderrequest) *request*) - the 'nodePath' parameter should refer to a paragraph, a cell or a row.
- [DeleteBorderOnlineResponse](/words/spec/border#deleteborderonlineresponse) **DeleteBorderOnline**([DeleteBorderOnlineRequest](/words/spec/border#deleteborderonlinerequest) *request*) - removes a border from the document node.
- [BordersResponse](/words/spec/border#bordersresponse) **DeleteBorders**([DeleteBordersRequest](/words/spec/border#deletebordersrequest) *request*) - the 'nodePath' parameter should refer to a paragraph, a cell or a row.
- [DeleteBordersOnlineResponse](/words/spec/border#deletebordersonlineresponse) **DeleteBordersOnline**([DeleteBordersOnlineRequest](/words/spec/border#deletebordersonlinerequest) *request*) - removes borders from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteComment**([DeleteCommentRequest](/words/spec/comment#deletecommentrequest) *request*) - removes a comment from the document.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteCommentOnline**([DeleteCommentOnlineRequest](/words/spec/comment#deletecommentonlinerequest) *request*) - removes a comment from the document.
- <span style="color:SteelBlue;">Task</span> **DeleteComments**([DeleteCommentsRequest](/words/spec/comment#deletecommentsrequest) *request*) - removes all comments from the document.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteCommentsOnline**([DeleteCommentsOnlineRequest](/words/spec/comment#deletecommentsonlinerequest) *request*) - removes all comments from the document.
- <span style="color:SteelBlue;">Task</span> **DeleteCustomXmlPart**([DeleteCustomXmlPartRequest](/words/spec/customxmlpart#deletecustomxmlpartrequest) *request*) - removes the custom xml part from the document.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteCustomXmlPartOnline**([DeleteCustomXmlPartOnlineRequest](/words/spec/customxmlpart#deletecustomxmlpartonlinerequest) *request*) - removes the custom xml part from the document.
- <span style="color:SteelBlue;">Task</span> **DeleteCustomXmlParts**([DeleteCustomXmlPartsRequest](/words/spec/customxmlpart#deletecustomxmlpartsrequest) *request*) - removes all custom xml parts from the document.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteCustomXmlPartsOnline**([DeleteCustomXmlPartsOnlineRequest](/words/spec/customxmlpart#deletecustomxmlpartsonlinerequest) *request*) - removes all custom xml parts from the document.
- <span style="color:SteelBlue;">Task</span> **DeleteDocumentProperty**([DeleteDocumentPropertyRequest](/words/spec/documentproperties#deletedocumentpropertyrequest) *request*) - removes a document property.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteDocumentPropertyOnline**([DeleteDocumentPropertyOnlineRequest](/words/spec/documentproperties#deletedocumentpropertyonlinerequest) *request*) - removes a document property.
- <span style="color:SteelBlue;">Task</span> **DeleteDrawingObject**([DeleteDrawingObjectRequest](/words/spec/drawingobject#deletedrawingobjectrequest) *request*) - removes a DrawingObject from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteDrawingObjectOnline**([DeleteDrawingObjectOnlineRequest](/words/spec/drawingobject#deletedrawingobjectonlinerequest) *request*) - removes a DrawingObject from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteField**([DeleteFieldRequest](/words/spec/field#deletefieldrequest) *request*) - removes a field from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteFieldOnline**([DeleteFieldOnlineRequest](/words/spec/field#deletefieldonlinerequest) *request*) - removes a field from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteFields**([DeleteFieldsRequest](/words/spec/field#deletefieldsrequest) *request*) - removes fields from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteFieldsOnline**([DeleteFieldsOnlineRequest](/words/spec/field#deletefieldsonlinerequest) *request*) - removes fields from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteFile**([DeleteFileRequest](/words/spec/file#deletefilerequest) *request*) - delete file.
- <span style="color:SteelBlue;">Task</span> **DeleteFolder**([DeleteFolderRequest](/words/spec/file#deletefolderrequest) *request*) - delete folder.
- <span style="color:SteelBlue;">Task</span> **DeleteFootnote**([DeleteFootnoteRequest](/words/spec/footnote#deletefootnoterequest) *request*) - removes a footnote from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteFootnoteOnline**([DeleteFootnoteOnlineRequest](/words/spec/footnote#deletefootnoteonlinerequest) *request*) - removes a footnote from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteFormField**([DeleteFormFieldRequest](/words/spec/formfield#deleteformfieldrequest) *request*) - removes a form field from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteFormFieldOnline**([DeleteFormFieldOnlineRequest](/words/spec/formfield#deleteformfieldonlinerequest) *request*) - removes a form field from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteHeaderFooter**([DeleteHeaderFooterRequest](/words/spec/headerfooter#deleteheaderfooterrequest) *request*) - removes a HeaderFooter object from the document section.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteHeaderFooterOnline**([DeleteHeaderFooterOnlineRequest](/words/spec/headerfooter#deleteheaderfooteronlinerequest) *request*) - removes a HeaderFooter object from the document section.
- <span style="color:SteelBlue;">Task</span> **DeleteHeadersFooters**([DeleteHeadersFootersRequest](/words/spec/headerfooter#deleteheadersfootersrequest) *request*) - removes HeaderFooter objects from the document section.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteHeadersFootersOnline**([DeleteHeadersFootersOnlineRequest](/words/spec/headerfooter#deleteheadersfootersonlinerequest) *request*) - removes HeaderFooter objects from the document section.
- <span style="color:SteelBlue;">Task</span> **DeleteMacros**([DeleteMacrosRequest](/words/spec/macros#deletemacrosrequest) *request*) - removes macros from the document.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteMacrosOnline**([DeleteMacrosOnlineRequest](/words/spec/macros#deletemacrosonlinerequest) *request*) - removes macros from the document.
- <span style="color:SteelBlue;">Task</span> **DeleteOfficeMathObject**([DeleteOfficeMathObjectRequest](/words/spec/mathobject#deleteofficemathobjectrequest) *request*) - removes an OfficeMath object from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteOfficeMathObjectOnline**([DeleteOfficeMathObjectOnlineRequest](/words/spec/mathobject#deleteofficemathobjectonlinerequest) *request*) - removes an OfficeMath object from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteParagraph**([DeleteParagraphRequest](/words/spec/paragraph#deleteparagraphrequest) *request*) - removes a paragraph from the document node.
- [ParagraphListFormatResponse](/words/spec/paragraphlist#paragraphlistformatresponse) **DeleteParagraphListFormat**([DeleteParagraphListFormatRequest](/words/spec/paragraphlist#deleteparagraphlistformatrequest) *request*) - removes the formatting properties of a paragraph list from the document node.
- [DeleteParagraphListFormatOnlineResponse](/words/spec/paragraphlist#deleteparagraphlistformatonlineresponse) **DeleteParagraphListFormatOnline**([DeleteParagraphListFormatOnlineRequest](/words/spec/paragraphlist#deleteparagraphlistformatonlinerequest) *request*) - removes the formatting properties of a paragraph list from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteParagraphOnline**([DeleteParagraphOnlineRequest](/words/spec/paragraph#deleteparagraphonlinerequest) *request*) - removes a paragraph from the document node.
- [TabStopsResponse](/words/spec/paragraphtabstop#tabstopsresponse) **DeleteParagraphTabStop**([DeleteParagraphTabStopRequest](/words/spec/paragraphtabstop#deleteparagraphtabstoprequest) *request*) - removes a paragraph tab stop from the document node.
- [DeleteParagraphTabStopOnlineResponse](/words/spec/paragraphtabstop#deleteparagraphtabstoponlineresponse) **DeleteParagraphTabStopOnline**([DeleteParagraphTabStopOnlineRequest](/words/spec/paragraphtabstop#deleteparagraphtabstoponlinerequest) *request*) - removes a paragraph tab stop from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteRun**([DeleteRunRequest](/words/spec/run#deleterunrequest) *request*) - removes a Run object from the paragraph.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteRunOnline**([DeleteRunOnlineRequest](/words/spec/run#deleterunonlinerequest) *request*) - removes a Run object from the paragraph.
- <span style="color:SteelBlue;">Task</span> **DeleteSection**([DeleteSectionRequest](/words/spec/section#deletesectionrequest) *request*) - removes a section from the document.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteSectionOnline**([DeleteSectionOnlineRequest](/words/spec/section#deletesectiononlinerequest) *request*) - removes a section from the document.
- <span style="color:SteelBlue;">Task</span> **DeleteTable**([DeleteTableRequest](/words/spec/table#deletetablerequest) *request*) - removes a table from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteTableCell**([DeleteTableCellRequest](/words/spec/tablecell#deletetablecellrequest) *request*) - removes a cell from the table row.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteTableCellOnline**([DeleteTableCellOnlineRequest](/words/spec/tablecell#deletetablecellonlinerequest) *request*) - removes a cell from the table row.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteTableOnline**([DeleteTableOnlineRequest](/words/spec/table#deletetableonlinerequest) *request*) - removes a table from the document node.
- <span style="color:SteelBlue;">Task</span> **DeleteTableRow**([DeleteTableRowRequest](/words/spec/tablerow#deletetablerowrequest) *request*) - removes a row from the table.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DeleteTableRowOnline**([DeleteTableRowOnlineRequest](/words/spec/tablerow#deletetablerowonlinerequest) *request*) - removes a row from the table.
- [DocumentResponse](/words/spec/document#documentresponse) **DeleteWatermark**([DeleteWatermarkRequest](/words/spec/watermark#deletewatermarkrequest) *request*) - removes a watermark from the document.
- [DeleteWatermarkOnlineResponse](/words/spec/watermark#deletewatermarkonlineresponse) **DeleteWatermarkOnline**([DeleteWatermarkOnlineRequest](/words/spec/watermark#deletewatermarkonlinerequest) *request*) - removes a watermark from the document.
- <span style="color:SteelBlue;">System.IO.Stream</span> **DownloadFile**([DownloadFileRequest](/words/spec/file#downloadfilerequest) *request*) - download file.
- [DocumentResponse](/words/spec/document#documentresponse) **ExecuteMailMerge**([ExecuteMailMergeRequest](/words/spec/report#executemailmergerequest) *request*) - executes a Mail Merge operation.
- <span style="color:SteelBlue;">System.IO.Stream</span> **ExecuteMailMergeOnline**([ExecuteMailMergeOnlineRequest](/words/spec/report#executemailmergeonlinerequest) *request*) - executes a Mail Merge operation online.
- [AvailableFontsResponse](/words/spec/font#availablefontsresponse) **GetAvailableFonts**([GetAvailableFontsRequest](/words/spec/font#getavailablefontsrequest) *request*) - reads available fonts from the document.
- [BookmarkResponse](/words/spec/bookmark#bookmarkresponse) **GetBookmarkByName**([GetBookmarkByNameRequest](/words/spec/bookmark#getbookmarkbynamerequest) *request*) - reads a bookmark, specified by name, from the document.
- [BookmarkResponse](/words/spec/bookmark#bookmarkresponse) **GetBookmarkByNameOnline**([GetBookmarkByNameOnlineRequest](/words/spec/bookmark#getbookmarkbynameonlinerequest) *request*) - reads a bookmark, specified by name, from the document.
- [BookmarksResponse](/words/spec/bookmark#bookmarksresponse) **GetBookmarks**([GetBookmarksRequest](/words/spec/bookmark#getbookmarksrequest) *request*) - reads bookmarks from the document.
- [BookmarksResponse](/words/spec/bookmark#bookmarksresponse) **GetBookmarksOnline**([GetBookmarksOnlineRequest](/words/spec/bookmark#getbookmarksonlinerequest) *request*) - reads bookmarks from the document.
- [BorderResponse](/words/spec/border#borderresponse) **GetBorder**([GetBorderRequest](/words/spec/border#getborderrequest) *request*) - the 'nodePath' parameter should refer to a paragraph, a cell or a row.
- [BorderResponse](/words/spec/border#borderresponse) **GetBorderOnline**([GetBorderOnlineRequest](/words/spec/border#getborderonlinerequest) *request*) - reads a border from the document node.
- [BordersResponse](/words/spec/border#bordersresponse) **GetBorders**([GetBordersRequest](/words/spec/border#getbordersrequest) *request*) - reads borders from the document node.
- [BordersResponse](/words/spec/border#bordersresponse) **GetBordersOnline**([GetBordersOnlineRequest](/words/spec/border#getbordersonlinerequest) *request*) - reads borders from the document node.
- [CommentResponse](/words/spec/comment#commentresponse) **GetComment**([GetCommentRequest](/words/spec/comment#getcommentrequest) *request*) - reads a comment from the document.
- [CommentResponse](/words/spec/comment#commentresponse) **GetCommentOnline**([GetCommentOnlineRequest](/words/spec/comment#getcommentonlinerequest) *request*) - reads a comment from the document.
- [CommentsResponse](/words/spec/comment#commentsresponse) **GetComments**([GetCommentsRequest](/words/spec/comment#getcommentsrequest) *request*) - reads comments from the document.
- [CommentsResponse](/words/spec/comment#commentsresponse) **GetCommentsOnline**([GetCommentsOnlineRequest](/words/spec/comment#getcommentsonlinerequest) *request*) - reads comments from the document.
- [CustomXmlPartResponse](/words/spec/customxmlpart#customxmlpartresponse) **GetCustomXmlPart**([GetCustomXmlPartRequest](/words/spec/customxmlpart#getcustomxmlpartrequest) *request*) - reads the custom xml part from the document.
- [CustomXmlPartResponse](/words/spec/customxmlpart#customxmlpartresponse) **GetCustomXmlPartOnline**([GetCustomXmlPartOnlineRequest](/words/spec/customxmlpart#getcustomxmlpartonlinerequest) *request*) - reads the custom xml part from the document.
- [CustomXmlPartsResponse](/words/spec/customxmlpart#customxmlpartsresponse) **GetCustomXmlParts**([GetCustomXmlPartsRequest](/words/spec/customxmlpart#getcustomxmlpartsrequest) *request*) - reads custom xml parts from the document.
- [CustomXmlPartsResponse](/words/spec/customxmlpart#customxmlpartsresponse) **GetCustomXmlPartsOnline**([GetCustomXmlPartsOnlineRequest](/words/spec/customxmlpart#getcustomxmlpartsonlinerequest) *request*) - reads custom xml parts from the document.
- [DocumentResponse](/words/spec/document#documentresponse) **GetDocument**([GetDocumentRequest](/words/spec/document#getdocumentrequest) *request*) - reads common information from the document.
- [DrawingObjectResponse](/words/spec/drawingobject#drawingobjectresponse) **GetDocumentDrawingObjectByIndex**([GetDocumentDrawingObjectByIndexRequest](/words/spec/drawingobject#getdocumentdrawingobjectbyindexrequest) *request*) - reads a DrawingObject from the document node.
- [DrawingObjectResponse](/words/spec/drawingobject#drawingobjectresponse) **GetDocumentDrawingObjectByIndexOnline**([GetDocumentDrawingObjectByIndexOnlineRequest](/words/spec/drawingobject#getdocumentdrawingobjectbyindexonlinerequest) *request*) - reads a DrawingObject from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **GetDocumentDrawingObjectImageData**([GetDocumentDrawingObjectImageDataRequest](/words/spec/drawingobject#getdocumentdrawingobjectimagedatarequest) *request*) - reads image data of a DrawingObject from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **GetDocumentDrawingObjectImageDataOnline**([GetDocumentDrawingObjectImageDataOnlineRequest](/words/spec/drawingobject#getdocumentdrawingobjectimagedataonlinerequest) *request*) - reads image data of a DrawingObject from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **GetDocumentDrawingObjectOleData**([GetDocumentDrawingObjectOleDataRequest](/words/spec/drawingobject#getdocumentdrawingobjectoledatarequest) *request*) - reads OLE data of a DrawingObject from the document node.
- <span style="color:SteelBlue;">System.IO.Stream</span> **GetDocumentDrawingObjectOleDataOnline**([GetDocumentDrawingObjectOleDataOnlineRequest](/words/spec/drawingobject#getdocumentdrawingobjectoledataonlinerequest) *request*) - reads OLE data of a DrawingObject from the document node.
- [DrawingObjectsResponse](/words/spec/drawingobject#drawingobjectsresponse) **GetDocumentDrawingObjects**([GetDocumentDrawingObjectsRequest](/words/spec/drawingobject#getdocumentdrawingobjectsrequest) *request*) - reads DrawingObjects from the document node.
- [DrawingObjectsResponse](/words/spec/drawingobject#drawingobjectsresponse) **GetDocumentDrawingObjectsOnline**([GetDocumentDrawingObjectsOnlineRequest](/words/spec/drawingobject#getdocumentdrawingobjectsonlinerequest) *request*) - reads DrawingObjects from the document node.
- [FieldNamesResponse](/words/spec/field#fieldnamesresponse) **GetDocumentFieldNames**([GetDocumentFieldNamesRequest](/words/spec/field#getdocumentfieldnamesrequest) *request*) - reads merge field names from the document.
- [FieldNamesResponse](/words/spec/field#fieldnamesresponse) **GetDocumentFieldNamesOnline**([GetDocumentFieldNamesOnlineRequest](/words/spec/field#getdocumentfieldnamesonlinerequest) *request*) - reads merge field names from the document.
- [HyperlinkResponse](/words/spec/hyperlink#hyperlinkresponse) **GetDocumentHyperlinkByIndex**([GetDocumentHyperlinkByIndexRequest](/words/spec/hyperlink#getdocumenthyperlinkbyindexrequest) *request*) - reads a hyperlink from the document.
- [HyperlinkResponse](/words/spec/hyperlink#hyperlinkresponse) **GetDocumentHyperlinkByIndexOnline**([GetDocumentHyperlinkByIndexOnlineRequest](/words/spec/hyperlink#getdocumenthyperlinkbyindexonlinerequest) *request*) - reads a hyperlink from the document.
- [HyperlinksResponse](/words/spec/hyperlink#hyperlinksresponse) **GetDocumentHyperlinks**([GetDocumentHyperlinksRequest](/words/spec/hyperlink#getdocumenthyperlinksrequest) *request*) - reads hyperlinks from the document.
- [HyperlinksResponse](/words/spec/hyperlink#hyperlinksresponse) **GetDocumentHyperlinksOnline**([GetDocumentHyperlinksOnlineRequest](/words/spec/hyperlink#getdocumenthyperlinksonlinerequest) *request*) - reads hyperlinks from the document.
- [DocumentPropertiesResponse](/words/spec/documentproperties#documentpropertiesresponse) **GetDocumentProperties**([GetDocumentPropertiesRequest](/words/spec/documentproperties#getdocumentpropertiesrequest) *request*) - reads document properties.
- [DocumentPropertiesResponse](/words/spec/documentproperties#documentpropertiesresponse) **GetDocumentPropertiesOnline**([GetDocumentPropertiesOnlineRequest](/words/spec/documentproperties#getdocumentpropertiesonlinerequest) *request*) - reads document properties.
- [DocumentPropertyResponse](/words/spec/documentproperties#documentpropertyresponse) **GetDocumentProperty**([GetDocumentPropertyRequest](/words/spec/documentproperties#getdocumentpropertyrequest) *request*) - reads a document property.
- [DocumentPropertyResponse](/words/spec/documentproperties#documentpropertyresponse) **GetDocumentPropertyOnline**([GetDocumentPropertyOnlineRequest](/words/spec/documentproperties#getdocumentpropertyonlinerequest) *request*) - reads a document property.
- [ProtectionDataResponse](/words/spec/documentprotection#protectiondataresponse) **GetDocumentProtection**([GetDocumentProtectionRequest](/words/spec/documentprotection#getdocumentprotectionrequest) *request*) - reads protection properties from the document.
- [ProtectionDataResponse](/words/spec/documentprotection#protectiondataresponse) **GetDocumentProtectionOnline**([GetDocumentProtectionOnlineRequest](/words/spec/documentprotection#getdocumentprotectiononlinerequest) *request*) - reads protection properties from the document.
- [StatDataResponse](/words/spec/documentstatistics#statdataresponse) **GetDocumentStatistics**([GetDocumentStatisticsRequest](/words/spec/documentstatistics#getdocumentstatisticsrequest) *request*) - reads document statistics.
- [StatDataResponse](/words/spec/documentstatistics#statdataresponse) **GetDocumentStatisticsOnline**([GetDocumentStatisticsOnlineRequest](/words/spec/documentstatistics#getdocumentstatisticsonlinerequest) *request*) - reads document statistics.
- <span style="color:SteelBlue;">System.IO.Stream</span> **GetDocumentWithFormat**([GetDocumentWithFormatRequest](/words/spec/document#getdocumentwithformatrequest) *request*) - converts a document in cloud storage to the specified format.
- [FieldResponse](/words/spec/field#fieldresponse) **GetField**([GetFieldRequest](/words/spec/field#getfieldrequest) *request*) - reads a field from the document node.
- [FieldResponse](/words/spec/field#fieldresponse) **GetFieldOnline**([GetFieldOnlineRequest](/words/spec/field#getfieldonlinerequest) *request*) - reads a field from the document node.
- [FieldsResponse](/words/spec/field#fieldsresponse) **GetFields**([GetFieldsRequest](/words/spec/field#getfieldsrequest) *request*) - reads fields from the document node.
- [FieldsResponse](/words/spec/field#fieldsresponse) **GetFieldsOnline**([GetFieldsOnlineRequest](/words/spec/field#getfieldsonlinerequest) *request*) - reads fields from the document node.
- [FilesList](/words/spec/file#fileslist) **GetFilesList**([GetFilesListRequest](/words/spec/file#getfileslistrequest) *request*) - get all files and folders within a folder.
- [FootnoteResponse](/words/spec/footnote#footnoteresponse) **GetFootnote**([GetFootnoteRequest](/words/spec/footnote#getfootnoterequest) *request*) - reads a footnote from the document node.
- [FootnoteResponse](/words/spec/footnote#footnoteresponse) **GetFootnoteOnline**([GetFootnoteOnlineRequest](/words/spec/footnote#getfootnoteonlinerequest) *request*) - reads a footnote from the document node.
- [FootnotesResponse](/words/spec/footnote#footnotesresponse) **GetFootnotes**([GetFootnotesRequest](/words/spec/footnote#getfootnotesrequest) *request*) - reads footnotes from the document node.
- [FootnotesResponse](/words/spec/footnote#footnotesresponse) **GetFootnotesOnline**([GetFootnotesOnlineRequest](/words/spec/footnote#getfootnotesonlinerequest) *request*) - reads footnotes from the document node.
- [FormFieldResponse](/words/spec/formfield#formfieldresponse) **GetFormField**([GetFormFieldRequest](/words/spec/formfield#getformfieldrequest) *request*) - reads a form field from the document node.
- [FormFieldResponse](/words/spec/formfield#formfieldresponse) **GetFormFieldOnline**([GetFormFieldOnlineRequest](/words/spec/formfield#getformfieldonlinerequest) *request*) - reads a form field from the document node.
- [FormFieldsResponse](/words/spec/formfield#formfieldsresponse) **GetFormFields**([GetFormFieldsRequest](/words/spec/formfield#getformfieldsrequest) *request*) - reads form fields from the document node.
- [FormFieldsResponse](/words/spec/formfield#formfieldsresponse) **GetFormFieldsOnline**([GetFormFieldsOnlineRequest](/words/spec/formfield#getformfieldsonlinerequest) *request*) - reads form fields from the document node.
- [HeaderFooterResponse](/words/spec/headerfooter#headerfooterresponse) **GetHeaderFooter**([GetHeaderFooterRequest](/words/spec/headerfooter#getheaderfooterrequest) *request*) - reads a HeaderFooter object from the document.
- [HeaderFooterResponse](/words/spec/headerfooter#headerfooterresponse) **GetHeaderFooterOfSection**([GetHeaderFooterOfSectionRequest](/words/spec/headerfooter#getheaderfooterofsectionrequest) *request*) - reads a HeaderFooter object from the document section.
- [HeaderFooterResponse](/words/spec/headerfooter#headerfooterresponse) **GetHeaderFooterOfSectionOnline**([GetHeaderFooterOfSectionOnlineRequest](/words/spec/headerfooter#getheaderfooterofsectiononlinerequest) *request*) - reads a HeaderFooter object from the document section.
- [HeaderFooterResponse](/words/spec/headerfooter#headerfooterresponse) **GetHeaderFooterOnline**([GetHeaderFooterOnlineRequest](/words/spec/headerfooter#getheaderfooteronlinerequest) *request*) - reads a HeaderFooter object from the document.
- [HeaderFootersResponse](/words/spec/headerfooter#headerfootersresponse) **GetHeaderFooters**([GetHeaderFootersRequest](/words/spec/headerfooter#getheaderfootersrequest) *request*) - reads HeaderFooter objects from the document section.
- [HeaderFootersResponse](/words/spec/headerfooter#headerfootersresponse) **GetHeaderFootersOnline**([GetHeaderFootersOnlineRequest](/words/spec/headerfooter#getheaderfootersonlinerequest) *request*) - reads HeaderFooter objects from the document section.
- [InfoResponse](/words/spec/other#inforesponse) **GetInfo**([GetInfoRequest](/words/spec/other#getinforequest) *request*) - returns application info.
- [ListResponse](/words/spec/list#listresponse) **GetList**([GetListRequest](/words/spec/list#getlistrequest) *request*) - reads a list from the document.
- [ListResponse](/words/spec/list#listresponse) **GetListOnline**([GetListOnlineRequest](/words/spec/list#getlistonlinerequest) *request*) - reads a list from the document.
- [ListsResponse](/words/spec/list#listsresponse) **GetLists**([GetListsRequest](/words/spec/list#getlistsrequest) *request*) - reads lists from the document.
- [ListsResponse](/words/spec/list#listsresponse) **GetListsOnline**([GetListsOnlineRequest](/words/spec/list#getlistsonlinerequest) *request*) - reads lists from the document.
- [OfficeMathObjectResponse](/words/spec/mathobject#officemathobjectresponse) **GetOfficeMathObject**([GetOfficeMathObjectRequest](/words/spec/mathobject#getofficemathobjectrequest) *request*) - reads an OfficeMath object from the document node.
- [OfficeMathObjectResponse](/words/spec/mathobject#officemathobjectresponse) **GetOfficeMathObjectOnline**([GetOfficeMathObjectOnlineRequest](/words/spec/mathobject#getofficemathobjectonlinerequest) *request*) - reads an OfficeMath object from the document node.
- [OfficeMathObjectsResponse](/words/spec/mathobject#officemathobjectsresponse) **GetOfficeMathObjects**([GetOfficeMathObjectsRequest](/words/spec/mathobject#getofficemathobjectsrequest) *request*) - reads OfficeMath objects from the document node.
- [OfficeMathObjectsResponse](/words/spec/mathobject#officemathobjectsresponse) **GetOfficeMathObjectsOnline**([GetOfficeMathObjectsOnlineRequest](/words/spec/mathobject#getofficemathobjectsonlinerequest) *request*) - reads OfficeMath objects from the document node.
- [ParagraphResponse](/words/spec/paragraph#paragraphresponse) **GetParagraph**([GetParagraphRequest](/words/spec/paragraph#getparagraphrequest) *request*) - reads a paragraph from the document node.
- [ParagraphFormatResponse](/words/spec/paragraphformat#paragraphformatresponse) **GetParagraphFormat**([GetParagraphFormatRequest](/words/spec/paragraphformat#getparagraphformatrequest) *request*) - reads the formatting properties of a paragraph from the document node.
- [ParagraphFormatResponse](/words/spec/paragraphformat#paragraphformatresponse) **GetParagraphFormatOnline**([GetParagraphFormatOnlineRequest](/words/spec/paragraphformat#getparagraphformatonlinerequest) *request*) - reads the formatting properties of a paragraph from the document node.
- [ParagraphListFormatResponse](/words/spec/paragraphlist#paragraphlistformatresponse) **GetParagraphListFormat**([GetParagraphListFormatRequest](/words/spec/paragraphlist#getparagraphlistformatrequest) *request*) - reads the formatting properties of a paragraph list from the document node.
- [ParagraphListFormatResponse](/words/spec/paragraphlist#paragraphlistformatresponse) **GetParagraphListFormatOnline**([GetParagraphListFormatOnlineRequest](/words/spec/paragraphlist#getparagraphlistformatonlinerequest) *request*) - reads the formatting properties of a paragraph list from the document node.
- [ParagraphResponse](/words/spec/paragraph#paragraphresponse) **GetParagraphOnline**([GetParagraphOnlineRequest](/words/spec/paragraph#getparagraphonlinerequest) *request*) - reads a paragraph from the document node.
- [ParagraphLinkCollectionResponse](/words/spec/paragraph#paragraphlinkcollectionresponse) **GetParagraphs**([GetParagraphsRequest](/words/spec/paragraph#getparagraphsrequest) *request*) - reads paragraphs from the document node.
- [ParagraphLinkCollectionResponse](/words/spec/paragraph#paragraphlinkcollectionresponse) **GetParagraphsOnline**([GetParagraphsOnlineRequest](/words/spec/paragraph#getparagraphsonlinerequest) *request*) - reads paragraphs from the document node.
- [TabStopsResponse](/words/spec/paragraphtabstop#tabstopsresponse) **GetParagraphTabStops**([GetParagraphTabStopsRequest](/words/spec/paragraphtabstop#getparagraphtabstopsrequest) *request*) - reads paragraph tab stops from the document node.
- [TabStopsResponse](/words/spec/paragraphtabstop#tabstopsresponse) **GetParagraphTabStopsOnline**([GetParagraphTabStopsOnlineRequest](/words/spec/paragraphtabstop#getparagraphtabstopsonlinerequest) *request*) - reads paragraph tab stops from the document node.
- [PublicKeyResponse](/words/spec/other#publickeyresponse) **GetPublicKey**([GetPublicKeyRequest](/words/spec/other#getpublickeyrequest) *request*) - get assymetric public key.
- [RangeTextResponse](/words/spec/range#rangetextresponse) **GetRangeText**([GetRangeTextRequest](/words/spec/range#getrangetextrequest) *request*) - reads range text from the document.
- [RangeTextResponse](/words/spec/range#rangetextresponse) **GetRangeTextOnline**([GetRangeTextOnlineRequest](/words/spec/range#getrangetextonlinerequest) *request*) - reads range text from the document.
- [RunResponse](/words/spec/run#runresponse) **GetRun**([GetRunRequest](/words/spec/run#getrunrequest) *request*) - reads a Run object from the paragraph.
- [FontResponse](/words/spec/run#fontresponse) **GetRunFont**([GetRunFontRequest](/words/spec/run#getrunfontrequest) *request*) - reads the font properties of a Run object from the paragraph.
- [FontResponse](/words/spec/run#fontresponse) **GetRunFontOnline**([GetRunFontOnlineRequest](/words/spec/run#getrunfontonlinerequest) *request*) - reads the font properties of a Run object from the paragraph.
- [RunResponse](/words/spec/run#runresponse) **GetRunOnline**([GetRunOnlineRequest](/words/spec/run#getrunonlinerequest) *request*) - reads a Run object from the paragraph.
- [RunsResponse](/words/spec/run#runsresponse) **GetRuns**([GetRunsRequest](/words/spec/run#getrunsrequest) *request*) - reads Run objects from the paragraph.
- [RunsResponse](/words/spec/run#runsresponse) **GetRunsOnline**([GetRunsOnlineRequest](/words/spec/run#getrunsonlinerequest) *request*) - reads Run objects from the paragraph.
- [SectionResponse](/words/spec/section#sectionresponse) **GetSection**([GetSectionRequest](/words/spec/section#getsectionrequest) *request*) - reads a section from the document.
- [SectionResponse](/words/spec/section#sectionresponse) **GetSectionOnline**([GetSectionOnlineRequest](/words/spec/section#getsectiononlinerequest) *request*) - reads a section from the document.
- [SectionPageSetupResponse](/words/spec/section#sectionpagesetupresponse) **GetSectionPageSetup**([GetSectionPageSetupRequest](/words/spec/section#getsectionpagesetuprequest) *request*) - reads the page setup of a section from the document.
- [SectionPageSetupResponse](/words/spec/section#sectionpagesetupresponse) **GetSectionPageSetupOnline**([GetSectionPageSetupOnlineRequest](/words/spec/section#getsectionpagesetuponlinerequest) *request*) - reads the page setup of a section from the document.
- [SectionLinkCollectionResponse](/words/spec/section#sectionlinkcollectionresponse) **GetSections**([GetSectionsRequest](/words/spec/section#getsectionsrequest) *request*) - reads sections from the document.
- [SectionLinkCollectionResponse](/words/spec/section#sectionlinkcollectionresponse) **GetSectionsOnline**([GetSectionsOnlineRequest](/words/spec/section#getsectionsonlinerequest) *request*) - reads sections from the document.
- [StyleResponse](/words/spec/style#styleresponse) **GetStyle**([GetStyleRequest](/words/spec/style#getstylerequest) *request*) - reads a style from the document.
- [StyleResponse](/words/spec/style#styleresponse) **GetStyleFromDocumentElement**([GetStyleFromDocumentElementRequest](/words/spec/style#getstylefromdocumentelementrequest) *request*) - reads a style from the document node.
- [StyleResponse](/words/spec/style#styleresponse) **GetStyleFromDocumentElementOnline**([GetStyleFromDocumentElementOnlineRequest](/words/spec/style#getstylefromdocumentelementonlinerequest) *request*) - reads a style from the document node.
- [StyleResponse](/words/spec/style#styleresponse) **GetStyleOnline**([GetStyleOnlineRequest](/words/spec/style#getstyleonlinerequest) *request*) - reads a style from the document.
- [StylesResponse](/words/spec/style#stylesresponse) **GetStyles**([GetStylesRequest](/words/spec/style#getstylesrequest) *request*) - reads styles from the document.
- [StylesResponse](/words/spec/style#stylesresponse) **GetStylesOnline**([GetStylesOnlineRequest](/words/spec/style#getstylesonlinerequest) *request*) - reads styles from the document.
- [TableResponse](/words/spec/table#tableresponse) **GetTable**([GetTableRequest](/words/spec/table#gettablerequest) *request*) - reads a table from the document node.
- [TableCellResponse](/words/spec/tablecell#tablecellresponse) **GetTableCell**([GetTableCellRequest](/words/spec/tablecell#gettablecellrequest) *request*) - reads a cell from the table row.
- [TableCellFormatResponse](/words/spec/tablecell#tablecellformatresponse) **GetTableCellFormat**([GetTableCellFormatRequest](/words/spec/tablecell#gettablecellformatrequest) *request*) - reads the formatting properties of a table cell.
- [TableCellFormatResponse](/words/spec/tablecell#tablecellformatresponse) **GetTableCellFormatOnline**([GetTableCellFormatOnlineRequest](/words/spec/tablecell#gettablecellformatonlinerequest) *request*) - reads the formatting properties of a table cell.
- [TableCellResponse](/words/spec/tablecell#tablecellresponse) **GetTableCellOnline**([GetTableCellOnlineRequest](/words/spec/tablecell#gettablecellonlinerequest) *request*) - reads a cell from the table row.
- [TableResponse](/words/spec/table#tableresponse) **GetTableOnline**([GetTableOnlineRequest](/words/spec/table#gettableonlinerequest) *request*) - reads a table from the document node.
- [TablePropertiesResponse](/words/spec/tableproperties#tablepropertiesresponse) **GetTableProperties**([GetTablePropertiesRequest](/words/spec/tableproperties#gettablepropertiesrequest) *request*) - reads properties of a table from the document node.
- [TablePropertiesResponse](/words/spec/tableproperties#tablepropertiesresponse) **GetTablePropertiesOnline**([GetTablePropertiesOnlineRequest](/words/spec/tableproperties#gettablepropertiesonlinerequest) *request*) - reads properties of a table from the document node.
- [TableRowResponse](/words/spec/tablerow#tablerowresponse) **GetTableRow**([GetTableRowRequest](/words/spec/tablerow#gettablerowrequest) *request*) - reads a row from the table.
- [TableRowFormatResponse](/words/spec/tablerow#tablerowformatresponse) **GetTableRowFormat**([GetTableRowFormatRequest](/words/spec/tablerow#gettablerowformatrequest) *request*) - reads the formatting properties of a table row.
- [TableRowFormatResponse](/words/spec/tablerow#tablerowformatresponse) **GetTableRowFormatOnline**([GetTableRowFormatOnlineRequest](/words/spec/tablerow#gettablerowformatonlinerequest) *request*) - reads the formatting properties of a table row.
- [TableRowResponse](/words/spec/tablerow#tablerowresponse) **GetTableRowOnline**([GetTableRowOnlineRequest](/words/spec/tablerow#gettablerowonlinerequest) *request*) - reads a row from the table.
- [TableLinkCollectionResponse](/words/spec/table#tablelinkcollectionresponse) **GetTables**([GetTablesRequest](/words/spec/table#gettablesrequest) *request*) - reads tables from the document node.
- [TableLinkCollectionResponse](/words/spec/table#tablelinkcollectionresponse) **GetTablesOnline**([GetTablesOnlineRequest](/words/spec/table#gettablesonlinerequest) *request*) - reads tables from the document node.
- [CommentResponse](/words/spec/comment#commentresponse) **InsertComment**([InsertCommentRequest](/words/spec/comment#insertcommentrequest) *request*) - inserts a new comment to the document.
- [InsertCommentOnlineResponse](/words/spec/comment#insertcommentonlineresponse) **InsertCommentOnline**([InsertCommentOnlineRequest](/words/spec/comment#insertcommentonlinerequest) *request*) - inserts a new comment to the document.
- [CustomXmlPartResponse](/words/spec/customxmlpart#customxmlpartresponse) **InsertCustomXmlPart**([InsertCustomXmlPartRequest](/words/spec/customxmlpart#insertcustomxmlpartrequest) *request*) - inserts a new custom xml part to the document.
- [InsertCustomXmlPartOnlineResponse](/words/spec/customxmlpart#insertcustomxmlpartonlineresponse) **InsertCustomXmlPartOnline**([InsertCustomXmlPartOnlineRequest](/words/spec/customxmlpart#insertcustomxmlpartonlinerequest) *request*) - inserts a new custom xml part to the document.
- [DrawingObjectResponse](/words/spec/drawingobject#drawingobjectresponse) **InsertDrawingObject**([InsertDrawingObjectRequest](/words/spec/drawingobject#insertdrawingobjectrequest) *request*) - inserts a new DrawingObject to the document node.
- [InsertDrawingObjectOnlineResponse](/words/spec/drawingobject#insertdrawingobjectonlineresponse) **InsertDrawingObjectOnline**([InsertDrawingObjectOnlineRequest](/words/spec/drawingobject#insertdrawingobjectonlinerequest) *request*) - inserts a new DrawingObject to the document node.
- [FieldResponse](/words/spec/field#fieldresponse) **InsertField**([InsertFieldRequest](/words/spec/field#insertfieldrequest) *request*) - inserts a new field to the document node.
- [InsertFieldOnlineResponse](/words/spec/field#insertfieldonlineresponse) **InsertFieldOnline**([InsertFieldOnlineRequest](/words/spec/field#insertfieldonlinerequest) *request*) - inserts a new field to the document node.
- [FootnoteResponse](/words/spec/footnote#footnoteresponse) **InsertFootnote**([InsertFootnoteRequest](/words/spec/footnote#insertfootnoterequest) *request*) - inserts a new footnote to the document node.
- [InsertFootnoteOnlineResponse](/words/spec/footnote#insertfootnoteonlineresponse) **InsertFootnoteOnline**([InsertFootnoteOnlineRequest](/words/spec/footnote#insertfootnoteonlinerequest) *request*) - inserts a new footnote to the document node.
- [FormFieldResponse](/words/spec/formfield#formfieldresponse) **InsertFormField**([InsertFormFieldRequest](/words/spec/formfield#insertformfieldrequest) *request*) - inserts a new form field to the document node.
- [InsertFormFieldOnlineResponse](/words/spec/formfield#insertformfieldonlineresponse) **InsertFormFieldOnline**([InsertFormFieldOnlineRequest](/words/spec/formfield#insertformfieldonlinerequest) *request*) - inserts a new form field to the document node.
- [HeaderFooterResponse](/words/spec/headerfooter#headerfooterresponse) **InsertHeaderFooter**([InsertHeaderFooterRequest](/words/spec/headerfooter#insertheaderfooterrequest) *request*) - inserts a new HeaderFooter object to the document section.
- [InsertHeaderFooterOnlineResponse](/words/spec/headerfooter#insertheaderfooteronlineresponse) **InsertHeaderFooterOnline**([InsertHeaderFooterOnlineRequest](/words/spec/headerfooter#insertheaderfooteronlinerequest) *request*) - inserts a new HeaderFooter object to the document section.
- [ListResponse](/words/spec/list#listresponse) **InsertList**([InsertListRequest](/words/spec/list#insertlistrequest) *request*) - inserts a new list to the document.
- [InsertListOnlineResponse](/words/spec/list#insertlistonlineresponse) **InsertListOnline**([InsertListOnlineRequest](/words/spec/list#insertlistonlinerequest) *request*) - inserts a new list to the document.
- [TabStopsResponse](/words/spec/paragraphtabstop#tabstopsresponse) **InsertOrUpdateParagraphTabStop**([InsertOrUpdateParagraphTabStopRequest](/words/spec/paragraphtabstop#insertorupdateparagraphtabstoprequest) *request*) - inserts a new or updates an existing paragraph tab stop in the document node.
- [InsertOrUpdateParagraphTabStopOnlineResponse](/words/spec/paragraphtabstop#insertorupdateparagraphtabstoponlineresponse) **InsertOrUpdateParagraphTabStopOnline**([InsertOrUpdateParagraphTabStopOnlineRequest](/words/spec/paragraphtabstop#insertorupdateparagraphtabstoponlinerequest) *request*) - inserts a new or updates an existing paragraph tab stop in the document node.
- [DocumentResponse](/words/spec/document#documentresponse) **InsertPageNumbers**([InsertPageNumbersRequest](/words/spec/page#insertpagenumbersrequest) *request*) - inserts page numbers to the document.
- [InsertPageNumbersOnlineResponse](/words/spec/page#insertpagenumbersonlineresponse) **InsertPageNumbersOnline**([InsertPageNumbersOnlineRequest](/words/spec/page#insertpagenumbersonlinerequest) *request*) - inserts page numbers to the document.
- [ParagraphResponse](/words/spec/paragraph#paragraphresponse) **InsertParagraph**([InsertParagraphRequest](/words/spec/paragraph#insertparagraphrequest) *request*) - inserts a new paragraph to the document node.
- [InsertParagraphOnlineResponse](/words/spec/paragraph#insertparagraphonlineresponse) **InsertParagraphOnline**([InsertParagraphOnlineRequest](/words/spec/paragraph#insertparagraphonlinerequest) *request*) - inserts a new paragraph to the document node.
- [RunResponse](/words/spec/run#runresponse) **InsertRun**([InsertRunRequest](/words/spec/run#insertrunrequest) *request*) - inserts a new Run object to the paragraph.
- [InsertRunOnlineResponse](/words/spec/run#insertrunonlineresponse) **InsertRunOnline**([InsertRunOnlineRequest](/words/spec/run#insertrunonlinerequest) *request*) - inserts a new Run object to the paragraph.
- [StyleResponse](/words/spec/style#styleresponse) **InsertStyle**([InsertStyleRequest](/words/spec/style#insertstylerequest) *request*) - inserts a new style to the document.
- [InsertStyleOnlineResponse](/words/spec/style#insertstyleonlineresponse) **InsertStyleOnline**([InsertStyleOnlineRequest](/words/spec/style#insertstyleonlinerequest) *request*) - inserts a new style to the document.
- [TableResponse](/words/spec/table#tableresponse) **InsertTable**([InsertTableRequest](/words/spec/table#inserttablerequest) *request*) - inserts a new table to the document node.
- [TableCellResponse](/words/spec/tablecell#tablecellresponse) **InsertTableCell**([InsertTableCellRequest](/words/spec/tablecell#inserttablecellrequest) *request*) - inserts a new cell to the table row.
- [InsertTableCellOnlineResponse](/words/spec/tablecell#inserttablecellonlineresponse) **InsertTableCellOnline**([InsertTableCellOnlineRequest](/words/spec/tablecell#inserttablecellonlinerequest) *request*) - inserts a new cell to the table row.
- [InsertTableOnlineResponse](/words/spec/table#inserttableonlineresponse) **InsertTableOnline**([InsertTableOnlineRequest](/words/spec/table#inserttableonlinerequest) *request*) - inserts a new table to the document node.
- [TableRowResponse](/words/spec/tablerow#tablerowresponse) **InsertTableRow**([InsertTableRowRequest](/words/spec/tablerow#inserttablerowrequest) *request*) - inserts a new row to the table.
- [InsertTableRowOnlineResponse](/words/spec/tablerow#inserttablerowonlineresponse) **InsertTableRowOnline**([InsertTableRowOnlineRequest](/words/spec/tablerow#inserttablerowonlinerequest) *request*) - inserts a new row to the table.
- [DocumentResponse](/words/spec/document#documentresponse) **InsertWatermarkImage**([InsertWatermarkImageRequest](/words/spec/watermark#insertwatermarkimagerequest) *request*) - inserts a new watermark image to the document.
- [InsertWatermarkImageOnlineResponse](/words/spec/watermark#insertwatermarkimageonlineresponse) **InsertWatermarkImageOnline**([InsertWatermarkImageOnlineRequest](/words/spec/watermark#insertwatermarkimageonlinerequest) *request*) - inserts a new watermark image to the document.
- [DocumentResponse](/words/spec/document#documentresponse) **InsertWatermarkText**([InsertWatermarkTextRequest](/words/spec/watermark#insertwatermarktextrequest) *request*) - inserts a new watermark text to the document.
- [InsertWatermarkTextOnlineResponse](/words/spec/watermark#insertwatermarktextonlineresponse) **InsertWatermarkTextOnline**([InsertWatermarkTextOnlineRequest](/words/spec/watermark#insertwatermarktextonlinerequest) *request*) - inserts a new watermark text to the document.
- [SaveResponse](/words/spec/document#saveresponse) **LoadWebDocument**([LoadWebDocumentRequest](/words/spec/document#loadwebdocumentrequest) *request*) - downloads a document from the Web using URL and saves it to cloud storage in the specified format.
- <span style="color:SteelBlue;">Task</span> **MoveFile**([MoveFileRequest](/words/spec/file#movefilerequest) *request*) - move file.
- <span style="color:SteelBlue;">Task</span> **MoveFolder**([MoveFolderRequest](/words/spec/file#movefolderrequest) *request*) - move folder.
- <span style="color:SteelBlue;">Task</span> **OptimizeDocument**([OptimizeDocumentRequest](/words/spec/document#optimizedocumentrequest) *request*) - applies document content optimization options, specific to a particular versions of Microsoft Word.
- <span style="color:SteelBlue;">System.IO.Stream</span> **OptimizeDocumentOnline**([OptimizeDocumentOnlineRequest](/words/spec/document#optimizedocumentonlinerequest) *request*) - applies document content optimization options, specific to a particular versions of Microsoft Word.
- [ProtectionDataResponse](/words/spec/documentprotection#protectiondataresponse) **ProtectDocument**([ProtectDocumentRequest](/words/spec/documentprotection#protectdocumentrequest) *request*) - adds protection to the document.
- [ProtectDocumentOnlineResponse](/words/spec/documentprotection#protectdocumentonlineresponse) **ProtectDocumentOnline**([ProtectDocumentOnlineRequest](/words/spec/documentprotection#protectdocumentonlinerequest) *request*) - adds protection to the document.
- [RevisionsModificationResponse](/words/spec/documentrevision#revisionsmodificationresponse) **RejectAllRevisions**([RejectAllRevisionsRequest](/words/spec/documentrevision#rejectallrevisionsrequest) *request*) - rejects all revisions in the document.
- [RejectAllRevisionsOnlineResponse](/words/spec/documentrevision#rejectallrevisionsonlineresponse) **RejectAllRevisionsOnline**([RejectAllRevisionsOnlineRequest](/words/spec/documentrevision#rejectallrevisionsonlinerequest) *request*) - rejects all revisions in the document.
- [DocumentResponse](/words/spec/document#documentresponse) **RemoveRange**([RemoveRangeRequest](/words/spec/range#removerangerequest) *request*) - removes a range from the document.
- [RemoveRangeOnlineResponse](/words/spec/range#removerangeonlineresponse) **RemoveRangeOnline**([RemoveRangeOnlineRequest](/words/spec/range#removerangeonlinerequest) *request*) - removes a range from the document.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderDrawingObject**([RenderDrawingObjectRequest](/words/spec/drawingobject#renderdrawingobjectrequest) *request*) - renders a DrawingObject to the specified format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderDrawingObjectOnline**([RenderDrawingObjectOnlineRequest](/words/spec/drawingobject#renderdrawingobjectonlinerequest) *request*) - renders a DrawingObject to the specified format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderMathObject**([RenderMathObjectRequest](/words/spec/mathobject#rendermathobjectrequest) *request*) - renders an OfficeMath object to the specified format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderMathObjectOnline**([RenderMathObjectOnlineRequest](/words/spec/mathobject#rendermathobjectonlinerequest) *request*) - renders an OfficeMath object to the specified format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderPage**([RenderPageRequest](/words/spec/page#renderpagerequest) *request*) - renders a page to the specified format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderPageOnline**([RenderPageOnlineRequest](/words/spec/page#renderpageonlinerequest) *request*) - renders a page to the specified format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderParagraph**([RenderParagraphRequest](/words/spec/paragraph#renderparagraphrequest) *request*) - renders a paragraph to the specified format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderParagraphOnline**([RenderParagraphOnlineRequest](/words/spec/paragraph#renderparagraphonlinerequest) *request*) - renders a paragraph to the specified format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderTable**([RenderTableRequest](/words/spec/table#rendertablerequest) *request*) - renders a table to the specified format.
- <span style="color:SteelBlue;">System.IO.Stream</span> **RenderTableOnline**([RenderTableOnlineRequest](/words/spec/table#rendertableonlinerequest) *request*) - renders a table to the specified format.
- [ReplaceTextResponse](/words/spec/text#replacetextresponse) **ReplaceText**([ReplaceTextRequest](/words/spec/text#replacetextrequest) *request*) - replaces text in the document.
- [ReplaceTextOnlineResponse](/words/spec/text#replacetextonlineresponse) **ReplaceTextOnline**([ReplaceTextOnlineRequest](/words/spec/text#replacetextonlinerequest) *request*) - replaces text in the document.
- [DocumentResponse](/words/spec/document#documentresponse) **ReplaceWithText**([ReplaceWithTextRequest](/words/spec/text#replacewithtextrequest) *request*) - replaces a range with text in the document.
- [ReplaceWithTextOnlineResponse](/words/spec/text#replacewithtextonlineresponse) **ReplaceWithTextOnline**([ReplaceWithTextOnlineRequest](/words/spec/text#replacewithtextonlinerequest) *request*) - replaces a range with text in the document.
- <span style="color:SteelBlue;">Task</span> **ResetCache**([ResetCacheRequest](/words/spec/font#resetcacherequest) *request*) - clears the font cache.
- [SaveResponse](/words/spec/document#saveresponse) **SaveAs**([SaveAsRequest](/words/spec/document#saveasrequest) *request*) - converts a document in cloud storage to the specified format.
- [SaveAsOnlineResponse](/words/spec/document#saveasonlineresponse) **SaveAsOnline**([SaveAsOnlineRequest](/words/spec/document#saveasonlinerequest) *request*) - converts a document to the specified format.
- [DocumentResponse](/words/spec/document#documentresponse) **SaveAsRange**([SaveAsRangeRequest](/words/spec/document#saveasrangerequest) *request*) - saves a range as a new document.
- [SaveAsRangeOnlineResponse](/words/spec/document#saveasrangeonlineresponse) **SaveAsRangeOnline**([SaveAsRangeOnlineRequest](/words/spec/document#saveasrangeonlinerequest) *request*) - saves a range as a new document.
- [SaveResponse](/words/spec/document#saveresponse) **SaveAsTiff**([SaveAsTiffRequest](/words/spec/document#saveastiffrequest) *request*) - converts a document in cloud storage to TIFF format using detailed conversion settings.
- [SaveAsTiffOnlineResponse](/words/spec/document#saveastiffonlineresponse) **SaveAsTiffOnline**([SaveAsTiffOnlineRequest](/words/spec/document#saveastiffonlinerequest) *request*) - converts a document to TIFF format using detailed conversion settings.
- [SearchResponse](/words/spec/text#searchresponse) **Search**([SearchRequest](/words/spec/text#searchrequest) *request*) - searches text, specified by the regular expression, in the document.
- [SearchResponse](/words/spec/text#searchresponse) **SearchOnline**([SearchOnlineRequest](/words/spec/text#searchonlinerequest) *request*) - searches text, specified by the regular expression, in the document.
- [SplitDocumentResponse](/words/spec/document#splitdocumentresponse) **SplitDocument**([SplitDocumentRequest](/words/spec/document#splitdocumentrequest) *request*) - splits a document into parts and saves them in the specified format.
- [SplitDocumentOnlineResponse](/words/spec/document#splitdocumentonlineresponse) **SplitDocumentOnline**([SplitDocumentOnlineRequest](/words/spec/document#splitdocumentonlinerequest) *request*) - splits a document into parts and saves them in the specified format.
- [ProtectionDataResponse](/words/spec/documentprotection#protectiondataresponse) **UnprotectDocument**([UnprotectDocumentRequest](/words/spec/documentprotection#unprotectdocumentrequest) *request*) - removes protection from the document.
- [UnprotectDocumentOnlineResponse](/words/spec/documentprotection#unprotectdocumentonlineresponse) **UnprotectDocumentOnline**([UnprotectDocumentOnlineRequest](/words/spec/documentprotection#unprotectdocumentonlinerequest) *request*) - removes protection from the document.
- [BookmarkResponse](/words/spec/bookmark#bookmarkresponse) **UpdateBookmark**([UpdateBookmarkRequest](/words/spec/bookmark#updatebookmarkrequest) *request*) - updates a bookmark in the document.
- [UpdateBookmarkOnlineResponse](/words/spec/bookmark#updatebookmarkonlineresponse) **UpdateBookmarkOnline**([UpdateBookmarkOnlineRequest](/words/spec/bookmark#updatebookmarkonlinerequest) *request*) - updates a bookmark in the document.
- [BorderResponse](/words/spec/border#borderresponse) **UpdateBorder**([UpdateBorderRequest](/words/spec/border#updateborderrequest) *request*) - the 'nodePath' parameter should refer to a paragraph, a cell or a row.
- [UpdateBorderOnlineResponse](/words/spec/border#updateborderonlineresponse) **UpdateBorderOnline**([UpdateBorderOnlineRequest](/words/spec/border#updateborderonlinerequest) *request*) - updates a border in the document node.
- [CommentResponse](/words/spec/comment#commentresponse) **UpdateComment**([UpdateCommentRequest](/words/spec/comment#updatecommentrequest) *request*) - updates a comment in the document.
- [UpdateCommentOnlineResponse](/words/spec/comment#updatecommentonlineresponse) **UpdateCommentOnline**([UpdateCommentOnlineRequest](/words/spec/comment#updatecommentonlinerequest) *request*) - updates a comment in the document.
- [CustomXmlPartResponse](/words/spec/customxmlpart#customxmlpartresponse) **UpdateCustomXmlPart**([UpdateCustomXmlPartRequest](/words/spec/customxmlpart#updatecustomxmlpartrequest) *request*) - updates the custom xml part in the document.
- [UpdateCustomXmlPartOnlineResponse](/words/spec/customxmlpart#updatecustomxmlpartonlineresponse) **UpdateCustomXmlPartOnline**([UpdateCustomXmlPartOnlineRequest](/words/spec/customxmlpart#updatecustomxmlpartonlinerequest) *request*) - updates the custom xml part in the document.
- [DrawingObjectResponse](/words/spec/drawingobject#drawingobjectresponse) **UpdateDrawingObject**([UpdateDrawingObjectRequest](/words/spec/drawingobject#updatedrawingobjectrequest) *request*) - updates a DrawingObject in the document node.
- [UpdateDrawingObjectOnlineResponse](/words/spec/drawingobject#updatedrawingobjectonlineresponse) **UpdateDrawingObjectOnline**([UpdateDrawingObjectOnlineRequest](/words/spec/drawingobject#updatedrawingobjectonlinerequest) *request*) - updates a DrawingObject in the document node.
- [FieldResponse](/words/spec/field#fieldresponse) **UpdateField**([UpdateFieldRequest](/words/spec/field#updatefieldrequest) *request*) - updates a field in the document node.
- [UpdateFieldOnlineResponse](/words/spec/field#updatefieldonlineresponse) **UpdateFieldOnline**([UpdateFieldOnlineRequest](/words/spec/field#updatefieldonlinerequest) *request*) - updates a field in the document node.
- [DocumentResponse](/words/spec/document#documentresponse) **UpdateFields**([UpdateFieldsRequest](/words/spec/field#updatefieldsrequest) *request*) - reevaluates field values in the document.
- [UpdateFieldsOnlineResponse](/words/spec/field#updatefieldsonlineresponse) **UpdateFieldsOnline**([UpdateFieldsOnlineRequest](/words/spec/field#updatefieldsonlinerequest) *request*) - reevaluates field values in the document.
- [FootnoteResponse](/words/spec/footnote#footnoteresponse) **UpdateFootnote**([UpdateFootnoteRequest](/words/spec/footnote#updatefootnoterequest) *request*) - updates a footnote in the document node.
- [UpdateFootnoteOnlineResponse](/words/spec/footnote#updatefootnoteonlineresponse) **UpdateFootnoteOnline**([UpdateFootnoteOnlineRequest](/words/spec/footnote#updatefootnoteonlinerequest) *request*) - updates a footnote in the document node.
- [FormFieldResponse](/words/spec/formfield#formfieldresponse) **UpdateFormField**([UpdateFormFieldRequest](/words/spec/formfield#updateformfieldrequest) *request*) - updates a form field in the document node.
- [UpdateFormFieldOnlineResponse](/words/spec/formfield#updateformfieldonlineresponse) **UpdateFormFieldOnline**([UpdateFormFieldOnlineRequest](/words/spec/formfield#updateformfieldonlinerequest) *request*) - updates a form field in the document node.
- [ListResponse](/words/spec/list#listresponse) **UpdateList**([UpdateListRequest](/words/spec/list#updatelistrequest) *request*) - updates a list in the document.
- [ListResponse](/words/spec/list#listresponse) **UpdateListLevel**([UpdateListLevelRequest](/words/spec/list#updatelistlevelrequest) *request*) - updates the level of a List element in the document.
- [UpdateListLevelOnlineResponse](/words/spec/list#updatelistlevelonlineresponse) **UpdateListLevelOnline**([UpdateListLevelOnlineRequest](/words/spec/list#updatelistlevelonlinerequest) *request*) - updates the level of a List element in the document.
- [UpdateListOnlineResponse](/words/spec/list#updatelistonlineresponse) **UpdateListOnline**([UpdateListOnlineRequest](/words/spec/list#updatelistonlinerequest) *request*) - updates a list in the document.
- [ParagraphFormatResponse](/words/spec/paragraphformat#paragraphformatresponse) **UpdateParagraphFormat**([UpdateParagraphFormatRequest](/words/spec/paragraphformat#updateparagraphformatrequest) *request*) - updates the formatting properties of a paragraph in the document node.
- [UpdateParagraphFormatOnlineResponse](/words/spec/paragraphformat#updateparagraphformatonlineresponse) **UpdateParagraphFormatOnline**([UpdateParagraphFormatOnlineRequest](/words/spec/paragraphformat#updateparagraphformatonlinerequest) *request*) - updates the formatting properties of a paragraph in the document node.
- [ParagraphListFormatResponse](/words/spec/paragraphlist#paragraphlistformatresponse) **UpdateParagraphListFormat**([UpdateParagraphListFormatRequest](/words/spec/paragraphlist#updateparagraphlistformatrequest) *request*) - updates the formatting properties of a paragraph list in the document node.
- [UpdateParagraphListFormatOnlineResponse](/words/spec/paragraphlist#updateparagraphlistformatonlineresponse) **UpdateParagraphListFormatOnline**([UpdateParagraphListFormatOnlineRequest](/words/spec/paragraphlist#updateparagraphlistformatonlinerequest) *request*) - updates the formatting properties of a paragraph list in the document node.
- [RunResponse](/words/spec/run#runresponse) **UpdateRun**([UpdateRunRequest](/words/spec/run#updaterunrequest) *request*) - updates a Run object in the paragraph.
- [FontResponse](/words/spec/run#fontresponse) **UpdateRunFont**([UpdateRunFontRequest](/words/spec/run#updaterunfontrequest) *request*) - updates the font properties of a Run object in the paragraph.
- [UpdateRunFontOnlineResponse](/words/spec/run#updaterunfontonlineresponse) **UpdateRunFontOnline**([UpdateRunFontOnlineRequest](/words/spec/run#updaterunfontonlinerequest) *request*) - updates the font properties of a Run object in the paragraph.
- [UpdateRunOnlineResponse](/words/spec/run#updaterunonlineresponse) **UpdateRunOnline**([UpdateRunOnlineRequest](/words/spec/run#updaterunonlinerequest) *request*) - updates a Run object in the paragraph.
- [SectionPageSetupResponse](/words/spec/section#sectionpagesetupresponse) **UpdateSectionPageSetup**([UpdateSectionPageSetupRequest](/words/spec/section#updatesectionpagesetuprequest) *request*) - updates the page setup of a section in the document.
- [UpdateSectionPageSetupOnlineResponse](/words/spec/section#updatesectionpagesetuponlineresponse) **UpdateSectionPageSetupOnline**([UpdateSectionPageSetupOnlineRequest](/words/spec/section#updatesectionpagesetuponlinerequest) *request*) - updates the page setup of a section in the document.
- [StyleResponse](/words/spec/style#styleresponse) **UpdateStyle**([UpdateStyleRequest](/words/spec/style#updatestylerequest) *request*) - updates a style in the document.
- [UpdateStyleOnlineResponse](/words/spec/style#updatestyleonlineresponse) **UpdateStyleOnline**([UpdateStyleOnlineRequest](/words/spec/style#updatestyleonlinerequest) *request*) - updates a style in the document.
- [TableCellFormatResponse](/words/spec/tablecell#tablecellformatresponse) **UpdateTableCellFormat**([UpdateTableCellFormatRequest](/words/spec/tablecell#updatetablecellformatrequest) *request*) - updates the formatting properties of a cell in the table row.
- [UpdateTableCellFormatOnlineResponse](/words/spec/tablecell#updatetablecellformatonlineresponse) **UpdateTableCellFormatOnline**([UpdateTableCellFormatOnlineRequest](/words/spec/tablecell#updatetablecellformatonlinerequest) *request*) - updates the formatting properties of a cell in the table row.
- [TablePropertiesResponse](/words/spec/tableproperties#tablepropertiesresponse) **UpdateTableProperties**([UpdateTablePropertiesRequest](/words/spec/tableproperties#updatetablepropertiesrequest) *request*) - updates properties of a table in the document node.
- [UpdateTablePropertiesOnlineResponse](/words/spec/tableproperties#updatetablepropertiesonlineresponse) **UpdateTablePropertiesOnline**([UpdateTablePropertiesOnlineRequest](/words/spec/tableproperties#updatetablepropertiesonlinerequest) *request*) - updates properties of a table in the document node.
- [TableRowFormatResponse](/words/spec/tablerow#tablerowformatresponse) **UpdateTableRowFormat**([UpdateTableRowFormatRequest](/words/spec/tablerow#updatetablerowformatrequest) *request*) - updates the formatting properties of a table row.
- [UpdateTableRowFormatOnlineResponse](/words/spec/tablerow#updatetablerowformatonlineresponse) **UpdateTableRowFormatOnline**([UpdateTableRowFormatOnlineRequest](/words/spec/tablerow#updatetablerowformatonlinerequest) *request*) - updates the formatting properties of a table row.
- [FilesUploadResult](/words/spec/file#filesuploadresult) **UploadFile**([UploadFileRequest](/words/spec/file#uploadfilerequest) *request*) - upload file.


## AuthType

This class is used in [Configuration](#configuration).

The following values are defined: OAuth2, RequestSignature.

