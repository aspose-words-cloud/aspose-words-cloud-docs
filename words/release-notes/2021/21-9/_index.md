---
title: "21.9 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-9/
aliases: [/aspose-words-cloud-21-8-release-notes/]
description: "Aspose Words Cloud 21.9 Release Notes"
weight: 30
---

The page contains release notes for Aspose.Words Cloud 21.9 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Multiple bug fixes and code improvements

## PDF to Word conversion improvements

- Implemented a new feature that saves custom PDF properties and transfers them into DOCX counterparts
- Fixed a `NullReferenceException` caused by empty table rows with no cells after `PDF2Word` conversion
- Fixed an `ArgumentNullException` when one of PDF properties contains a composite value
- Fixed an `InvalidCastException` in font reading code

## All changes

| #               | Summary                                                                                       | Category |
|-----------------|-----------------------------------------------------------------------------------------------|----------|
| WORDSCLOUD-1309 | The SplitDcoument API throws `OutOfMemoryException`                                           | Bug      |
| WORDSCLOUD-1547 | The Comparison API results in an I/O error ('Image file cannot be written to disk')           | Bug      |
| WORDSCLOUD-1565 | Processing files from Dropbox Storage results in an error ('Cannot access a closed stream')   | Bug      |
| WORDSCLOUD-1718 | An empty result is returned to a client when an error is caused by the `online`-method        | Bug      |
| WORDSCLOUD-1720 | An error occurs when running BDD tests inside the Docker container                            | Bug      |
| WORDSCLOUD-1725 | The Comparison API `online`-methods produce the result in DOCX format instead of HTML         | Bug      |
| WORDSCLOUD-1726 | Incorrect data in log files                                                                   | Bug      |
| WORDSCLOUD-1744 | The Comparison API causes a 'Bad request' error                                               | Bug      |
| PDF2WORD-815    | The `ClusterBuilder` API merges distantly located glyphs                                      | Bug      |
| PDF2WORD-843    | The 'Footer' element is missing when column detection is enabled                              | Bug      |
| PDF2WORD-845    | Line spacing becomes invalid when column detection is enabled                                 | Bug      |
| PDF2WORD-869    | Read custom properties from a PDF file and store them in a `PdfDocumentInfo` object           | Task     |
| PDF2WORD-870    | Implement custom saving-properties for DOCX files                                             | Task     |
| PDF2WORD-875    | `System.NullReferenceException` is thrown                                                     | Bug      |
| PDF2WORD-893    | `ArgumentOutOfRangeException` is thrown when column detection is enabled                      | Bug      |
| PDF2WORD-899    | `ArgumentNullException`: Value cannot be null. (Parameter 'value')                            | Bug      |
| PDF2WORD-900    | `PdfFontBuilderArgs.CalculateBaseFont()` method throws `InvalidCastException`                 | Bug      |
