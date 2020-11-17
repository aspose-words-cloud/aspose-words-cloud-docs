---
title: "20.10 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2020/20-10/
aliases: [/aspose-words-cloud-20-10-release-notes/]
description: "Aspose Words Cloud 20.10 Release Notes"
weight: 10
---

The page contains release notes for Aspose.Words Cloud 20.10 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Various fixes and improvements

## PDF to Word conversion improvements

- Reduced amount of the wrong paragraph splits by improving text line comparison logic
- Reworked page numbering detection to support more patterns and number formats (including Roman numerals)
- Improved space size calculation to correct the reported issues with words joined together
- Removed redundant paragraph breaks caused by footnote references
- Fixed the spacing in lists after the first item
- Implemented the first iteration of paragraph joining logic between adjacent pages (a similar change for lists will be made later)

## All changes

| #               | Summary                                                                                       | Category    |
|-----------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-588  | HTML to Word (DOCX) Conversion. Table data is truncated                                       | Bug         |
| WORDSCLOUD-591  | HTML to Word Conversion. Public Image hosted on Client Server is missing in the Output Word   | Bug         |
| WORDSCLOUD-811  | DOCX to PDF Conversion issue with SaveAs API method                                           | Bug         |
| WORDSCLOUD-1006 | Statistics API is throwing 502 Bad Gateway                                                    | Bug         |
| WORDSCLOUD-1007 | Numbering list alignment issue in HTML to DOCX Conversion                                     | Bug         |
| WORDSCLOUD-1231 | GetDocumentStatistics throwing Object reference not set to an instance of an object exception | Bug         |
| WORDSCLOUD-1262 | GetDocumentStatistics is throwing error a value with the specified key has already been added | Bug         |
| WORDSCLOUD-1271 | GetDocumentStatistics is throwing object reference not set error                              | Bug         |
| WORDSCLOUD-1272 | Split API method throws GlossaryDocument Error                                                | Bug         |
| WORDSCLOUD-1273 | Split API Method unable to load Word document                                                 | Bug         |
| WORDSCLOUD-1274 | GetDocumentStatistics API is unable to load Word document                                     | Bug         |
| WORDSCLOUD-1276 | SplitDocument API Method is throwing Object Reference error                                   | Bug         |
| WORDSCLOUD-1278 | GetDocumentStatistics API is throwing cannot insert a not this type error                     | Bug         |
| WORDSCLOUD-1279 | GetDocumentStatistics API is throwing GDI+ error                                              | Bug         |
| WORDSCLOUD-1280 | SplitDocument API is throwing GDI+ error                                                      | Bug         |
| WORDSCLOUD-1281 | ODT to TXT conversion issue with SaveAs API                                                   | Bug         |
| WORDSCLOUD-1284 | Split API is throwing Object not set error while splitting Word to HTML                       | Bug         |
| WORDSCLOUD-1289 | SaveAs API is throwing Object reference error                                                 | Bug         |
| WORDSCLOUD-1310 | Split Document API is throwing duplicate attribute name error                                 | Bug         |
| WORDSCLOUD-1311 | Split API is throwing Buildingblocks error                                                    | Bug         |
| WORDSCLOUD-1312 | SplitDocument API is throwing Overflow error for a big Word Document                          | Bug         |
| WORDSCLOUD-1314 | SaveAs API Method is throwing Object reference not set error                                  | Bug         |
| WORDSCLOUD-1315 | SaveAs API is throwing not supported structured storage version                               | Bug         |
| WORDSCLOUD-1316 | ODT to TXT conversion document loading issue                                                  | Bug         |
| WORDSCLOUD-1322 | Append Document API is throwing error while loading file exception                            | Bug         |
| WORDSCLOUD-1346 | DeleteMacros API throwing image file saving error                                             | Bug         |
| WORDSCLOUD-1353 | Text alignment difference in HTML to DOCX conversion between 20.7 and 20.9                    | Bug         |
| WORDSCLOUD-1354 | HTML to DOCX conversion issue with the numbering list inside HTML table                       | Bug         |
| WORDSCLOUD-1355 | HTML to DOCX content misalignment                                                             | Bug         |
| WORDSCLOUD-1356 | Section numbering disappears on HTML to DOCX conversion                                       | Bug         |
| WORDSCLOUD-1359 | Unterminated string. Expected delimiter exception when call batch request                     | Bug         |
| WORDSCLOUD-1363 | CreateFolder method in PHP SDK throwing 500 Error connecting to the API                       | Bug         |
| WORDSCLOUD-1380 | getDocumentDrawingObjects API regression issue in Aspose.Word Cloud SDK for Node.js           | Bug         |
| WORDSCLOUD-1389 | Regression: SplitDocument API is overwriting all output pages with the first page of the input document | Bug |
| WORDSCLOUD-1390 | PHP SDK File Upload throwing 400                                                              | Bug         |
| PDF2WORD-5      | Process paragraph placed on two pages simultaneously as one paragraph, not as two ones        | New feature |
| PDF2WORD-29     | Spaces missing in converting of certain doc                                                   | Bug         |
| PDF2WORD-545    | Unexpected section breaks after every page because of Headers/Footers                         | Bug         |
| PDF2WORD-549    | Many words are joined together on Windows                                                     | Bug         |
| PDF2WORD-552    | Page numbers are recognized as normal text                                                    | Bug         |
| PDF2WORD-571    | Footnotes refactoring                                                                         | Task        |
| PDF2WORD-574    | Unexpected table was detected                                                                 | Bug         |
| PDF2WORD-577    | Footnote after space not detected                                                             | Bug         |
| PDF2WORD-580    | Adding a new item to a list after the first one breaks visual consistency                     | Bug         |
| PDF2WORD-582    | Wrong paragraph split, incorrect carriage return detection                                    | Bug         |
| PDF2WORD-583    | Wrong paragraph split due to list detection                                                   | Bug         |
| PDF2WORD-584    | Wrong paragraph split due to textual cluster building                                         | Bug         |
| PDF2WORD-587    | Implement Case-Document-PageID pattern recognition in headers                                 | Task        |
| PDF2WORD-588    | Implement i-ii-iii page number pattern recognition                                            | Task        |
| PDF2WORD-593    | Improve header pattern recognition for Rent-A-Center.pdf                                      | Task        |
