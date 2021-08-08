---
title: "21.7 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-7/
aliases: [/aspose-words-cloud-21-7-release-notes/]
description: "Aspose Words Cloud 21.7 Release Notes"
weight: 40
---

The page contains release notes for Aspose.Words Cloud 21.7 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Implemented an automated solution for publishing C++ SDK binaries on GitHub with release CI/CD
- Added an option for saving IML files (`ImlRenderingMode`)
- Added an option for saving text (`MaxCharactersPerLine`)
- Implemented an API to obtain RSA public keys used in document password encryption
- Added a common query option to pass encrypted passwords (`encryptedPassword`)

## PDF to Word conversion improvements

- Improved the handling of PDF encrypted documents in accordance with Adobe PDF Encryption Revisions 2 and 3
- Fixed a series of `ZlibExceptions` caused by incorrect `ObjectEncryptionKey` parameter value for RC4-encrypted PDF files
- Fixed several `InvalidOperationExceptions` appeared as 'Operator should take N operands' messages
- Added a default value for `BitsPerComponent` property of PDF images to avoid errors
- Reworked the 'Unicode font CMaps reading' algorithm to support 1-to-N symbol replacement
- Fixed the incorrect spacing for words consisting of a single character
- Restored missing text for cases where an `XObject` form is placed inside the other

## All changes

| #               | Summary                                                                                       | Category |
|-----------------|-----------------------------------------------------------------------------------------------|----------|
| WORDSCLOUD-1340 | 'Split Document' API throws `OutOfMemoryException`                                            | Bug      |
| WORDSCLOUD-1485 | 'Put Online/SaveAs Document to fixed HTML layout' APIs return only CSS instead of instead of the complete data (HTML+CSS+resources) | Bug      |
| WORDSCLOUD-1587 | Incorrect descriptions of some online methods                                                 | Bug      |
| WORDSCLOUD-1625 | An error occurs in the process of interaction between the 'Mail Merge' add-on and Google Cloud Storage      | Bug      |
| WORDSCLOUD-1645 | Some methods don't have the `withoutNodePath`-version in Swagger UI                           | Bug      |
| WORDSCLOUD-1661 | An error occurs when running PHP SDK inside a Docker container                                | Bug      |
| WORDSCLOUD-1546 | Implemented an automated solution for publishing C++ SDK binaries on GitHub with release CI/CD | New Feature |
| WORDSCLOUD-1623 | Added a new `ImlRenderingMode` option for saving files                                        | New Feature |
| WORDSCLOUD-1624 | Added a new `MaxCharactersPerLine` option for saving text                                     | New Feature |
| PDF2WORD-812    | Unexpected section break inside an area with two columns                                      | Bug      |
| PDF2WORD-814    | Incorrect column validation                                                                   | Bug      |
| PDF2WORD-816    | Unexpected columns                                                                            | Bug      |
| PDF2WORD-818    | `NotImplementedException`: Security handler is not implemented for V=1, R=3                   | Bug      |
| PDF2WORD-819    | `NotImplementedException`: Security handler is not implemented for V=2, R=2                   | Bug      |
| PDF2WORD-822    | `InvalidOperationException`: Operator should take 6 operands                                  | Bug      |
| PDF2WORD-823    | Missing the `BitsPerComponent` parameter in `PdfImage` dictionary                                 | Bug      |
| PDF2WORD-824    | `ArgumentOutOfRangeException`: CID codes exceed max byte size (parameter 'Length')            | Bug      |
| PDF2WORD-825    | `InvalidOperationException`: Operator should take 4 operands                                  | Bug      |
| PDF2WORD-826    | `InvalidOperationException`: Operator should take 2 operands                                  | Bug      |
| PDF2WORD-839    | A value of the `Font.Spacing` parameter is set to `NaN`                                       | Bug      |
| PDF2WORD-841    | `ZlibException`: Bad state (invalid window size (19))                                         | Bug      |
| PDF2WORD-842    | PDF glyphs are skipped due to an incorrect value of the `ClippingPath` parameter              | Bug      |
