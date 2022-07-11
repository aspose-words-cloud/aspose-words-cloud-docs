---
title: "22.7 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2022/22-7/
aliases: [/aspose-words-cloud-22-7-release-notes/]
description: "Aspose Words Cloud 22.7 Release Notes"
weight: 40
---

The page contains release notes for Aspose.Words Cloud 22.7 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Improved the 'AppendDocument' method to support 'ImageEntryList' in order to directly append images to a document and images to an image
- Implemented the 'CompressDocument' API for reducing the size of a document, and for compressing and resizing images within a document


## PDF to Word conversion improvements

- Fixed reading PDF pages with background images
- Fixed a couple of problems in encrypted PDFs' import
- Added new logic that merges duplicates in custom document properties (to avoid errors later)
- Reworked 'Metadata' section reading to support both encrypted and non-encrypted formats
- Filtered out PDF images with incorrect width or height (less than 1 pixel)
- MediaBox data recovery was improved to work properly with complex page trees

## Cloud SDK Changes

- **.NET, C++, Dart, Go, Node.js, Swift SDKs**:
    - Improved the 'AppendDocument' method to support 'ImageEntryList' in order to directly append images to a document and images to an image
    - Implemented the 'CompressDocument' API for reducing the size of a document, and for compressing and resizing images within a document


## All changes

| #               | Summary                                                                                              | Category    |
|-----------------|------------------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1654 | Parse the multipart response and make it possible to download individual files from it using Swagger UI | New Feature |
| WORDSCLOUD-2035 | Implement new API to compress documents                                                              | New Feature |
| WORDSCLOUD-2038 | Implement new API to merge images to a document and images to an image                               | New Feature |
| WORDSCLOUD-1574 | Converting DOCX to HTML and back to DOCX changes the color of list items                             | Bug         |
| WORDSCLOUD-2041 | `Filemanager` instance has not been initialized on the production server                             | Bug         |
| WORDSCLOUD-2057 | Ruby SDK: incorrect timeout handling                                                                 | Bug         |
| WORDSNET-23810  | Incorrect background image after `Pdf2Word` conversion                                               | Bug         |
| WORDSNET-23855  | `CryptographicException`: The input data is not a complete block                                     | Bug         |
| WORDSNET-23918  | `ArgumentException` is thrown due to duplicate elements in `CustomDocumentProperties`                | Bug         |
| WORDSNET-23941  | `ZlibException`: Bad state (invalid distance code)                                                   | Bug         |
| WORDSNET-23947  | `OverflowException`: Value was either too large or too small for an `Int32`                          | Bug         |
| WORDSNET-23948  | `InvalidOperationException`: MediaBox is null                                                        | Bug         |
