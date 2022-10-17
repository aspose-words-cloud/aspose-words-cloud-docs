---
title: "22.10 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2022/22-10/
aliases: [/aspose-words-cloud-22-10-release-notes/]
description: "Aspose Words Cloud 22.10 Release Notes"
weight: 25
---

The page contains release notes for Aspose.Words Cloud 22.10 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Removed the deprecated `FlatOpcXmlMappingOnly` save option
- Added support for `PdfSaveOptions.CacheHeaderFooterShapes` save option
- Implemented the ability to set a custom `StartingNumber` in InsertPageNumbers API
- Added EMF format support for ConvertDocument API
- A new implementation of the `AppendDocumentOnline` method


## PDF to Word conversion improvements

- Improved functionality for detecting strikethrough text
- Fixed several issues with PDF import
- Fixed rare issue with RTL table content


## All changes

| #               | Summary                                                                                              | Category |
|-----------------|------------------------------------------------------------------------------------------------------|----------|
| WORDSCLOUD-1937 | Configure the Aspose.Words Docker Container to listen on a specific port                             | New Feature |
| WORDSCLOUD-2039 | Add support for Danish local number format in Mail Merge                                             | New Feature |
| WORDSCLOUD-2118 | An error occurs while converting DOCX to EMF using ConvertDocument API                               | Bug      |
| WORDSCLOUD-2036 | Implement the ability to send appending documents in the request body using AppendDocumentOnline API | New Feature |
| WORDSCLOUD-2097 | Add support for `PdfSaveOptions.CacheHeaderFooterShapes` property                                    | New Feature |
| WORDSCLOUD-2115 | Implement the ability to set a custom `StartingNumber` for `PageNumbers` in InsertPageNumbers API    | New Feature |
| WORDSNET-24238 | Strikethrough text changes to underlined text when importing PDF                                      | Bug         |
| WORDSNET-24299 | `InvalidOperationException`: incorrect stream content                                                 | Bug         |
| WORDSNET-24300 | `InvalidOperationException`: too big integer value                                                    | Bug         |
| WORDSNET-24358 | Excess spaces appear after importing a table from a PDF with RTL content                              | Bug         |
| WORDSNET-24420 | `CenteredParagraphCorrector` throws `NullReferenceException` when importing PDF                       | Bug         |
