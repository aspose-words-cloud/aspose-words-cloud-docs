---
title: "Aspose.Words Cloud 20.7 Release Notes"
type: docs
url: /release-notes/2020/20-7/
aliases: [/aspose-words-cloud-20-7-release-notes/]
weight: 20
---

The page contains release notes for Aspose.Words Cloud 20.7 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words

- Added "Markdown" save format

## PDF

- Corrected KeyNotFoundException and InvalidOperationException errors while loading a PDF
- Implemented first version of footnote detection
- Corrected recognition for page headers with image and text
- Fixed an ObjectDisposedException when PDF is loaded from a stream

## All changes

|ID|Summary|Category|
| :- | :- | :- |
|WORDSCLOUD-785|Add "Markdown" save format|Feature|
|WORDSCLOUD-852|Problem with ordered/unordered lists inside table|Bug|
|WORDSCLOUD-1187|UpdateParagraphFormat method fails with Internal Server Error|Bug|
|PDF2WORD-484 |Footnote detection |Story|
|PDF2WORD-503 |Incorrect text formatting in colontitle |Bug|
|PDF2WORD-507 |Metadata is missed in release dlls |Bug|
|PDF2WORD-513 |Remove duplicated methods CheckAndRetrieveParameters from PdfOperator descendant classes |Task|
|PDF2WORD-516 |Change parsing of operator BI (inline image) |Task|
|PDF2WORD-525 |Prepare new folder structure similar to ParagraphDetection in AccuracyEvaluation project |Task|
|PDF2WORD-531 |Error while processing a PDF file from a MemoryStream |Bug|
|PDF2WORD-533 |Prepare wiki documentation for table recognition workflow |Task|
|PDF2WORD-535 |PdfCCITTFaxDecodeFilter processing fails with an error |Bug|
|PDF2WORD-536 |CffEncodingParser fails to decode a Type 1 CFF font |Bug|
|PDF2WORD-537 |JBig2Decoder causes an OverflowException |Bug|
|PDF2WORD-538 |PdfPageTree class fails on IsTreeNode function |Bug|
|PDF2WORD-539 |Sign Pdf2Word release with the same certificate and key as Aspose.Words team does |Task|

## SDK Changes

## Aspose

- Added "Markdown" save format
- UpdateParagraphFormatRequest now takes ParagraphFormatUpdateDto
- ParagraphFormat's hierarchy changed: ParagraphFormatBase model was introduced and contains all common properties

## Aspose

- Added "Markdown" save format
- Added endpoint to update paragraph format without node path (PUT "/words/{name}/paragraphs/{index}/format")

