---
title: "21.12 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-12/
aliases: [/aspose-words-cloud-21-12-release-notes/]
description: "Aspose Words Cloud 21.12 Release Notes"
weight: 15
---

The page contains release notes for Aspose.Words Cloud 21.12 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Implemented the "/info" endpoint to obtain API usage details
- Added support for configuring `document.FieldOptions` in the process of MailMerge
- Improved protection for `CommonRequestParameters.Password`
- Provided an option to exclude intermediate document's data from responses during 'Batch Request' processing
- Provided support for OfficeMath-to-SVG rendering in the process of DOCX-to-HTML conversion
- Multiple bug fixes and improvements

## PDF to Word conversion improvements

- Implemented the detection of footnotes that have no horizontal separator line above them
- Determined the location and fixed a bug in release building scripts, causing errors in the "JPEG 2000" decoder
- Improved the `cm` operator processing to get correct text coordinates
- Improved the PDF importing algorithm: word duplicates are ignored now if they have the same coordinates and text
- Implemented decoding for the newest 'PDF encryption Rev 6' (PDF 2.0 and PDF 1.7 Extension 6 formats)
- Improved data editing logic to avoid "Collection was modified" errors
- Optimized footnotes scanning area to avoid `InvalidOperationException`
- Implemented the 'Default Font' protective mode, activated when a PDF font has incorrect data or its subtype can't be determined
- Improved the processing of references in PDF, pointing to non-existent objects

## All changes

| #               | Summary                                                                                       | Category    |
|-----------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1424 | Provide support for OfficeMath-to-SVG rendering in the process of DOCX-to-HTML conversion     | New Feature |
| WORDSCLOUD-1450 | Improve protection for `CommonRequestParameters.Password`                                     | New Feature |
| WORDSCLOUD-1480 | Change all API calls to asynchronous (`async/await`) in .NET SDK                              | New Feature |
| WORDSCLOUD-1507 | Add an option to exclude intermediate document's data from responses during batch processing  | New Feature |
| WORDSCLOUD-1742 | Provide support for configuring `document.FieldOptions` in the process of MailMerge           | New Feature |
| WORDSCLOUD-1784 | Provide an option to remove superscript text in PDF to Markdown conversion                    | New Feature |
| WORDSCLOUD-1828 | Implement timeout configuration (settings) for Cloud SDKs                                     | New Feature |
| WORDSCLOUD-1416 | Issue with using control chars (page breaks) in LINQ Reporting templates                      | Bug         |
| WORDSCLOUD-1419 | PHP SDK (Cloud API): logging request in debug mode doesn't work                               | Bug         |
| WORDSCLOUD-1447 | Image resize issue in MailMerge Templates                                                     | Bug         |
| WORDSCLOUD-1678 | Storage providers cause errors when reading input streams for the second time                 | Bug         |
| WORDSCLOUD-1717 | `ExecuteMailMerge` API method throws "Invalid container" exception                            | Bug         |
| WORDSCLOUD-1748 | `CompareDocumentOnline` API method fails to save an output to Cloud storage                   | Bug         |
| WORDSCLOUD-1750 | Error when populating images from Cloud storage with `MailMerge` online method                | Bug         |
| WORDSCLOUD-1751 | `EmptyParagraphs` cleanup option is not working as expected                                   | Bug         |
| WORDSCLOUD-1761 | `EncryptedPassword` is not working for online methods                                         | Bug         |
| WORDSCLOUD-1813 | Calling `BuildReportOnline` via `cURL` returns an error                                       | Bug         |
| WORDSCLOUD-1814 | Incorrect usage details in the Docker Container                                               | Bug         |
| WORDSCLOUD-1816 | Document conversion speed issue in Aspose.Words Cloud Docker Container                        | Bug         |
| WORDSCLOUD-1820 | Timeout error occurs when generating long reports                                             | Bug         |
| WORDSNET-23048  | Text is skipped because of incorrect `ClippingBounds` calculation                             | Bug         |
| WORDSNET-23058  | Implement the detection of footnotes that have no horizontal separator line above them        | Task        |
| WORDSNET-22968  | `FileLoadException` is thrown in the process of loading a PDF                                 | Bug         |
| WORDSNET-22969  | Content is missing when converting PDF to DOCX                                                | Bug         |
| WORDSNET-22970  | Extra content is found when converting PDF to DOCX                                            | Bug         |
| WORDSNET-23060  | Duplicated letters in words detected after the conversion                                     | Bug         |
| WORDSNET-23047  | `NotImplementedException`: Security handler is not implemented for V=5, R=6                   | Bug         |
| WORDSNET-23050  | `NullReferenceException` when a PDF file has empty cross-reference stream                     | Bug         |
| WORDSNET-23061  | `NullReferenceException` at `TableOfContentsTabStorage.NumberIsIncreasing`                    | Bug         |
| WORDSNET-23062  | `InvalidOperationException`: Subtype must be present in a `Font` resource                     | Bug         |
| WORDSNET-23065  | `InvalidOperationException`: PDF is corrupt. Reference does not point to a valid indirect object. | Bug     |
| WORDSNET-23139  | `InvalidOperationException`: Collection was modified                                          | Bug         |
| WORDSNET-23140  | `InvalidOperationException`: Footnotes are only allowed inside the main text of the document  | Bug         |
| WORDSNET-23028  | `NullReferenceException` at CSJ2K's `FileFormatReader.readFileFormat`                         | Bug         |
| WORDSNET-23021  | `NullReferenceException` at CSJ2K's `FileBitstreamReaderAgent..ctor`                          | Bug         |
| WORDSNET-23020  | `NullReferenceException` at CSJ2K's `readBox()`                                               | Bug         |

