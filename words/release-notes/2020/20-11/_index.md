---
title: "20.11 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2020/20-11/
aliases: [/aspose-words-cloud-20-11-release-notes/]
description: "Aspose Words Cloud 20.11 Release Notes"
weight: 9
---

The page contains release notes for Aspose.Words Cloud 20.11 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Dart SDK released
- Added support for "PageBreaks" in XML responses and in search requests
- Fixed authorization error when call batch sub-requests

## PDF to Word conversion improvements

- Fixed `IndexOutOfRangeException` caused by wrong color index calculation
- Corrected list items positioning when numerals are Roman
- Fixed text size calculation and spacing for a specific case with text matrices
- Increased performance of JBIG2 image decoding
- Implemented proper footnotes auto numbering
- Finished first version of the typo fixer that is currently used to repair text in Searchable PDFs produced by OmniPage Capture SDK
- Corrected position of text cells when tables are placed inside text blocks
- Removed wrong right margin in paragraphs with a single line of text
- Supported "X/Y" page numbering format in headers and footers
- Corrected additional issues with text lines not joining into paragraphs
- Implemented Indexed to RGB color mapping to repair pixel color conversion of some images
- Reduced long spacing between words happened after font replacement
- Added first parts of logic required for Right-to-Left text support


## All changes

| #               | Summary                                                                       | Category    |
|-----------------|-------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1384 | Authorization error when call batch sub-requests                              | Bug         |
| WORDSCLOUD-1395 | PDF to HTML conversion throws the file cannot be opened                       | Bug         |
| WORDSCLOUD-1415 | Get Runs with XML response type throws exception on page breaks               | Bug         |
| WORDSCLOUD-1418 | Search does not support control characters in search templates                | Bug         |
| PDF2WORD-323    | A list with Roman numerals has incorrect layout after the conversion          | Bug         |
| PDF2WORD-534    | Very poor conversion results for one looking normal PDF                       | Bug         |
| PDF2WORD-540    | Slow decoding for PDFs with JBig2 images                                      | Bug         |
| PDF2WORD-569    | New footnote number starts with 1 in recognized DOCX file                     | Bug         |
| PDF2WORD-573    | Special characters are not recognized in Word doc                             | Bug         |
| PDF2WORD-575    | Cell values incorrectly located outside of a table                            | Bug         |
| PDF2WORD-592    | Footnote reference is not recognized as superscript                           | Bug         |
| PDF2WORD-596    | Incorrect text width caused incorrect paragraph formatting                    | Bug         |
| PDF2WORD-597    | Text lines don't join on JMemo documents                                      | Bug         |
| PDF2WORD-598    | Pages numbers aren't recognized in "X/Y" format                               | Bug         |
| PDF2WORD-599    | Wrong paragraph merging                                                       | Bug         |
| PDF2WORD-600    | Generate correct Bidi settings for RTL text blocks                            | Task        |
| PDF2WORD-601    | Read RTL text properties from PDFs                                            | Task        |
| PDF2WORD-605    | Fix `scn` operator processing to avoid getting `IndexOutOfRangeException`     | Bug         |
| PDF2WORD-608    | Increase PDF name buffer to 127 bytes                                         | Task        |
| PDF2WORD-609    | Two pages with images are filled with black instead of white                  | Bug         |
| PDF2WORD-610    | Long spaces between words make user editing very difficult                    | Bug         |
