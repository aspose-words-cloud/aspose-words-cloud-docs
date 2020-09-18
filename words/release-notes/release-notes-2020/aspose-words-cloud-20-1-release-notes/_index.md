---
title: "Aspose.Words Cloud 20.1 Release Notes"
type: docs
url: /aspose-words-cloud-20-1-release-notes/
aliases: [/aspose-words-cloud-20-1-release-notes/]
weight: 70
---

## Important Changes and Enhancements
### API changes
1. Property "ColorMode" moved from SaveOptionsData to FixedPageSaveOptionsData
### PDF to Word conversion improvements
1. Corrected document layout on first saving;
1. Added recognition for ICC based color spaces from PDF documents;
1. Reduced the number of processing steps for PDF images (should improve processing time for some PDFs).
## All changes

|**Summary**|**Category**|
| :- | :- |
|Move property "**ColorMode**" from SaveOptionsData to FixedPageSaveOptionsData|Enhancement|
|Replace MemoryStream and byte[] with SixLabors.ImageSharp.IImage in image processing|Enhancement|
|Include support of ICC profiles and implement ICCBased color space|Enhancement|
|Pdf -> HtmlFixed conversion issue |Bug|
|` `ConvertDocument API: PDF to HTML conversion Issue|Bug|
|Test TableIsFoundCorrectlyByHeader fails on Linux |Bug|
|Sometimes a test fails with NullReferenceException |Bug|

