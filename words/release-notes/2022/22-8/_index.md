---
title: "22.8 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2022/22-8/
aliases: [/aspose-words-cloud-22-8-release-notes/]
description: "Aspose Words Cloud 22.8 Release Notes"
weight: 35
---

The page contains release notes for Aspose.Words Cloud 22.8 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Improved performance when working with Azure Cloud Storage
- Fixed styles/formatting error when converting DOCX to HTML
- Fixed import algorithms in AppendDocument API (when `KeepSourceFormatting` option is enabled)


## PDF to Word conversion improvements

- Improved recognition of tables with RTL text
- Fixed handling of graphics inside tables
- Fixed a bug when processing footnotes


## All changes

| #               | Summary                                                                                              | Category |
|-----------------|------------------------------------------------------------------------------------------------------|----------|
| WORDSCLOUD-1536 | Footer page number alignment is lost when converting DOCX to HTML and back to DOCX                   | Bug      |
| WORDSCLOUD-1962 | Performance issue when appending Word documents from Azure storage                                   | Bug      |
| WORDSCLOUD-1991 | AppendDocument API: `KeepSourceFormatting ImportFormatMode` does not keep styles of the document intact | Bug      |
| WORDSNET-23917  | `InvalidOperationException` at `FootnoteCorrector.MergeLines`                                        | Bug      |
| WORDSNET-23620  | The last characters from the first column are moved to the second column of the RTL table            | Bug      |
| WORDSNET-24032  | Part of the content disappears and text wrapping changes after PDF import                            | Bug      |
| WORDSNET-24042  | PDF document with tables is imported incorrectly                                                     | Bug      |
| WORDSNET-24043  | RTL content is imported incorrectly from PDF documents                                               | Bug      |
| WORDSNET-23619  | The spacing between words in some cells of the RTL table is too large                                | Bug      |
