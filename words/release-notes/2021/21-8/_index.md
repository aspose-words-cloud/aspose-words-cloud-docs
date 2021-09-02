---
title: "21.8 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-8/
aliases: [/aspose-words-cloud-21-8-release-notes/]
description: "Aspose Words Cloud 21.8 Release Notes"
weight: 35
---

The page contains release notes for Aspose.Words Cloud 21.8 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Implemented several API methods to get, insert, update and delete custom XML parts from documents
- Added a new parameter to the 'Comparison' API (`ResultDocumentFormat`)
- Added a new option for saving PDF files (`ExportLanguageToSpanTag`)
- Added a new option for saving FlatOPC files (`FlatOpcXmlMappingOnly`)

## PDF to Word conversion improvements

- Fixed a `ZlibException` caused by extra spaces in `FlateDecode` PDF streams
- Fixed a `ZlibException` caused by data streams with incorrect checksums (as some PDF software doesn't follow the specification)
- Fixed an `InvalidOperationException` related to PDF filter processing
- Fixed an `InvalidOperationException` appeared as "Operator should take 1 operand" message

## All changes

| #               | Summary                                                                                       | Category    |
|-----------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1655 | Add a new `ResultDocumentFormat` parameter to the 'Comparison' API to specify an output format | New Feature |
| WORDSCLOUD-1691 | Read custom XML parts from Word documents                                                     | New Feature |
| WORDSCLOUD-1697 | Add a new `FlatOpcXmlMappingOnly` option for saving FlatOPC files                             | New Feature |
| WORDSCLOUD-1698 | Add a new `ExportLanguageToSpanTag` exporting option                                          | New Feature |
| WORDSCLOUD-1714 | Declare properties in models as `public`, add support for chains of `set`-methods in the Swift SDK | New Feature |
| WORDSCLOUD-1651 | Check if an 'Internal Server Error' is returned for every error in the Ruby SDK               | Bug      |
| WORDSCLOUD-1660 | The Ruby SDK is expected to generate an exception when comparing documents with multiple revisions | Bug      |
| WORDSCLOUD-1692 | The `DeleteFile` API does not accept a leading forward slash in a file path                   | Bug      |
| WORDSCLOUD-1694 | An error occurs in the LINQ Reporting Engine when handling absent input data (JSON)           | Bug      |
| WORDSCLOUD-1695 | An error occurs in the LINQ Reporting Engine when splitting strings                           | Bug      |
| WORDSCLOUD-1713 | Incorrect DOCX files are returned when calling the 'Comparison' API online-method             | Bug      |
| PDF2WORD-810    | Thin lines are mistakenly processed as separate paragraphs                                    | Bug      |
| PDF2WORD-811    | Incorrect image position                                                                      | Bug      |
| PDF2WORD-817    | `ZlibException`: Bad state (unknown compression method (0x20))                                | Bug      |
| PDF2WORD-821    | `InvalidOperationException`: Operator should take 1 operands                                  | Bug      |
| PDF2WORD-844    | The contents of a page is mistakenly shifted when column detection is enabled                 | Bug      |
| PDF2WORD-847    | `InvalidOperationException`: Filter entry of stream object must be either PDF name or PDF Array | Bug    |
| PDF2WORD-855    | Implement the ability to specify footer distance                                              | Task     |
| PDF2WORD-856    | `ZlibException`: Bad state (incorrect data check)                                             | Bug      |
