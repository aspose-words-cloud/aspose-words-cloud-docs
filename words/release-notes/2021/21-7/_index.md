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

- Added a new `ImlRenderingMode` option for saving files
- Added a new `MaxCharactersPerLine` option for saving text
- Added a new API method to obtain RSA public keys used in document password encryption
- Added a new `encryptedPassword` common query option to pass an encrypted document password

## PDF to Word conversion improvements

- Improved the handling of PDF encrypted documents in accordance with Adobe PDF Encryption Revisions 2 and 3
- Fixed a series of `ZlibExceptions` caused by incorrect `ObjectEncryptionKey` parameter value for RC4-encrypted PDF files
- Fixed several `InvalidOperationExceptions` appeared as 'Operator should take N operands' messages
- Added a default value for `BitsPerComponent` property of PDF images to avoid errors when it is omitted
- Reworked the 'Unicode font CMaps reading' algorithm to support 1-to-N symbol replacement
- Fixed the incorrect spacing for words consisting of a single character
- Restored missing text for cases where an `XObject` form is placed inside another one

## All changes

| #            | Summary                                                                                       | Category |
|--------------|-----------------------------------------------------------------------------------------------|----------|
| PDF2WORD-812 | Unexpected section break inside an area with two columns                                      | Bug      |
| PDF2WORD-814 | Incorrect column validation                                                                   | Bug      |
| PDF2WORD-816 | Unexpected columns                                                                            | Bug      |
| PDF2WORD-818 | `NotImplementedException`: Security handler is not implemented for V=1, R=3                   | Bug      |
| PDF2WORD-819 | `NotImplementedException`: Security handler is not implemented for V=2, R=2                   | Bug      |
| PDF2WORD-822 | `InvalidOperationException`: Operator should take 6 operands                                  | Bug      |
| PDF2WORD-823 | Missing `BitsPerComponent` parameter in `PdfImage` dictionary                                 | Bug      |
| PDF2WORD-824 | `ArgumentOutOfRangeException`: CID codes exceed max byte size (parameter 'Length')            | Bug      |
| PDF2WORD-825 | `InvalidOperationException`: Operator should take 4 operands                                  | Bug      |
| PDF2WORD-826 | `InvalidOperationException`: Operator should take 2 operands                                  | Bug      |
| PDF2WORD-839 | `Font.Spacing` parameter value is set to `NaN`                                                | Bug      |
| PDF2WORD-841 | `ZlibException`: Bad state (invalid window size (19))                                         | Bug      |
| PDF2WORD-842 | PDF glyphs are skipped due to an incorrect `ClippingPath` parameter value                     | Bug      |
