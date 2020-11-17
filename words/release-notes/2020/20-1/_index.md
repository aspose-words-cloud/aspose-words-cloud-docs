---
title: "20.1 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2020/20-1/
aliases: [/aspose-words-cloud-20-1-release-notes/]
description: "Aspose Words Cloud 20.1 Release Notes"
weight: 70
---

## Important Changes and Enhancements

## API

- Property "ColorMode" moved from SaveOptionsData to FixedPageSaveOptionsData

## PDF

- Corrected document layout on first saving;
- Added recognition for ICC based color spaces from PDF documents;
- Reduced the number of processing steps for PDF images (should improve processing time for some PDFs).

## All changes

|Summary|Category|
| :- | :- |
|Move property "**ColorMode**" from SaveOptionsData to FixedPageSaveOptionsData|Enhancement|
|Replace MemoryStream and byte[] with SixLabors.ImageSharp.IImage in image processing|Enhancement|
|Include support of ICC profiles and implement ICCBased color space|Enhancement|
|Pdf -> HtmlFixed conversion issue |Bug|
|` `ConvertDocument API: PDF to HTML conversion Issue|Bug|
|Test TableIsFoundCorrectlyByHeader fails on Linux |Bug|
|Sometimes a test fails with NullReferenceException |Bug|

