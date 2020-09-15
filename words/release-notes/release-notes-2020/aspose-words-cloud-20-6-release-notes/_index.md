---
title: "Aspose.Words Cloud 20.6 Release Notes"
type: docs
url: /aspose-words-cloud-20-6-release-notes/
weight: 30
---

{{% alert color="primary" %}} 

The page contains release notes for Aspose.Words Cloud 20.6 – [API Reference](https://apireference.aspose.cloud/words/)

{{% /alert %}} 
## **Important Changes and New Features**
### **Words Cloud changes**
1. Added OoxmlSaveOption CompressionLevel property
1. Added group of methods without nodePath property
   1. DeleteAllParagraphTabStops
   1. DeleteParagraphListFormat
   1. DeleteParagraphTabStop
   1. GetParagraphTabStops
   1. InsertOrUpdateParagraphTabStop
   1. InsertParagraph
   1. UpdateParagraphFormat
   1. UpdateParagraphListFormat
1. In methods InsertOrUpdateParagraphTabStop, DeleteParagraphTabStop order of parameters has changed NodePath was moved to one position next, like if it was second before, now it's
1. Fixed swagger specification for "insert drawing object" and "update drawing object" methods
### **PDF to Word conversion improvements**
1. Implemented clipping path detection for W and W\* operators
1. Added support for PDF files with early EOFs
1. Slightly improved speed of PDF recognition workflow
1. Corrected space detection between links on the same row
1. Fixed a rare concurrency error in font loading code
## ` `**All changes**

|**ID**|**Summary**|**Category**|
| :- | :- | :- |
|WORDSCLOUD-1183|Add new OoxmlSaveOption CompressionLevel|Feature|
|WORDSCLOUD-1147|Some methods don't have "withoutNodePath" version in swagger UI|Bug|
|WORDSCLOUD-1222|Swagger UI authentication is not working on DockerHub version|Bug|
|PDF2WORD-450 |Links lines must be separated |Bug|
|PDF2WORD-485 |Optimize and enable Colontitle Accuracy test with Full DataSet |Task|
|PDF2WORD-496 |Unify all implementations of accuracy tests |Task |
|PDF2WORD-498 |Investigate how difficult would it be to support arabic writing |Task|
|PDF2WORD-499 |Sometimes PDF conversion fails on Linux |Bug|
|PDF2WORD-500 |Can't open doc-1.pdf because there is no "end of stream" marker |Bug|
|PDF2WORD-501 |Duplicated bottom text line after PDF conversion |Bug|
### **API Changes for Aspose.Words Cloud SDKs (.Net, Java, PHP, Ruby, Node.js, Python, Go and Swift)**
1. Added new methods:
   1. deleteAllParagraphTabStopsWithoutNodePath
   1. deleteParagraphTabStopWithoutNodePath
   1. getParagraphTabStopsWithoutNodePath
   1. insertOrUpdateParagraphTabStopWithoutNodePath
   1. insertParagraphWithoutNodePath
   1. updateParagraphFormatWithoutNodePath
   1. updateParagraphListFormatWithoutNodePath
   1. deleteParagraphListFormatWithoutNodePath
1. DrawingObject related methods have been changed body content. Special request classes are introduced instead of strings.
1. insertOrUpdateParagraphTabStop, deleteParagraphTabStop methods have been changed parameter order
1. OoxmlSaveOptionsData.CompressionLevel property has been added



