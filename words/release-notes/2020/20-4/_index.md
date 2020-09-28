---
title: "20.4 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2020/20-4/
aliases: [/aspose-words-cloud-20-4-release-notes/]
description: "Aspose Words Cloud 20.4 release notes"
weight: 50
---

The page contains release notes for Aspose.Words Cloud 20.4 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and Enhancements

## Words

- Added CompareOptions to "Compare documents" endpoint
- Added "Password" option to OdtSaveOptions
- Added "Dml3DEffectsRenderingMode" to SaveOptions
- Added "InterpolateImages" option to PdfSaveOptions
- Added "UpdateLastPrintedProperty" to SaveOptions
- Added "UseTargetMachineFonts" option to HtmlFixedSaveOptions

## PDF

- Fixed all issues related to Xamarin support;
- Improved formulas formatting when font substitution occurs during the recognition;
- Got better bookmark detection when running on Linux;
- Corrected vector lines position and alignment with text on Linux.

## All changes

|#|Summary|Category|
| :- | :- | :- |
|WORDSCLOUD-279|Add "UseTargetMachineFonts" option to HtmlFixedSaveOptions Data |Feature|
|WORDSCLOUD-422|Add "Password" option to OdtSaveOptions |Feature|
|WORDSCLOUD-671|Provision of Compare Options in Aspose.Words Cloud |Feature|
|WORDSCLOUD-1060|Add new SaveOptionsData.UpdateLastPrintedProperty |Feature|
|WORDSCLOUD-1131|Add new Saveoption Dml3DEffectsRenderingMode |Feature|
|WORDSCLOUD-1132|Add new PdfSaveOption "InterpolateImages" |Feature|
|WORDSCLOUD-1099|EOF error if APP KEY is incorrect |Bug|
|WORDSCLOUD-1129|DrawingObjects API response includes unsecured Href |Bug|
|PDF2WORD-135 |Slow processing on some files |Bug|
|PDF2WORD-412 |Wrong formulas formatting |Bug|
|PDF2WORD-425 |TestRecognizingTextWithBookmarks fails on Linux |Bug|
|PDF2WORD-429|TestDocument_CorrectResult_BothHeadersAndFooters fails on Linux|Bug|
|PDF2WORD-460|TableDetector doesn't recognize a colored table|Bug|
|PDF2WORD-469|Table doesn't fit it's border|Bug|
|PDF2WORD-470 |Some vector lines aren't visible on the chart|Bug|
|PDF2WORD-476 |Pdf2Word plugin doesn't work with Xamarin (Mac, Android, iOS) |Bug|
|PDF2WORD-458 |Research possible Aspose.Drawing usage in PDF2Word project |Task|
|PDF2WORD-471 |Enable case-sensitive Git for project's repository (cancelled) |Task|
|PDF2WORD-480 |Test Live Share feature in Visual Studio 2019 |Task|
|PDF2WORD-481|Integrate StyleCop and Cloud style rules|Task|
|PDF2WORD-482 |Migrate Pdf2Word projects to VS 2019, C# 8 and .NET Core 3.1 |Task|

## SDK Changes

1. 'rangeEndIdentifier' now non-required for all SDKs, just like NET SDK.
2. The same order of parameters in the modelRequests for all SDKs.
3. Added CompareOptions property to CompareData class
4. Added Password property to OdtSaveOptions class
5. Added Dml3DEffectsRenderingMode property to SaveOptions class
6. Added UpdateLastPrintedProperty property to SaveOptions class
7. Added InterpolateImages property to PdfSaveOptions class
8. Added UseTargetMachineFonts property to HtmlFixedSaveOptions class
9. Added some request data classes: 
   - RunUpdate and RunInsert
   - FootnoteUpdate and FootnoteInsert
   - FieldUpdate and FieldInsert
   - CommentUpdate and CommentInsert
   - DocumentPropertyCreateOrUpdate
