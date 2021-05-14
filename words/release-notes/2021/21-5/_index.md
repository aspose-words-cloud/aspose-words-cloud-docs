---
title: "21.5 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-5/
aliases: [/aspose-words-cloud-21-5-release-notes/]
description: "Aspose Words Cloud 21.5 Release Notes"
weight: 50
---

The page contains release notes for Aspose.Words Cloud 21.5 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Improved speed of execution for `Split` and `Statistics` operations
- Fixed multiple bugs in `Split` and `Statistics` operations

## PDF to Word conversion improvements

- Corrected detection of footnotes with Roman and Letter numbering styles
- Fixed a `KeyNotFoundException` when a PDF image stream doesn't have `Length` property
- Fixed another `KeyNotFoundException` when a PDF color mask doesn't specify its type
- Corrected PDF reading code to support annotations without `Subtype` property

## All changes

| #               | Summary                                                                                       | Category    |
|-----------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-364  | Execute MailMerge and save the output document as PDF in one request                          | Feature     |
| WORDSCLOUD-409  | Replace multiple text items in a single API call                                              | Feature     |
| WORDSCLOUD-1270 | Split documents by page range to generate a single document                                   | Feature     |
| WORDSCLOUD-1351 | Replace multiple text values in a Word document without using cloud storage                   | Feature     |
| WORDSCLOUD-1444 | Implement `PUT /CompatibilityOptions/` resource                                               | Feature     |
| WORDSCLOUD-1576 | Implement `resultOf` feature in Node SDK                                                      | Feature     |
| WORDSCLOUD-1579 | Implement `resultOf` feature for online methods with multipart body                           | Feature     |
| WORDSCLOUD-1582 | Implement `dependsOn` feature in .NET SDK                                                     | Feature     |
| WORDSCLOUD-1584 | Implement `dependsOn` feature in Ruby SDK                                                     | Feature     |
| WORDSCLOUD-1585 | Improve `BatchRequest` functionality in Node SDK for better usability                         | Feature     |
| WORDSCLOUD-92   | Conversion error when splitting DOC to PNG and HTML                                           | Bug         |
| WORDSCLOUD-326  | SplitDocument API produces documents only with 2 pages                                        | Bug         |
| WORDSCLOUD-715  | Sentences are split incorrectly across multiple pages                                         | Bug         |
| WORDSCLOUD-1092 | Invalid word counting performance of Statistics API                                           | Bug         |
| WORDSCLOUD-1232 | SplitDocument API throws `OutOfMemoryException`                                               | Bug         |
| WORDSCLOUD-1234 | GetDocumentStatistics API throws `OutOfMemoryException`                                       | Bug         |
| WORDSCLOUD-1256 | SplitDocument API throws `OutOfMemoryException`                                               | Bug         |
| WORDSCLOUD-1342 | Split API throws `OutOfMemoryException`                                                       | Bug         |
| WORDSCLOUD-1391 | AppendDocument API breaks alignment of tables                                                 | Bug         |
| WORDSCLOUD-1454 | Error in the process of converting DOCX to MD format                                          | Bug         |
| WORDSCLOUD-1460 | GetDocumentStatistics API is not able to load a file                                          | Bug         |
| WORDSCLOUD-1462 | GetDocumentStatistics API throws `OutOfMemoryException`                                       | Bug         |
| WORDSCLOUD-1463 | GetDocumentStatistics API throws "Invalid document model" exception                           | Bug         |
| WORDSCLOUD-1469 | Statistics API throws `ArgumentNullException`                                                 | Bug         |
| WORDSCLOUD-1537 | GetDocumentStatistics API throws "Invalid document model" exception                           | Bug         |
| WORDSCLOUD-1581 | Internal Server Error (500) in the process of converting DOC to Markdown                      | Bug         |
| WORDSCLOUD-1591 | Unit tests for checking online method do not pass when they are executed in Visual Studio     | Bug         |
| PDF2WORD-705    | Provide support for different footnote numbering styles                                       | Task        |
| PDF2WORD-706    | Only the first footnote with Roman numerals was detected                                      | Bug         |
| PDF2WORD-773    | `KeyNotFoundException`: "Dictionary doesn't contain `Subtype` entry"                          | Bug         |
| PDF2WORD-775    | `KeyNotFoundException`: "Dictionary doesn't contain `Type` entry"                             | Bug         |
