---
title: "23.4 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2023/23-4/
aliases: [/aspose-words-cloud-23-4-release-notes/]
description: "Aspose Words Cloud 23.4 Release Notes"
weight: 55
---

The page contains release notes for Aspose.Words Cloud 23.4 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Implemented a new type `RangeEndIdentifier` as part of the Range API
- Fixed an issue with font substitution
- Various changes that improve stability and performance

## PDF to Word conversion improvements

- Fixed an issue with handling footnotes
- Improved PDF import methods


## All changes

| #                | Summary                                                                                       | Category    |
|------------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSNET-24666   | `InvalidOperationException`: footnotes are only allowed inside the main text of the document  | Bug         |
| WORDSNET-25170   | `System.NotImplementedException` : cannot add `ApsImageWrapper` into `ApsPageModel`           | Bug         |
| WORDSNET-25174   | `ZlibException`: Bad state (invalid bit length repeat)                                        | Bug         |
| WORDSNET-25185   | `InvalidOperationException`: PDF corrupt. Invalid PDF page node object                        | Bug         |
| WORDSCLOUD-2243  | Implement the ability to use the `GetRangeTextOnline` API without passing the end identifier  | New Feature |
| WORDSCLOUD-2317  | Formatting issue related to Arial fonts when converting DOCX to PDF                           | Bug         |
| WORDSCLOUD-2293  | Exception thrown in batch download requests                                                   | Bug         |
