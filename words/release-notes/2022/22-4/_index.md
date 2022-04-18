---
title: "22.4 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2022/22-4/
aliases: [/aspose-words-cloud-22-4-release-notes/]
description: "Aspose Words Cloud 22.4 Release Notes"
weight: 55
---

The page contains release notes for Aspose.Words Cloud 22.4 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Enhanced HTML export: added support for `ExportShapesAsSvg` in `HtmlSaveOptions`
- Added new endpoint `~/styles/copy_from`

## PDF to Word conversion improvements

- Improved image cleanup logic for searchable PDFs containing text behind images
- Fixed the order of parentheses in Arabic text inside tables
- Fixed detection of colored cells in large tables with multiline text cells
- Fixed several issues with table detection when rows have small height
- Improved support of non-standard footnotes that have no visible separators
- Improved page processing logic to avoid splitting large lists into smaller parts
- Fixed incorrect line breaks in centered page titles with two or more lines
- Fixed `ArgumentNullException` when processing PDF annotations

## Cloud SDK Changes

**All SDKs**: 

- Enhanced HTML export: added support for `ExportShapesAsSvg` in `HtmlSaveOptions`
- Added new endpoint `~/styles/copy_from`

**.NET SDK**: implemented the ability to set proxy configuration

## All changes

| #                | Summary                                                                                       | Category    |
|------------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1662   | Implement `Document.CopyStylesFromTemplate` feature                                               | New Feature  |
| WORDSCLOUD-1927   | Add support for `ExportShapesAsSvg` in `HtmlSaveOptions`                                          | New Feature  |
| WORDSCLOUD-1961   | Implement the ability to set proxy configuration in 'Aspose.Words Cloud SDK for .NET'             | New Feature  |
| WORDSCLOUD-1933   | Issue with detecting custom footnotes in multipage PDF                                            | Bug          |
| WORDSCLOUD-1958   | Error when calling `AppendDocumentOnline` method in PHP SDK                                       | Bug          |
| WORDSCLOUD-1960   | Array indexing fails with exception in PHP SDK                                                    | Bug          |
| WORDSNET-23419    | Large images (redundant scans) should be removed from a searchable PDF during processing          | Bug          |
| WORDSNET-23499    | Inaccurate Arabic text appears when importing a PDF                                               | Bug          |
| WORDSNET-23506    | Cell background color issue when importing a PDF                                                  | Bug          |
| WORDSNET-23507    | Table is distorted when importing a PDF                                                           | Bug          |
| WORDSNET-23548    | `FootnoteDetector` fails to find footnotes above page numbers                                     | Bug          |
| WORDSNET-23610    | Line break is lost when resaving a PDF                                                            | Bug          |
| WORDSNET-23631    | `System.ArgumentNullException`: Value cannot be null                                              | Bug          |