---
title: "21.01 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-01/
aliases: [/aspose-words-cloud-21-01-release-notes/]
description: "Aspose Words Cloud 21.01 Release Notes"
weight: 70
---

The page contains release notes for Aspose.Words Cloud 21.01 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Refactoring of Go SDK, all API method signatures are changed
- Added support of batch requests to Go SDK
- Added typed `NodePath` builder to .NET SDK

## PDF to Word conversion improvements

- Invisible text from PDFs will be skipped now
- Corrected paragraph width after font replacement happens
- Fixed splitting of text lines with Arabic symbols
- Removed empty transparent images from result documents
- Improved font style recognition on Hebrew pages
- Fixed various PDF reading errors
- Corrected page background conversion by supporting `gs` PDF operator
- Fixed "Content extraction is restricted by file permissions" error


## All changes

| #               | Summary                                                                       | Category    |
|-----------------|-------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1396 | Document protection level change method doesn't work for protected documents  | Bug         |
| WORDSCLOUD-1425 | Image quality of OfficeMath object in DOCX to HTML conversion                 | Bug         |
| WORDSCLOUD-1317 | Typed `NodePath` builder in .NET SDK                                          | Feature     |
| WORDSCLOUD-1398 | Implement batch processing for Go SDK                                         | Feature     |
| PDF2WORD-85     | Skip PDF text that has the same color as background (i.e. invisible)          | Task        |
| PDF2WORD-612    | Different paragraph width within the same page                                | Bug         |
| PDF2WORD-621    | Text line is split into two lines                                             | Bug         |
| PDF2WORD-637    | Support page solid color background                                           | Feature     |
| PDF2WORD-647    | Recognized file contains background empty image                               | Bug         |
| PDF2WORD-648    | Font style doesn't match the PDF text                                         | Bug         |
| PDF2WORD-650    | Can't open a PDF because "Stream length has to be numeric value"              | Bug         |
| PDF2WORD-658    | "Sequence contains no matching element" exception                             | Bug         |
| PDF2WORD-665    | `InvalidOperationException`: PDF corrupt, base font range start invalid       | Bug         |
| PDF2WORD-668    | Content extraction is restricted by file permissions                          | Bug         |
| PDF2WORD-669    | `EnterLiteralStringState` fails with `IndexOutOfRangeException`               | Bug         |
| PDF2WORD-670    | Embedded CFF font map has failed to decode                                    | Bug         |
| PDF2WORD-671    | Image disposing concurrency error                                             | Bug         |
| PDF2WORD-673    | Lost background images after the conversion                                   | Bug         |
