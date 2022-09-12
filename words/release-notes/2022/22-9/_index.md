---
title: "22.9 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2022/22-9/
aliases: [/aspose-words-cloud-22-9-release-notes/]
description: "Aspose Words Cloud 22.9 Release Notes"
weight: 30
---

The page contains release notes for Aspose.Words Cloud 22.9 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Document compression method (`CompressDocument`) now supports working with images
- Document conversion API now supports working with password-protected documents


## PDF to Word conversion improvements

- Implemented recognition of a simple table of contents in an RTL document
- Fixed bugs when processing RTL text: improved the algorithm for determining the text direction, removed extra spaces
- Fixed a bug when processing `CustomDocumentProperties` during PDF conversion


## Cloud SDK Changes

- `ConvertDocumentRequest` now has 3 new properties:
  - `LoadEncoding` - encoding that will be used to load the HTML (or TXT) document if the encoding is not specified in the HTML
  - `Password` - password for the protected Word document (the SDK encrypts it automatically)
  - `EncryptedPassword` - password for the protected Word document in encrypted form. Use the parameter to pass an encrypted password to direct API calls
- `CompressDocument` method now supports working with images

## All changes

| #               | Summary                                                                                              | Category |
|-----------------|------------------------------------------------------------------------------------------------------|----------|
| WORDSCLOUD-2058 | AppendDocument API: content is appended to the last page of a previous document, instead of starting on a new page | Bug      |
| WORDSCLOUD-2059 | Implement password-protected document conversions using the ConvertDocument API                      | Feature  |
| WORDSCLOUD-2093 | Implement support for images in `CompressDocument` method                                            | Feature  |
| WORDSNET-24063  | After PDF import, RTL table of contents is corrupted                                                 | Bug      |
| WORDSNET-24062  | After PDF import, RTL content is reversed and contains extra spaces                                  | Bug      |
| WORDSNET-24199  | `ArgumentException` is thrown due to an empty key in `CustomDocumentProperties`                      | Bug      |
| WORDSNET-23174  | `LibTiff` library throws `IndexOutOfRangeException`                                                  | Bug      |