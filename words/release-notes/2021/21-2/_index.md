---
title: "21.2 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-2/
aliases: [/aspose-words-cloud-21-2-release-notes/]
description: "Aspose Words Cloud 21.2 Release Notes"
weight: 65
---

The page contains release notes for Aspose.Words Cloud 21.2 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Added method to remove all comments inside document
- Added `AllowEmbeddingPostScriptFonts` option

## PDF to Word conversion improvements

- Optimized processing of large PDF images (reduced time and peak memory usage)
- Removed requirement for a few PDF markers (some PDF producers don’t follow the spec)
- Fixed decoding of child resources inside page resource dictionaries
- Corrected an issue with images been lost if a PDF page size is too large (added downscaling to the allowed MS Word limits)
- Improved image comparison in `ColontitleDetector` logic to avoid getting wrong images in header/footer areas
- Added protection against duplicate values that embedded CFF fonts might have on rare occasions
- Fixed two issues in header/footer detection related to element positioning
- Finished rework of footnote processing logic to support RTL text properly
- Corrected alignment of text lines that have both RTL and LTR words

## All changes

| #               | Summary                                                                                       | Category    |
|-----------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1477 | Add methods for removing all comments in a document                                           | Feature     |
| WORDSCLOUD-1443 | Add `AllowEmbeddingPostScriptFonts` option to `SaveOptions`                                   | Feature     |
| WORDSCLOUD-1320 | Swagger misses parameter order when sending multipart request                                 | Bug         |
| WORDSCLOUD-1451 | OpenXPS file format error in Swagger UI                                                       | Bug         |
| WORDSCLOUD-1285 | Swagger can't send value in field if it contains `:`                                          | Bug         |
| WORDSCLOUD-1286 | Swagger adds `,` to some fields if you didn't specify them                                    | Bug         |
| WORDSCLOUD-1306 | Issue with the forward slash directory separator in Swagger UI                                | Bug         |
| WORDSCLOUD-1452 | PostScript file format conversion error in Swagger UI                                         | Bug         |
| PDF2WORD-69     | Support Arabic writing                                                                        | Feature     |
| PDF2WORD-613    | Support PDF pages with colored background                                                     | Feature     |
| PDF2WORD-619    | RTL footnotes are not recognized                                                              | Bug         |
| PDF2WORD-652    | Incorrect text direction of bidirectional text                                                | Bug         |
| PDF2WORD-653    | Hebrew text is moved on the second line because of extra spaces                               | Bug         |
| PDF2WORD-677    | "An item with the same key has already been added" in `ParseMainEncodingFormat0`              | Bug         |
| PDF2WORD-681    | `IndexOutOfRangeException` happened on several PDFs                                           | Bug         |
| PDF2WORD-685    | Footer detection issues                                                                       | Bug         |
| PDF2WORD-687    | PDF font dictionary must contain a `/Type` - `/Font` key-value pair                           | Bug         |
| PDF2WORD-688    | Context is not set. Set a valid `PdfResourceDictionary` instance as Context for `Do` operator | Bug         |
| PDF2WORD-689    | Cannot cast `PdfIndirectObjectReference` to `PdfDictionary`                                   | Bug         |
| PDF2WORD-690    | `OutOfMemoryException` while processing large images from PDFs                                | Bug         |
| PDF2WORD-693    | Horizontal lines are not recognized as part of footers                                        | Bug         |
| PDF2WORD-694    | Spacing is lost between Icon and `PAGE` field code in a footer                                | Bug         |
| PDF2WORD-695    | Slow processing for PDF with large images                                                     | Bug         |
| PDF2WORD-696    | The image is not visible after the `Pdf2Word` conversion                                      | Bug         |
| PDF2WORD-698    | Scan images were detected as a header picture by mistake                                      | Bug         |
