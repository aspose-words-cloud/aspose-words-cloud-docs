---
title: "Aspose.Words Cloud 20.5 Release Notes"
type: docs
url: /release-notes/2020/20-5/
aliases: [/aspose-words-cloud-20-5-release-notes/]
weight: 40
---

The page contains release notes for Aspose.Words Cloud 20.5 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and Enhancements

## Words

1. Added "BuildReport" feature (uses [Linq reporting](https://docs.aspose.com/display/wordsnet/LINQ+Reporting+Engine+API)).
2. Added support of "Document.Lists"
3. Added support of "Paragraph.ListFormat"
4. Added support of "Document.Styles"
5. Added support of change "Style" for document elements
6. Added support of "ParagraphFormat.Shading" and "ParagraphFormat.Tabstops"
7. Added support of UrlEncoded "NodePath" parameters
8. Released "Downloadable" version of API on DockerHub

## PDF

1. Fixed letters disappearance during PDF recognition;
2. Implemented diagonal lines detection in tables;
3. Improved space detection between words;
4. Solved several problems with landscape page recognition.

## All changes

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

## SDK Changes

## Aspose

1. Added methods to work with Word document lists
   - GetLists
   - GetList
   - InsertList
   - UpdateList
   - UpdateListLevel
2. Added methods to work with styles
   - GetStyles
   - UpdateStyle
   - InsertStyle
   - CopyStyle
   - GetStyleFromDocumentElement
   - ApplyStyleToDocumentElement
3. Added methods to work with paragraph list format
   - GetParagraphListFormat
   - GetParagraphListFormatWithoutNodePath
   - UpdateParagraphListFormat
   - DeleteParagraphListFormat
4. Added methods to work with paragraph tab stops
   - GetParagraphTabStops
   - InsertOrUpdateParagraphTabStop
   - DeleteAllParagraphTabStops
   - DeleteParagraphTabStop
5. Added methods to build reports
   - BuildReport
   - BuildReportOnline
6. Added Shading property to ParagraphFormat

## Aspose

1. Added methods to work with Word document lists
   - getLists
   - getList
   - insertList
   - updateList
   - updateListLevel
2. Added methods to work with styles
   - getStyles
   - updateStyle
   - insertStyle
   - copyStyle
   - getStyleFromDocumentElement
   - applyStyleToDocumentElement
3. Added methods to work with paragraph list format
   - getParagraphListFormat
   - getParagraphListFormatWithoutNodePath
   - updateParagraphListFormat
   - deleteParagraphListFormat
4. Added methods to work with paragraph tab stops
   - getParagraphTabStops
   - insertOrUpdateParagraphTabStop
   - deleteAllParagraphTabStops
   - deleteParagraphTabStop
5. Added methods to build reports
   - buildReport
   - buildReportOnline
6. Added Shading property to ParagraphFormat

## Aspose

1. Added methods to work with Word document lists
   - GetLists
   - GetList
   - InsertList
   - UpdateList
   - UpdateListLevel
2. Added methods to work with styles
   - GetStyles
   - UpdateStyle
   - InsertStyle
   - CopyStyle
   - GetStyleFromDocumentElement
   - ApplyStyleToDocumentElement
3. Added methods to work with paragraph list format
   - GetParagraphListFormat
   - GetParagraphListFormatWithoutNodePath
   - UpdateParagraphListFormat
   - DeleteParagraphListFormat
4. Added methods to work with paragraph tab stops
   - GetParagraphTabStops
   - InsertOrUpdateParagraphTabStop
   - DeleteAllParagraphTabStops
   - DeleteParagraphTabStop
5. Added methods to build reports
   - BuildReport
   - BuildReportOnline
6. Added Shading property to ParagraphFormat

## Aspose

1. Added methods to work with Word document lists
   - GetLists
   - GetList
   - InsertList
   - UpdateList
   - UpdateListLevel
2. Added methods to work with styles
   - GetStyles
   - UpdateStyle
   - InsertStyle
   - CopyStyle
   - GetStyleFromDocumentElement
   - ApplyStyleToDocumentElement
3. Added methods to work with paragraph list format
   - GetParagraphListFormat
   - GetParagraphListFormatWithoutNodePath
   - UpdateParagraphListFormat
   - DeleteParagraphListFormat
4. Added methods to work with paragraph tab stops
   - GetParagraphTabStops
   - InsertOrUpdateParagraphTabStop
   - DeleteAllParagraphTabStops
   - DeleteParagraphTabStop
5. Added methods to build reports
   - BuildReport
   - BuildReportOnline
6. Added Shading property to ParagraphFormat

## ` `Aspose

1. Added methods to work with Word document lists
   - getLists
   - getList
   - insertList
   - updateList
   - updateListLevel
2. Added methods to work with styles
   - getStyles
   - updateStyle
   - insertStyle
   - copyStyle
   - getStyleFromDocumentElement
   - applyStyleToDocumentElement
3. Added methods to work with paragraph list format
   - getParagraphListFormat
   - getParagraphListFormatWithoutNodePath
   - updateParagraphListFormat
   - deleteParagraphListFormat
4. Added methods to work with paragraph tab stops
   - getParagraphTabStops
   - insertOrUpdateParagraphTabStop
   - deleteAllParagraphTabStops
   - deleteParagraphTabStop
5. Added methods to build reports
   - buildReport
   - buildReportOnline
6. Added Shading property to ParagraphFormat

## Aspose

1. Added methods to work with Word document lists
   - GetLists
   - GetList
   - InsertList
   - UpdateList
   - UpdateListLevel
2. Added methods to work with styles
   - GetStyles
   - UpdateStyle
   - InsertStyle
   - CopyStyle
   - GetStyleFromDocumentElement
   - ApplyStyleToDocumentElement
3. Added methods to work with paragraph list format
   - GetParagraphListFormat
   - GetParagraphListFormatWithoutNodePath
   - UpdateParagraphListFormat
   - DeleteParagraphListFormat
4. Added methods to work with paragraph tab stops
   - GetParagraphTabStops
   - InsertOrUpdateParagraphTabStop
   - DeleteAllParagraphTabStops
   - DeleteParagraphTabStop
5. Added methods to build reports
   - BuildReport
   - BuildReportOnline
6. Added Shading property to ParagraphFormat

## Aspose

1. Added methods to work with Word document lists
   - GetLists
   - GetList
   - InsertList
   - UpdateList
   - UpdateListLevel
2. Added methods to work with styles
   - GetStyles
   - UpdateStyle
   - InsertStyle
   - CopyStyle
   - GetStyleFromDocumentElement
   - ApplyStyleToDocumentElement
3. Added methods to work with paragraph list format
   - GetParagraphListFormat
   - GetParagraphListFormatWithoutNodePath
   - UpdateParagraphListFormat
   - DeleteParagraphListFormat
4. Added methods to work with paragraph tab stops
   - GetParagraphTabStops
   - InsertOrUpdateParagraphTabStop
   - DeleteAllParagraphTabStops
   - DeleteParagraphTabStop
5. Added methods to build reports
   - BuildReport
   - BuildReportOnline
6. Added Shading property to ParagraphFormat

## Aspose

1. Added methods to work with Word document lists
   - GetLists
   - GetList
   - InsertList
   - UpdateList
   - UpdateListLevel
2. Added methods to work with styles
   - GetStyles
   - UpdateStyle
   - InsertStyle
   - CopyStyle
   - GetStyleFromDocumentElement
   - ApplyStyleToDocumentElement
3. Added methods to work with paragraph list format
   - GetParagraphListFormat
   - GetParagraphListFormatWithoutNodePath
   - UpdateParagraphListFormat
   - DeleteParagraphListFormat
4. Added methods to work with paragraph tab stops
   - GetParagraphTabStops
   - InsertOrUpdateParagraphTabStop
   - DeleteAllParagraphTabStops
   - DeleteParagraphTabStop
5. Added methods to build reports
   - BuildReport
   - BuildReportOnline
6. Added Shading property to ParagraphFormat

## Aspose

1. Added methods to work with Word document lists
   - GetLists
   - GetList
   - InsertList
   - UpdateList
   - UpdateListLevel
2. Added methods to work with styles
   - GetStyles
   - UpdateStyle
   - InsertStyle
   - CopyStyle
   - GetStyleFromDocumentElement
   - ApplyStyleToDocumentElement
3. Added methods to work with paragraph list format
   - GetParagraphListFormat
   - GetParagraphListFormatWithoutNodePath
   - UpdateParagraphListFormat
   - DeleteParagraphListFormat
4. Added methods to work with paragraph tab stops
   - GetParagraphTabStops
   - InsertOrUpdateParagraphTabStop
   - DeleteAllParagraphTabStops
   - DeleteParagraphTabStop
5. Added methods to build reports
   - BuildReport
   - BuildReportOnline
6. Added Shading property to ParagraphFormat
