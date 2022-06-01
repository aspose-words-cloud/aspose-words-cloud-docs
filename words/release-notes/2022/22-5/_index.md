---
title: "22.5 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2022/22-5/
aliases: [/aspose-words-cloud-22-5-release-notes/]
description: "Aspose Words Cloud 22.5 Release Notes"
weight: 50
---

The page contains release notes for Aspose.Words Cloud 22.5 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features


## PDF to Word conversion improvements

- Improved processing of incorrect UTF-16 hexadecimal values that are used in Unicode character maps
- Fixed visibility of graphic elements when they intersect with tables below or above them
- Implemented conversion of PDF pages with multiple image layers (they are merged now into a single image)
- Fixed `InvalidOperationException` in footnote detection code
- Changed the line spacing in paragraphs from 'Exactly' to 'At least' to improve the editability of the resulting documents

## Cloud SDK Changes

**All SDKs**: fixes and improvements to the internal API.

## All changes

| #               | Summary                                                                      | Category |
|-----------------|------------------------------------------------------------------------------|----------|
| WORDSCLOUD-1963 | PDF to MD/DOCX conversion causes internal error                              | Bug      |
| WORDSCLOUD-1984 | Swift SDK internal error when connecting to production server                | Bug      |
| WORDSCLOUD-1987 | Wrong result file when comparing documents via 'Online' method call          | Bug      |
| WORDSNET-23025  | `ArgumentException`: Incorrect hex length                                    | Bug      |
| WORDSNET-23527  | Vector graphics is lost when importing a PDF document                        | Bug      |
| WORDSNET-23563  | Content is lost when loading a PDF document                                  | Bug      |
| WORDSNET-23693  | `InvalidOperationException`: Sequence contains more than one matching element  | Bug      |
| WORDSNET-23725  | Incorrect paragraph formatting after Pdf2Word conversion, which affects images added later | Bug      |
