---
title: "Aspose.Words Cloud 20.5 Release Notes"
type: docs
url: /aspose-words-cloud-20-5-release-notes/
weight: 40
---

{{% alert color="primary" %}} 

The page contains release notes for Aspose.Words Cloud 20.5 – [API Reference](https://apireference.aspose.cloud/words/)

{{% /alert %}} 
## **Important Changes and Enhancements**
### **Words Cloud changes**
1. Added "BuildReport" feature (uses [Linq reporting](https://docs.aspose.com/display/wordsnet/LINQ+Reporting+Engine+API))
1. Added support of "Document.Lists"
1. Added support of "Paragraph.ListFormat"
1. Added support of "Document.Styles"
1. Added support of change "Style" for document elements
1. Added support of "ParagraphFormat.Shading" and "ParagraphFormat.Tabstops"
1. Added support of UrlEncoded "NodePath" parameters
1. Released "Downloadable" version of API on DockerHub
### **PDF to Word conversion improvements**
1. Fixed letters disappearance during PDF recognition;
1. Implemented diagonal lines detection in tables;
1. Improved space detection between words;
1. Solved several problems with landscape page recognition.
## **All changes**

|#|Summary|Category|
| :- | :- | :- |
|WORDSCLOUD-699|Support of Text Style attributes|Feature|
|WORDSCLOUD-717|Downloadable docker version of API|Feature|
|WORDSCLOUD-786|Support to update document style|Feature|
|WORDSCLOUD-808|Add multilevel Bullet List in Word Documente|Feature|
|WORDSCLOUD-846|Support Document.Lists functionality|Feature|
|WORDSCLOUD-847|Support Paragraph.ListFormat functionality|Feature|
|WORDSCLOUD-942|Add support of ParagraphFormat properties|Feature|
|WORDSCLOUD-957|Add linq reporting support|Feature|
|WORDSCLOUD-941|Word to HTML, placeholder breaks into spans|Bug|
|WORDSCLOUD-1136|GetParagraph API parameter is encoded in API Explorer|Bug|
|WORDSCLOUD-1137|GetParagraphFormat API parameter is encoded in API Explorer|Bug|
|PDF2WORD-73 |Sometimes letters "fi" disappear in the word "Definition" |Bug|
|PDF2WORD-320 |Diagonal lines in tables aren't recognized |Bug|
|PDF2WORD-368 |Corrupted PDF error during recognition |Bug|
|PDF2WORD-417 |Underlined text does not recognized correctly |Bug|
|PDF2WORD-426 |Simple segments tests fail on Linux|Bug|
|PDF2WORD-427 |TestRecognizingHyperlinks fails on Linux |Bug|
|PDF2WORD-483 |Incorrect processing of pages with landscape orientation |Bug|
|PDF2WORD-491 |Pdf2Word doesn't work for some Aspose.Words customers on .NET Framework 4.6.1 |Bug|
|PDF2WORD-492 |Aspose.Words tries to load old Pdf2Word version 20.02 instead of latest 20.04 |Bug|
|PDF2WORD-497 |Why do we have netstandard2 facade reference in .NET 4.6.1 release build? |Bug|
|PDF2WORD-294 |Add Accuracy tests to build verification on GitLab (except the slowest one) |Task|
## **SDK Changes**
### **Aspose Words Cloud .Net SDK 20.5**
1. Added methods to work with Word document lists
   1. GetLists
   1. GetList
   1. InsertList
   1. UpdateList
   1. UpdateListLevel
1. Added methods to work with styles
   1. GetStyles
   1. UpdateStyle
   1. InsertStyle
   1. CopyStyle
   1. GetStyleFromDocumentElement
   1. ApplyStyleToDocumentElement
1. Added methods to work with paragraph list format
   1. GetParagraphListFormat
   1. GetParagraphListFormatWithoutNodePath
   1. UpdateParagraphListFormat
   1. DeleteParagraphListFormat
1. Added methods to work with paragraph tab stops
   1. GetParagraphTabStops
   1. InsertOrUpdateParagraphTabStop
   1. DeleteAllParagraphTabStops
   1. DeleteParagraphTabStop
1. Added methods to build reports
   1. BuildReport
   1. BuildReportOnline
1. Added Shading property to ParagraphFormat
### **Aspose Words Cloud C++ SDK 20.5**
1. Added methods to work with Word document lists
   1. getLists
   1. getList
   1. insertList
   1. updateList
   1. updateListLevel
1. Added methods to work with styles
   1. getStyles
   1. updateStyle
   1. insertStyle
   1. copyStyle
   1. getStyleFromDocumentElement
   1. applyStyleToDocumentElement
1. Added methods to work with paragraph list format
   1. getParagraphListFormat
   1. getParagraphListFormatWithoutNodePath
   1. updateParagraphListFormat
   1. deleteParagraphListFormat
1. Added methods to work with paragraph tab stops
   1. getParagraphTabStops
   1. insertOrUpdateParagraphTabStop
   1. deleteAllParagraphTabStops
   1. deleteParagraphTabStop
1. Added methods to build reports
   1. buildReport
   1. buildReportOnline
1. Added Shading property to ParagraphFormat
### **Aspose Words Cloud Go SDK 20.5**
1. Added methods to work with Word document lists
   1. GetLists
   1. GetList
   1. InsertList
   1. UpdateList
   1. UpdateListLevel
1. Added methods to work with styles
   1. GetStyles
   1. UpdateStyle
   1. InsertStyle
   1. CopyStyle
   1. GetStyleFromDocumentElement
   1. ApplyStyleToDocumentElement
1. Added methods to work with paragraph list format
   1. GetParagraphListFormat
   1. GetParagraphListFormatWithoutNodePath
   1. UpdateParagraphListFormat
   1. DeleteParagraphListFormat
1. Added methods to work with paragraph tab stops
   1. GetParagraphTabStops
   1. InsertOrUpdateParagraphTabStop
   1. DeleteAllParagraphTabStops
   1. DeleteParagraphTabStop
1. Added methods to build reports
   1. BuildReport
   1. BuildReportOnline
1. Added Shading property to ParagraphFormat
### **Aspose Words Cloud Java SDK 20.5**
1. Added methods to work with Word document lists
   1. GetLists
   1. GetList
   1. InsertList
   1. UpdateList
   1. UpdateListLevel
1. Added methods to work with styles
   1. GetStyles
   1. UpdateStyle
   1. InsertStyle
   1. CopyStyle
   1. GetStyleFromDocumentElement
   1. ApplyStyleToDocumentElement
1. Added methods to work with paragraph list format
   1. GetParagraphListFormat
   1. GetParagraphListFormatWithoutNodePath
   1. UpdateParagraphListFormat
   1. DeleteParagraphListFormat
1. Added methods to work with paragraph tab stops
   1. GetParagraphTabStops
   1. InsertOrUpdateParagraphTabStop
   1. DeleteAllParagraphTabStops
   1. DeleteParagraphTabStop
1. Added methods to build reports
   1. BuildReport
   1. BuildReportOnline
1. Added Shading property to ParagraphFormat
### ` `**Aspose Words Cloud Node.js SDK 20.5**
1. Added methods to work with Word document lists
   1. getLists
   1. getList
   1. insertList
   1. updateList
   1. updateListLevel
1. Added methods to work with styles
   1. getStyles
   1. updateStyle
   1. insertStyle
   1. copyStyle
   1. getStyleFromDocumentElement
   1. applyStyleToDocumentElement
1. Added methods to work with paragraph list format
   1. getParagraphListFormat
   1. getParagraphListFormatWithoutNodePath
   1. updateParagraphListFormat
   1. deleteParagraphListFormat
1. Added methods to work with paragraph tab stops
   1. getParagraphTabStops
   1. insertOrUpdateParagraphTabStop
   1. deleteAllParagraphTabStops
   1. deleteParagraphTabStop
1. Added methods to build reports
   1. buildReport
   1. buildReportOnline
1. Added Shading property to ParagraphFormat
### **Aspose Words Cloud PHP SDK 20.5**
1. Added methods to work with Word document lists
   1. GetLists
   1. GetList
   1. InsertList
   1. UpdateList
   1. UpdateListLevel
1. Added methods to work with styles
   1. GetStyles
   1. UpdateStyle
   1. InsertStyle
   1. CopyStyle
   1. GetStyleFromDocumentElement
   1. ApplyStyleToDocumentElement
1. Added methods to work with paragraph list format
   1. GetParagraphListFormat
   1. GetParagraphListFormatWithoutNodePath
   1. UpdateParagraphListFormat
   1. DeleteParagraphListFormat
1. Added methods to work with paragraph tab stops
   1. GetParagraphTabStops
   1. InsertOrUpdateParagraphTabStop
   1. DeleteAllParagraphTabStops
   1. DeleteParagraphTabStop
1. Added methods to build reports
   1. BuildReport
   1. BuildReportOnline
1. Added Shading property to ParagraphFormat
### **Aspose Words Cloud Python SDK 20.5**
1. Added methods to work with Word document lists
   1. GetLists
   1. GetList
   1. InsertList
   1. UpdateList
   1. UpdateListLevel
1. Added methods to work with styles
   1. GetStyles
   1. UpdateStyle
   1. InsertStyle
   1. CopyStyle
   1. GetStyleFromDocumentElement
   1. ApplyStyleToDocumentElement
1. Added methods to work with paragraph list format
   1. GetParagraphListFormat
   1. GetParagraphListFormatWithoutNodePath
   1. UpdateParagraphListFormat
   1. DeleteParagraphListFormat
1. Added methods to work with paragraph tab stops
   1. GetParagraphTabStops
   1. InsertOrUpdateParagraphTabStop
   1. DeleteAllParagraphTabStops
   1. DeleteParagraphTabStop
1. Added methods to build reports
   1. BuildReport
   1. BuildReportOnline
1. Added Shading property to ParagraphFormat
### **Aspose Words Cloud Ruby SDK 20.5**
1. Added methods to work with Word document lists
   1. GetLists
   1. GetList
   1. InsertList
   1. UpdateList
   1. UpdateListLevel
1. Added methods to work with styles
   1. GetStyles
   1. UpdateStyle
   1. InsertStyle
   1. CopyStyle
   1. GetStyleFromDocumentElement
   1. ApplyStyleToDocumentElement
1. Added methods to work with paragraph list format
   1. GetParagraphListFormat
   1. GetParagraphListFormatWithoutNodePath
   1. UpdateParagraphListFormat
   1. DeleteParagraphListFormat
1. Added methods to work with paragraph tab stops
   1. GetParagraphTabStops
   1. InsertOrUpdateParagraphTabStop
   1. DeleteAllParagraphTabStops
   1. DeleteParagraphTabStop
1. Added methods to build reports
   1. BuildReport
   1. BuildReportOnline
1. Added Shading property to ParagraphFormat
### **Aspose Words Cloud Swift SDK 20.5**
1. Added methods to work with Word document lists
   1. GetLists
   1. GetList
   1. InsertList
   1. UpdateList
   1. UpdateListLevel
1. Added methods to work with styles
   1. GetStyles
   1. UpdateStyle
   1. InsertStyle
   1. CopyStyle
   1. GetStyleFromDocumentElement
   1. ApplyStyleToDocumentElement
1. Added methods to work with paragraph list format
   1. GetParagraphListFormat
   1. GetParagraphListFormatWithoutNodePath
   1. UpdateParagraphListFormat
   1. DeleteParagraphListFormat
1. Added methods to work with paragraph tab stops
   1. GetParagraphTabStops
   1. InsertOrUpdateParagraphTabStop
   1. DeleteAllParagraphTabStops
   1. DeleteParagraphTabStop
1. Added methods to build reports
   1. BuildReport
   1. BuildReportOnline
1. Added Shading property to ParagraphFormat
