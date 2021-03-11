---
title: "21.3 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-3/
aliases: [/aspose-words-cloud-21-3-release-notes/]
description: "Aspose Words Cloud 21.3 Release Notes"
weight: 60
---

The page contains release notes for Aspose.Words Cloud 21.3 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Added a new `UpdateCreatedTimeProperty` option for saving output files
- Added support for multiple tables in `HeaderFooter` objects. Thus it's possible to address paragraphs inside a table as follows: "sections/0/headersfooters/1/tables/0/rows/0/cells/0/paragraphs/0"

## PDF to Word conversion improvements

- Improved formatting for a table of contents when page numbers are not aligned
- Corrected erroneously reduced spacing between words in some text paragraphs
- Corrected PDF element derefencing when `xref` table has incorrect data
- Added support for PDFs with duplicate values in `Font` encoding dictionaries
- Added support for white symbols in `ASCII-85` text to fix decoding of such files
- Added support for PDFs with missed `Content` and `Resources` elements
- Fixed `NullReferenceException` in the process of `PdfContentProcessor` class creation
- Fixed issues causing `FormatException` on a dozen of PDFs
- Restored color decoding by adding new logic for `Shading` fill pattern
- Added support for images with 2-bit colors (when 4 pixels are encoded into one byte)
- Fixed the "Can't receive the results" exception, caused by PDFs with images

## All changes

| #               | Summary                                                                                       | Category    |
|-----------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1488 | Add a new `UpdateCreatedTimeProperty` to `SaveOptions`                                        | Feature     |
| WORDSCLOUD-1512 | Provide support for multiple `Table` objects in `HeaderFooter` objects                        | Feature     |
| WORDSCLOUD-1379 | Issue with executing Mail Merge API                                                           | Bug         |
| WORDSCLOUD-1445 | `GetFields()` and `SaveAs()` methods throw `InternalError` exception                          | Bug         |
| WORDSCLOUD-1457 | Split API throws "Object reference not set ..." exception                                     | Bug         |
| WORDSCLOUD-1466 | Statistics API throws "Object reference not set ..." exception                                | Bug         |
| WORDSCLOUD-1467 | Statistics API and Split API throw "Unable to cast object" exception                          | Bug         |
| WORDSCLOUD-1468 | Statistics API throws "Object reference not set ..." exception                                | Bug         |
| WORDSCLOUD-1470 | Split API throws "Parameter is not valid" exception                                           | Bug         |
| WORDSCLOUD-1472 | Issue with `SaveAs()` method and ODF format                                                   | Bug         |
| WORDSCLOUD-1483 | Support,SplitDocument API throws "Parameter is not valid" exception                           | Bug         |
| WORDSCLOUD-1509 | Issue with reading paragraph format from a header                                             | Bug         |
| PDF2WORD-683    | Integrate a new OCR project with PDF2Word                                                     | Task        |
| PDF2WORD-684    | Table of contents conversion issues                                                           | Bug         |
| PDF2WORD-686    | Increased spacing between words                                                               | Bug         |
| PDF2WORD-691    | `SixLabors.ImageSharp` fails to find actual image size                                        | Bug         |
| PDF2WORD-700    | Page numbers in a table of contents are not aligned                                           | Bug         |
| PDF2WORD-701    | Line spacing in a table of contents is too large                                              | Bug         |
| PDF2WORD-703    | `InvalidOperationException`: "Pdf corrupt. Reference with Obj #78. Gen #0 does not point ..." | Bug         |
| PDF2WORD-707    | Provide support for duplicates in Font/Encoding/Difference arrays                             | Task        |
| PDF2WORD-708    | Add `Image2Word` facade class to provide OCR feature for Aspose.Apps                          | Task        |
| PDF2WORD-724    | `InvalidOperationException`: "Invalid ASCII base-85 character"                                | Bug         |
| PDF2WORD-726    | `InvalidOperationException`: "Page neither contains nor inherits a `Resource` dictionary"     | Bug         |
| PDF2WORD-727    | `NullReferenceException` is thrown during `PdfContentProcessor` creation                      | Bug         |
| PDF2WORD-728    | `FileLoadException`: "The file doesn't have PDF header and/or footer"                         | Bug         |
| PDF2WORD-729    | `FormatException`: "Input string was not in a correct format"                                 | Bug         |
| PDF2WORD-730    | Colons alignment is lost                                                                      | Bug         |
| PDF2WORD-731    | Increased spacing between words                                                               | Bug         |
| PDF2WORD-732    | `ArgumentException`: "Unsupported number of bits per item: 2"                                 | Bug         |
| PDF2WORD-733    | `InvalidOperationException`: "Can't receive the results"                                      | Bug         |
| PDF2WORD-734    | `InvalidOperationException`: "Pdf corrupt. Reference with Obj #76. Gen #0 does not point ..." | Bug         |
| PDF2WORD-735    | Image colors are lost in the process of conversion                                            | Bug         |
