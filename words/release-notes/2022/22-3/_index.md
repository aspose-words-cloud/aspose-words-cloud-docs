---
title: "22.3 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2022/22-3/
aliases: [/aspose-words-cloud-22-3-release-notes/]
description: "Aspose Words Cloud 22.3 Release Notes"
weight: 60
---

The page contains release notes for Aspose.Words Cloud 22.3 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- The data type of some members of the `SaveOptions` class, as well as classes inherited from it, has been changed from `string` to the corresponding enums
- Improved data security:
  - Parameters containing sensitive data are transmitted only in encrypted form. The names of such parameters are prefixed with 'encrypted'
  - Added the `Encrypt` method to encrypt data with an API public key. This method can be used to generate encrypted parameter values
- Various other fixes and improvements

## PDF to Word conversion improvements

- Fixed a rare error that could occur when processing encrypted PDF content
- Fixed algorithm for importing images in `JBig2` format
- Improved reading of `MediaBox` page property which describes visible page borders
- Improved handling of links embedded in some PDFs
- Fixed background color recognition algorithm. The bug resulted in the appearance of black cells in tables
- Switched to a different implementation of the `FlateDecode` reader to get more accurate results
- Added limited support for `Type3` fonts by converting text to Unicode characters
- Implemented reading and saving headings (such as `H1`, `H2`, etc.) marked with `BDC` operators
- Improved algorithm for reading table rows with low height
- Fixed Arabic text size inside table cells

## Cloud SDK Changes

**All SDKs**: 
- The online methods return a dictionary of files in responses, with the original filename included as a key, instead of the file's content
- Parameters containing sensitive data are transmitted in encrypted form. The names of such parameters are prefixed with 'encrypted'
- Added the `Encrypt` method to encrypt data with an API public key. This method can be used to generate encrypted parameter values
- The data type of some members of the `SaveOptions` class, as well as classes inherited from it, has been changed from `string` to the corresponding enums

## All changes

| #                | Summary                                                                                       | Category    |
|------------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1907  | Text is not exported correctly when converting from OCR PDF to DOCX/MD format                 | Bug         |
| WORDSCLOUD-1931  | An error occurs when trying to replace (insert) text with HTML in a document using the Range API | Bug      |
| WORDSNET-23026   | `InvalidOperationException`: Encrypt element in the trailer dictionary must also be dictionary  | Bug       |
| WORDSNET-23037   | `IndexOutOfRangeException` at `JBig2Decoder.JBIG2Bitmap.DuplicateRow`                         | Bug         |
| WORDSNET-23190   | `KeyNotFoundException`: MediaBox was not present in the dictionary                            | Bug         |
| WORDSNET-23191   | `KeyNotFoundException`: Dictionary doesn't contain 'S' entry                                  | Bug         |
| WORDSNET-23204   | Incorrect text with black background after the conversion                                     | Bug         |
| WORDSNET-23221   | Incorrect result of `PdfFlateDecodeFilter`                                                    | Bug         |
| WORDSNET-23403   | Implement PDF text conversion written in `Type3` font using `ToUnicode` character map         | Task        |
| WORDSNET-23414   | Preserve paragraph outline level when importing a tagged PDF document                         | Feature     |
| WORDSNET-23472   | `NullReferenceException` at `TableBordersFilter.GetBorders`                                   | Bug         |
| WORDSNET-23478   | Some characters are retrieved incorrectly                                                     | Bug         |
| WORDSNET-23497   | Table is distorted when importing PDF                                                         | Bug         |
| WORDSNET-23510   | Arabic text inside table cells is too large                                                   | Bug         |
