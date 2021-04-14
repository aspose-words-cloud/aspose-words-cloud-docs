---
title: "21.4 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-4/
aliases: [/aspose-words-cloud-21-4-release-notes/]
description: "Aspose Words Cloud 21.4 Release Notes"
weight: 55
---

The page contains release notes for Aspose.Words Cloud 21.4 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Added a new `CustomTimeZoneInfoData` option for saving output files
- Removed an obsolete `EscapeUri` option previously used for PDF file saving
- The URL of a child request in a batch now can be specified with an absolute path. Earlier the path could only be relative
- Added a new 'RequestId' header to all the REST responses

## PDF to Word conversion improvements

- Improved text positioning to avoid unnecessary content shift to the next page
- Added a stub picture for PDF images that can't be decoded
- Fixed the detection logic of table rows in a PDF
- Fixed duplicate coordinates processing when a PDF has many small elements
- Fixes an object cast error from type `ImageTextualElement` to type `TextWord`
- Reworked `PdfRectangle` processing logic when it has more than 4 items
- Fixed `ArgumentOutOfRangeException` when processing 'SpaceBefore' and 'PreferredWidth' parameters
- Added support for PDFs with missing `Type` markers in font descriptors and fill patterns
- Made a workaround to remove empty paragraphs that could be mistakenly added to a document

## All changes

| #               | Summary                                                                                       | Category    |
|-----------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1277 | `SaveAs` API throws `OutOfMemoryException` in the process of Word-to-PDF conversion           | Bug         |
| WORDSCLOUD-1313 | `Split` API throws `NullReferenceException`                                                   | Bug         |
| WORDSCLOUD-1423 | `UpdateTableCellBorder` method changes color incorrectly                                      | Bug         |
| WORDSCLOUD-1458 | `SplitDocument` API throws `IndexOutOfRangeException`                                         | Bug         |
| WORDSCLOUD-1459 | `GetDocumentStatistics` API throws `IndexOutOfRangeException`                                 | Bug         |
| WORDSCLOUD-1474 | `Statistics` API throws `IndexOutOfRangeException`                                            | Bug         |
| WORDSCLOUD-1481 | `SaveAs` API throws `IndexOutOfRangeException`                                                | Bug         |
| WORDSCLOUD-1533 | Swagger error when running Aspose.Words Cloud 21.3 Docker Container                           | Bug         |
| WORDSCLOUD-1534 | Some functions of 'Aspose.Words Cloud 21.3' are not working as expected                       | Bug         |
| WORDSCLOUD-1538 | `SaveAs` API throws 'Unsupported file format' exception                                       | Bug         |
| WORDSCLOUD-1541 | Custom fonts from the '/Font' volume remain unused                                            | Bug         |
| WORDSCLOUD-1487 | Add a new `CustomTimeZoneInfo` property to `SaveOptions`                                      | Feature     |
| WORDSCLOUD-1515 | Ignore the URL-prefix for inner requests in a batch request                                   | Feature     |
| PDF2WORD-722    | The content should appear on a previous page                                                  | Bug         |
| PDF2WORD-725    | Use a stub image in case `ImageSharp` fails to process one                                    | Bug         |
| PDF2WORD-744    | `ArgumentException`: 'An item with the same key has already been added'                       | Bug         |
| PDF2WORD-745    | Unable to cast an object of `ImageTextualElement` type to `TextWord` type                     | Bug         |
| PDF2WORD-746    | `InvalidOperationException`: 'Rectangle must contain exactly 4 numbers'                       | Bug         |
| PDF2WORD-747    | `ArgumentOutOfRangeException` is thrown when processing the 'SpaceBefore' parameter           | Bug         |
| PDF2WORD-759    | `ArgumentOutOfRangeException` is thrown when processing the 'PreferredWidth' parameter        | Bug         |
| PDF2WORD-760    | `InvalidOperationException`: 'PDF pattern dictionary must contain 'type/pattern' key-value pair.' | Bug         |
| PDF2WORD-761    | `System.Exception`: a font descriptor should contain the 'type'-key.                          | Bug         |
| PDF2WORD-770    | Unexpected empty paragraph is added to documents with fields in Headers/Footers.              | Bug         |
