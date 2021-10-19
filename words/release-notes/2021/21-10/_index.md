---
title: "21.10 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-10/
aliases: [/aspose-words-cloud-21-10-release-notes/]
description: "Aspose Words Cloud 21.10 Release Notes"
weight: 25
---

The page contains release notes for Aspose.Words Cloud 21.10 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Removed an outdated `GraphicsQualityOptions` image save option as it is no longer supported
- Added a new `displayIntermediateResults` query parameter for batch requests. When set to `false`, only the last response in a batch will be returned. By default the value is set to `true`.

## PDF to Word conversion improvements

- Fixed the processing of unsupported `Annotation` types - skipping them to avoid `ArgumentException`
- Fixed multiple `InvalidCastException`s when received PDF data doesn't match the expected format
- Fixed multiple errors in PDF column detection: spacing, page numbers, list markers, text borders
- Enabled multicolumn PDF recognition for all users

## All changes

| #               | Summary                                                                                       | Category |
|-----------------|-----------------------------------------------------------------------------------------------|----------|
| PDF2WORD-872    | `ArgumentException`: Requested value '3D' was not found                                       | Bug      |
| PDF2WORD-891    | Incorrect page number appears if column detection is enabled                                  | Bug      |
| PDF2WORD-892    | Invalid spacing in multicolumn sections                                                       | Bug      |
| PDF2WORD-895    | Columns are not detected in text with a border                                                | Bug      |
| PDF2WORD-896    | A column with list markers is detected only                                                   | Bug      |
| PDF2WORD-901    | `InvalidCastException`: Unable to cast `PdfIndirectObjectReference` to `PdfName`              | Bug      |
| PDF2WORD-902    | `InvalidCastException`: Unable to cast `PdfName` to `PdfUnfilteredStream`                     | Bug      |
| PDF2WORD-903    | `InvalidCastException`: Unable to cast `PdfIndirectObjectReference` to `PdfNumber`            | Bug      |
| PDF2WORD-904    | `InvalidCastException`: Unable to cast `PdfUnfilteredStream` to `PdfDictionary`               | Bug      |
| PDF2WORD-906    | `InvalidCastException`: Unable to cast `PdfFloat` to `PdfInteger`                             | Bug      |
| PDF2WORD-907    | `InvalidCastException`: Unable to cast `PdfUnfilteredStream` to `PdfArray`                    | Bug      |
| PDF2WORD-908    | `InvalidCastException`: Unable to cast `PdfInteger` to `PdfArray`                             | Bug      |
| PDF2WORD-909    | `InvalidCastException`: Unable to cast `PdfIndirectObjectReference` to `PdfString`            | Bug      |
| PDF2WORD-914    | The bottom segment is missing when column detection is enabled                                | Bug      |
| PDF2WORD-926    | Enable column detection by default                                                            | Task     |

