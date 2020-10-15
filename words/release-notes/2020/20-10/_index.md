---
title: "20.10 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2020/20-10/
aliases: [/aspose-words-cloud-20-10-release-notes/]
description: "Aspose.Words Cloud 20.10 Release Notes"
weight: 10
---

The page contains release notes for Aspose.Words Cloud 20.10 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words

- Various fixes and improvements

## PDF

- Reduced amount of the wrong paragraph splits by improving text line comparison logic
- Reworked page numbering detection to support more patterns and number formats (including Roman numerals)
- Improved space size calculation to correct the reported issues with words joined together
- Removed redundant paragraph breaks caused by footnote references
- Fixed the spacing in lists after the first item
- Implemented the first iteration of paragraph joining logic between adjacent pages (a similar change for lists will be made later)

## All changes

| #            | Summary                                                                                | Category    |
|--------------|----------------------------------------------------------------------------------------|-------------|
| PDF2WORD-5   | Process paragraph placed on two pages simultaneously as one paragraph, not as two ones | New feature |
| PDF2WORD-29  | Spaces missing in converting of certain doc                                            | Bug         |
| PDF2WORD-545 | Unexpected section breaks after every page because of colontitles                      | Bug         |
| PDF2WORD-549 | Many words are joined together on Windows                                              | Bug         |
| PDF2WORD-552 | Page numbers are recognized as normal text                                             | Bug         |
| PDF2WORD-571 | Footnotes refactoring                                                                  | Task        |
| PDF2WORD-574 | Unexpected table was detected                                                          | Bug         |
| PDF2WORD-577 | Footnote after space not detected                                                      | Bug         |
| PDF2WORD-580 | Adding a new item to a list after the first one breaks visual consistency              | Bug         |
| PDF2WORD-582 | Wrong paragraph split, incorrect carriage return detection                             | Bug         |
| PDF2WORD-583 | Wrong paragraph split due to list detection                                            | Bug         |
| PDF2WORD-584 | Wrong paragraph split due to textual cluster building                                  | Bug         |
| PDF2WORD-587 | Implement Case-Document-PageID pattern recognition in headers                          | Task        |
| PDF2WORD-588 | Implement i-ii-iii page number pattern recognition                                     | Task        |
| PDF2WORD-593 | Improve header pattern recognition for Rent-A-Center.pdf                               | Task        |
