---
title: "20.3 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2020/20-3/
aliases: [/aspose-words-cloud-20-3-release-notes/]
description: "Aspose Words Cloud 20.3 release notes"
weight: 60
---

## Important Changes and Enhancements

## API

- Added RtfSaveOptionsData.SaveImagesAsWmf property
- Added SDK for Swift
- Added SDK for Go
- PHP SDK. From now in packagist sdk has different package name aspose-words-cloud [new link here](https://packagist.org/packages/aspose-cloud/aspose-words-cloud).
  Old package is abandoned and no more updated since this release [ABANDONED package](https://packagist.org/packages/aspose/words-sdk-php).

## PDF

- Improved space detection between words in text paragraphs;
- Fixed position in text for images rotated by 45 degrees;
- Corrected PDF header recognition while checking file format;
- Fixed a blur effect for images encoded with ICC profiles;
- Adjusted text position and alignment on Linux;
- Improved line endings detection for text lines;
- Table cell size calculation was slightly updated.

## All changes

|#|Summary|Category|
| :- | :- | :- |
|WORDSCLOUD-549|Swift Cloud SDK |Feature|
|WORDSCLOUD-984|Go Cloud SDK |Feature|
|WORDSCLOUD-1004|Add new RtfSaveOption.SaveImagesAsWmf |Feature|
|WORDSCLOUD-1038|API V1 GetParagraphs not working for files greater than 5mb |Bug|
|WORDSCLOUD-1040|ExecuteMailMerge API region option issue |Bug|
|WORDSCLOUD-1061|GetFilesList method returns dates in inconsistent format |Bug|
|WORDSCLOUD-1072|Authentication Failures after 24hrs |Bug|
|WORDSCLOUD-1093 |Word files Upload failing and throwing unexpected error |Bug|
|PDF2WORD-328 |Integrate PDF2Word plugin with Aspose.Words package |Feature|
|PDF2WORD-402 |Fix lines endings in unexpected places |Task|
|PDF2WORD-403 |Wrong single line position in output png|Bug|
|PDF2WORD-404|Wrong text position inside vector images in output png on Linux|Bug|
|PDF2WORD-405 |Space length is too big |Bug|
|PDF2WORD-406 |Wrong paragraphs indent|Bug|
|PDF2WORD-407 |Line endings in unexpected places |Bug|
|PDF2WORD-408 |Text could not be fully visible inside table cells |Bug|
|PDF2WORD-409 |Wrong charts positioning |Bug|
|PDF2WORD-410 |Text overlaying for multicolumn layouts |Bug|
|PDF2WORD-413|Similar output files have pixel diffs in golds on Linux |Bug|
|PDF2WORD-414 |Text could not be fully displayed inside graphical elements on Linux |Bug|
|PDF2WORD-415 |SearchablePdf_WithTextBehindImages_MustNotHaveDuplicatedText fails on Linux |Bug|
|PDF2WORD-418 |Wrong text wrapping |Bug|
|PDF2WORD-419 |Wrong rotated and flipped image positions |Bug |
|PDF2WORD-421 |Missing font error in unit tests on Linux |Bug|
|PDF2WORD-422 |TestSimpleHighlightedGlyphs fails with null reference exception |Bug|
|PDF2WORD-423 |Paragraph alignment tests fail on Linux |Bug|
|PDF2WORD-424 |TestRecognizingOneSimpleParagraph fails on Linux |Bug|
|PDF2WORD-431 |FileNotFoundException errors. |Bug|
|PDF2WORD-461|Logo image from a document recognized as white noise|Bug|
|PDF2WORD-462 |Text block groupping doesn't work properly after font replacement |Bug|
|PDF2WORD-463 |Incorrect division to words and too big spaces in the text strings |Bug|
|PDF2WORD-464 |Reduce build time on GitLab for master commits |Task|
|PDF2WORD-465 |Single lines have wrong position and overlap nearby text |Bug|
|PDF2WORD-467 |Large whitespace gaps which break words inside of text flow. |Bug|
|PDF2WORD-468 |Incorrect text alignment on Linux |Bug|
|PDF2WORD-472 |Can't open a couple Chinese PDFs because they have unexpected file header |Bug |
|PDF2WORD-478 |Wrong formulas block alignment in Appendix_C_CITables docx |Bug|
|PDF2WORD-479 |Different Golds for 2018_blueprint.pdf on dev PCs and GitLab |Bug|

## SDKs Changes

## Aspose

- XmlColor.Alpha isn't a required property
- RtfSaveOptionsData.SaveImageAsWmf property is added

## Aspose

- Alpha property of XmlColor class isn't a required now
- SaveImageAsWmf property is added to RtfSaveOptionsData class.

## Aspose

- XmlColor.Alpha isn't a required property
- RtfSaveOptionsData.SaveImageAsWmf property is added

## Aspose

- Added RtfSaveOptionsData.SaveImagesAsWmf property
- WordsApi class now has credentials parameters
- Methods which used to work with File now work with byte[]

## ` `Aspose

- XmlColor.Alpha isn't a required property
- RtfSaveOptionsData.SaveImageAsWmf property is added

## Aspose

- Added RtfSaveOptionsData.SaveImagesAsWmf property
- WordsApi class now has credentials parameters

## Important

From now in packagist sdk has different package name aspose-words-cloud [new link here](https://packagist.org/packages/aspose-cloud/aspose-words-cloud).
Old package is abandoned and no more updated since this release [ABANDONED package](https://packagist.org/packages/aspose/words-sdk-php).

## Aspose

- Added RtfSaveOptionsData.SaveImagesAsWmf property
- WordsApi class now has credentials parameters
- All methods which are used files, now operate with bytes array

## ` `Aspose

- Added RtfSaveOptionsData.SaveImagesAsWmf property
- WordsApi class now has credentials parameters

