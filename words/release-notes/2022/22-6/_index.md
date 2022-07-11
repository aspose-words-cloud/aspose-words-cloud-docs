---
title: "22.6 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2022/22-6/
aliases: [/aspose-words-cloud-22-6-release-notes/]
description: "Aspose Words Cloud 22.6 Release Notes"
weight: 45
---

The page contains release notes for Aspose.Words Cloud 22.6 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Bookmarks API: added 'DeleteBookmark' and 'DeleteBookmarkOnline' methods to remove a bookmark specified by name from a document
- Bookmarks API: added 'DeleteBookmarks' and 'DeleteBookmarksOnline' methods to remove all bookmarks from a document
- Bookmarks API: added 'InsertBookmark' and 'InsertBookmarkOnline' methods to create new bookmarks in a document
- The 'Create Document' endpoint now supports all file formats supported by Aspose.Words


## PDF to Word conversion improvements

- Fixed rare infinite loop in Word layout recalculation logic
- Improved table candidates detection by supporting smaller tables and filtering incorrect table lines
- Handled missing characters in Unicode maps differently to avoid getting long spaces in output documents
- Supported unusual PDF images that store pixel data in their image masks
- Added a workaround for incorrect hex numbers in Unicode character mapping tables

## Cloud SDK Changes

- **All SDKs**:
    - Bookmarks API: added methods to remove a bookmark specified by name from a document
    - Bookmarks API: added methods to remove all bookmarks from a document
    - Bookmarks API: added methods to create new bookmarks in a document
    - Added support for all save formats for the 'CreateDocument' operation

- **Ruby SDK**:
    - Added support for the 'dependsOn' feature in batch requests


## All changes

| #               | Summary                                                                                                          | Category    |
|-----------------|------------------------------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-455  | Added support for calling Aspose.Words APIs asynchronously so the client doesn't need to keep the thread waiting | New Feature |
| WORDSCLOUD-1225 | Implemented the ability to reuse a header/footer from a template Word document in another document               | New Feature |
| WORDSCLOUD-2010 | Bookmarks API: implement new methods for inserting and deleting bookmarks in a document                          | New Feature |
| WORDSCLOUD-2007 | Remove obsolete `ExportTextBoxAsSvg` property, add `ExportShapesAsSvg` property                                  | New Feature |
| WORDSCLOUD-1956 | `NullReferenceException` during DOCX to PDF conversion                       | Bug         |
| WORDSCLOUD-1957 | Formatting issue when converting PDF to DOCX                                 | Bug         |
| WORDSCLOUD-2009 | API for updating bookmarks does not change bookmark names                    | Bug         |
| WORDSCLOUD-2011 | Unexpected result when replacing multiple strings in a document using a batch request  | Bug         |
| WORDSNET-23035  | `InvalidOperationException`: Infinite loop detected                          | Bug         |
| WORDSNET-23613  | Table formatting is destroyed during PDF to DOCX conversion                  | Bug         |
| WORDSNET-23808  | Separator elements are erroneously added instead of spaces during the `Pdf2Word` conversion | Bug         |
| WORDSNET-23809  | Images with text are corrupted during the `Pdf2Word` conversion              | Bug         |
| WORDSNET-23813  | `InvalidOperationException`: Failed to find the start of the hex number      | Bug         |
