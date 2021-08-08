---
title: "21.6 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-6/
aliases: [/aspose-words-cloud-21-6-release-notes/]
description: "Aspose Words Cloud 21.6 Release Notes"
weight: 45
---

The page contains release notes for Aspose.Words Cloud 21.6 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- `CompareDocumentOnline` method can handle two documents for comparison located in a message's body
- `CompareDocument` method can handle PDF files with an output document saved as DOCX
- Added a new `AcceptAllRevisionsBeforeComparison` option which specifies whether to accept all revisions before the comparison

## PDF to Word conversion improvements

- Fixed `OverflowException`: Value was either too large or too small for an Int32
- Fixed `InvalidCastException`: Cannot cast PdfArray to PdfDictionary
- Fixed black page background by supporting custom color settings in path drawing logic
- Fixed `System.FormatException`: Value doesn't follow the Roman number format
- Fixed `InvalidOperationException`: BBox definition is not PDF array
- Fixed `ArgumentException` in `NamedDestinations.ReadDestValue` method
- Fixed `KeyNotFoundException`: Dictionary doesn't contain `Length` entry
- Fixed `NullReferenceException` in `PdfOperatorDo.ProcessImage` method
- Fixed several `IndexOutOfRangeException` in `PdfTokenParser` and other PDF parser components

## All changes

| #               | Summary                                                                                       | Category |
|-----------------|-----------------------------------------------------------------------------------------------|----------|
| WORDSCLOUD-1476 | Provide support for online methods in Go SDK                                                  | Feature  |
| WORDSCLOUD-1573 | Draw a horizontal line at the end of a text line                                              | Feature  |
| WORDSCLOUD-1611 | Append two files from a message's body in `CompareDocumentOnline` method                      | Feature  |
| WORDSCLOUD-1615 | Provide support for comparison of PDF files                                                   | Feature  |
  WORDSCLOUD-767  | Fix an error caused by timeouts                                                                | Bug      |
| WORDSCLOUD-1287 | `SaveAsRange` method is not working for sections                                              | Bug      |
| WORDSCLOUD-1465 | Statistics API throws `NullReferenceException`                                                | Bug      |
| WORDSCLOUD-1482 | GetStatistics API throws "Cannot insert a node of this type at this location" exception       | Bug      |
| WORDSCLOUD-1539 | Online version of `buildReport` method returns a strange error message                        | Bug      |
| WORDSCLOUD-1620 | Requests with query parameters are formed incorrectly in Go SDK                               | Bug      |
| WORDSCLOUD-1641 | Responses should be closed before reading in Go SDK                                           | Bug      |
| WORDSCLOUD-1656 | Issue with saving temporary files in Ruby SDK                                                 | Bug      |
| WORDSCLOUD-1658 | DOCX files are saved incorrectly after the comparison                                         | Bug      |
| WORDSCLOUD-1661 | An error occurres when running PHP SDK inside a Docker container                              | Bug      |
| PDF2WORD-766    | Provide support for multi-columns in DSR classes                                              | Task     |
| PDF2WORD-767    | Provide support for multi-columns in the "Formatted Document Model"                           | Task     |
| PDF2WORD-768    | Set the correct section attributes for `AsposeWordsDocumentBuilder`                           | Task     |
| PDF2WORD-774    | `KeyNotFoundException`: Dictionary doesn't contain `Length` entry                             | Bug      |
| PDF2WORD-776    | `ArgumentOutOfRangeException` is thrown in `BookmarkExtractor.LoadObjects` method             | Bug      |
| PDF2WORD-791    | `InvalidCastException`: Cannot cast `PdfArray` to `PdfDictionary`                             | Bug      |
| PDF2WORD-792    | `ArgumentException` is thrown in `PdfObjectStream.FillNumberToOffsetMap` method               | Bug      |
| PDF2WORD-793    | `OverflowException`: Value was either too large or too small for an Int32                     | Bug      |
| PDF2WORD-794    | `InvalidOperationException`: BBox definition is not PDF array                                 | Bug      |
| PDF2WORD-802    | `ArgumentException` is thrown in `NamedDestinations.ReadDestValue` method                     | Bug      |
| PDF2WORD-803    | A background color is set to black though it should be white                                  | Bug      |
| PDF2WORD-804    | `FormatException`: Value doesn't follow the Roman number format: "k"                          | Bug      |
| PDF2WORD-806    | `NullReferenceException` is thrown in `PdfOperatorDo.ProcessImage` method                     | Bug      |
| PDF2WORD-808    | `IndexOutOfRangeException` is thrown in `PdfTokenParser` and similar components               | Bug      |