---
title: "20.6 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2020/20-6/
aliases: [/aspose-words-cloud-20-6-release-notes/]
description: "Aspose Words Cloud 20.6 Release Notes"
weight: 30
---

The page contains release notes for Aspose.Words Cloud 20.6 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words

1. Added OoxmlSaveOption CompressionLevel property
2. Added group of methods without nodePath property
   - DeleteAllParagraphTabStops
   - DeleteParagraphListFormat
   - DeleteParagraphTabStop
   - GetParagraphTabStops
   - InsertOrUpdateParagraphTabStop
   - InsertParagraph
   - UpdateParagraphFormat
   - UpdateParagraphListFormat
3. In methods InsertOrUpdateParagraphTabStop, DeleteParagraphTabStop order of parameters has changed NodePath was moved to one position next, like if it was second before, now it's
4. Fixed swagger specification for "insert drawing object" and "update drawing object" methods

## PDF

- Implemented clipping path detection for W and W\* operators
- Added support for PDF files with early EOFs
- Slightly improved speed of PDF recognition workflow
- Corrected space detection between links on the same row
- Fixed a rare concurrency error in font loading code

## All changes

|ID|Summary|Category|
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

## API

1. Added new methods:
   - deleteAllParagraphTabStopsWithoutNodePath
   - deleteParagraphTabStopWithoutNodePath
   - getParagraphTabStopsWithoutNodePath
   - insertOrUpdateParagraphTabStopWithoutNodePath
   - insertParagraphWithoutNodePath
   - updateParagraphFormatWithoutNodePath
   - updateParagraphListFormatWithoutNodePath
   - deleteParagraphListFormatWithoutNodePath
2. DrawingObject related methods have been changed body content. Special request classes are introduced instead of strings.
3. insertOrUpdateParagraphTabStop, deleteParagraphTabStop methods have been changed parameter order
4. OoxmlSaveOptionsData.CompressionLevel property has been added

