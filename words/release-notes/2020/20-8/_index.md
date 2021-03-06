---
title: "20.8 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2020/20-8/
aliases: [/aspose-words-cloud-20-8-release-notes/]
description: "Aspose Words Cloud 20.8 Release Notes"
weight: 11
---

The page contains release notes for Aspose.Words Cloud 20.8 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words

- Added "optimize document" feature
- Added '**ApplyBaseDocumentHeadersAndFootersToAppendingDocuments**' option to '**DocumentEntryList**' for **AppendDocument** API
- **WithoutNodePath** methods were removed from SDKs

## PDF

- Improved header/footer detection by removing false candidates
- Corrected multiple issues with footnotes recognition (numbers, alignment, continuation, etc)
- Reduced memory allocations for PDFs with big images (10 times less now)
- Fixed page height calculation that was causing empty output document
- Supported more formats in numbered list detection
- Removed false one element lists from table cells
- Fixed a couple of PDF processing errors
- Created a new option that allows skipping all images from a PDF
- Changed obfuscation settings for fix iOS compatibility

## All changes

|ID|Summary|Category|
| :- | :- | :- |
|WORDSCLOUD-1206|UpdateField API unable to find TOC field and update|Bug|
|WORDSCLOUD-1230|Convert ODT to TXT with SaveAs API throws Index was outside the bounds of the array error|Bug|
|WORDSCLOUD-1242|Stop adding headers and footers from destination document to source document|Bug|
|WORDSCLOUD-1258|DOC to TXT conversion throws internalError Error while loading file|Bug|
|WORDSCLOUD-1267|Fonts being changed converting from Word to PDF|Bug|
|WORDSCLOUD-1235|How to optimize Word document for Word 2016|Feature|
|PDF2WORD-532 |Excessive section breaks as a result of incorrect footer detection |Bug|
|PDF2WORD-541 |Footnotes without a number are not recognized |Bug|
|PDF2WORD-542 |Two numbered footnotes were not recognized |Bug |
|PDF2WORD-551 |Wrong footnotes alignment in one document |Bug|
|PDF2WORD-553 |Heavy memory usage on Searchable PDFs from the customer |Bug|
|PDF2WORD-554|Negative page height causes all elements to be skipped during the recognition|Bug|
|PDF2WORD-562 |List detection doesn't work properly on a customer's file |Bug|
|PDF2WORD-563 |Destination reference error stops PDF processing |Bug|
|PDF2WORD-564 |FileLoadException happens because of PdfTokenParser can't read big numbers |Bug|
|PDF2WORD-347 |PdfParser refactoring|Task|
|PDF2WORD-514|Simplify usage of PdfStreamProvider class|Task|
|PDF2WORD-515 |Refactoring of class PdfContentProcessor |Task|
|PDF2WORD-558|Use new flag to skip all image processing methods when requested|Task|
|PDF2WORD-561|Change obfuscation settings to fix iOS compatibility|Task|

## SDK Changes

## Aspose

- Added new api method

```JAVA
{name}/compatibility/optimize
```

which is allows to optimize the document contents as well as default Aspose.Words behavior to a particular versions of MS Word

- Added '**ApplyBaseDocumentHeadersAndFootersToAppendingDocuments**' option to '**DocumentEntryList**' for **AppendDocument** API

