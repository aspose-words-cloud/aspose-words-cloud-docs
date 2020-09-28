---
title: "20.9 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2020/20-9/
aliases: [/aspose-words-cloud-20-9-release-notes/]
description: "Aspose Words Cloud 20.9 release notes"
weight: 10
---

The page contains release notes for Aspose.Words Cloud 20.9 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words

- Added "Batch API" feature

## PDF

- Improved font recognition logic
- Corrected footnotes overlapping with footer area
- Fixed splitting issues with numbered lists
- Removed redundant paragraph breaks caused by footnote references
- Corrected interval height between list items
- Recovered a few pages that were lost by the wrong rotation detection
- Fixed extra empty pages added because of unrecognized header parts

## All changes

| #               | Summary                                                                                            | Category |
|-----------------|----------------------------------------------------------------------------------------------------|----------|
| WORDSCLOUD-1257 | DeleteMacros API Method throws internalError while loading file                                    | Bug      |
| WORDSCLOUD-1260 | DeleteMacros API Method throws unable to cast object error                                         | Bug      |
| WORDSCLOUD-1321 | Files from "split and zip" saved as input data in logsr                                            | Bug      |
| WORDSCLOUD-1347 | Change ZIP implementation in Split API                                                             | Task     |
| PDF2WORD-543    | Use WarningCallback to notify about font substitution                                              | Task     |
| PDF2WORD-544    | Many joined words in a result document when recognizing on Linux                                   | Bug      |
| PDF2WORD-546    | Implement JsonFontCache to achieve good recognition quality on Linux                               | Task     |
| PDF2WORD-548    | Investigate the possibility of font detection rework                                               | Task     |
| PDF2WORD-550    | Wrong text was detected as footnotes                                                               | Bug      |
| PDF2WORD-555    | List items are separated from each other                                                           | Bug      |
| PDF2WORD-556    | Wrong paragraph split                                                                              | Bug      |
| PDF2WORD-559    | Low interval between text lines after the conversion                                               | Bug      |
| PDF2WORD-565    | Integrate a DI container                                                                           | Task     |
| PDF2WORD-572    | Pages lost in the resultant word document                                                          | Bug      |
| PDF2WORD-576    | DI doesn't work in release builds because of obfuscation                                           | Bug      |
| PDF2WORD-579    | Wrong header recognition created two extra pages in the output document                            | Bug      |
| PDF2WORD-581    | A paragraph is recognized as two separate paragraphs, which a breaks the sequence of list segments | Bug      |
| PDF2WORD-585    | Autofac doesn't work on Android after obfuscation                                                  | Bug      |

## SDK Changes

## Aspose.Words Cloud .NET SDK

- Added new api method

```C#
/batch
```


