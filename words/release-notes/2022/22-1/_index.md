---
title: "22.1 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2022/22-1/
aliases: [/aspose-words-cloud-22-1-release-notes/]
description: "Aspose Words Cloud 22.1 Release Notes"
weight: 70
---

The page contains release notes for Aspose.Words Cloud 22.1 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Provided localization support for 'Mail Merge' fields (`FieldOptions.FieldUpdateCultureName`)
- Implemented secure password handling for the second document (to be appended) in `AppendDocument` requests
- Implemented secure password handling for the second document (to be compared with) in `CompareDocument` requests
- Various bug fixes and improvements

## PDF to Word conversion improvements

- Implemeted a workaround for handling PDF strings with uneven parenthesis
- Implemented new functionality to handle incorrect order and duplicates in `BT/ET` operators ('Begin Text'/'End Text')
- Identified and fixed a problem with concurrent image rows processing
- Added support for a new combination of `NamedDestination` parameters (links within a PDF document)
- Implemented `FormatException` handling in a couple of methods to support the conversion of partially incorrect PDF files
- Improved the algorithm to ignore the `Tj` text operator if a font has not been tentatively defined with the `Tf` operator (to avoid logical errors)
- Improved the algorithm to prevent falling into an endless reading loop in `PdfTokenParser` by correcting the processing of the last byte in a PDF stream
- Reworked data buffering algorithm in `PdfSyntaxParser` to support large data arrays (we found a PDF array with 85042 elements)
- Improved the algorithm to prevent `IndexOutOfRangeException` at `ColorSpaceDeviceRGB` (provided support for Gray 8-bit color inside RGB Image Reader)
- Improved the processing of PDF files without proper `/Page` elements (set default collection values for this scenario)

## Cloud SDK Changes

- **All SDKs**: 
  - Added `FieldOptions.FieldUpdateCultureName` parameter to set a specific culture (locale) for 'Mail Merge' fields
  - Added `DocumentEntry.Password` parameter to set an encrypted password for the seconds document (to append) in `AppendDocument` requests
  - Added `EncryptedPassword2` parameter to set an encrypted password for the second document (to compare with) in `CompareDocument` and `CompareDocumentOnline` requests
- **Go SDK**: made exception messages more informative


## All changes

| #                | Summary                                                                                       | Category    |
|------------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1721  | Implement the ability to set custom locales at the 'Mail Merge' template level                | New Feature |
| WORDSCLOUD-1822  | Implement password handling for the second document in `AppendDocument` requests  | New Feature |
| WORDSCLOUD-1823  | Implement password handling for the second document in `CompareDocument` requests | New Feature |
| WORDSCLOUD-1855  | Go SDK: improve error diagnostics, make exception messages more informative                   | New Feature |
| WORDSCLOUD-1866  | Provide complete localization support for 'Mail Merge' fields                                 | New Feature |
| WORDSCLOUD-1464  | `GetDocumentStatistics` API throws "Object reference not set" exception                       | Bug         |
| WORDSCLOUD-1577  | Batch requests return incorrect responses when the `ResultOf` parameter is assigned           | Bug         |
| WORDSCLOUD-1586  | Swagger UI returns an error on some sevice endpoints                                          | Bug         |
| WORDSCLOUD-1857  | Some online methods return incorrect links to processed documents                             | Bug         |
| WORDSCLOUD-1864  | An error occurred while deploying 'Aspose.Words Cloud' to Heroku platform as a Docker container | Bug         |
| WORDSCLOUD-18704 | 'Aspose.Words Cloud API Reference' doesn't mention the `encryptedPassword` parameter          | Bug         |
| WORDSNET-23023   | `FormatException` at `PdfTokenParser.EnterHexStringState`                                     | Bug         |
| WORDSNET-23027   | `NullReferenceException` at `SASLPrepAlgorithm.MapCharacters`                                 | Bug         |
| WORDSNET-23175   | `IndexOutOfRangeException` at `PdfSyntaxParser.ParseArray`                                    | Bug         |
| WORDSNET-23177   | `NullReferenceException` is thrown if page resources are missing                              | Bug         |
| WORDSNET-23189   | `FormatException` at `TimeSpanFormat.FormatCustomized`                                        | Bug         |
| WORDSNET-23192   | `KeyNotFoundException` at `RomanNumber.TryParse`                                              | Bug         |
| WORDSNET-23193   | `InvalidCastException`: Cannot cast `PdfDictionary` to `PdfArray`                             | Bug         |
| WORDSNET-23203   | `NullReferenceException` at `PdfOperatorTj.Apply`                                             | Bug         |
| WORDSNET-23212   | `IndexOutOfRangeException` at `ColorSpaceDeviceRGB.ToRgb`                                     | Bug         |
