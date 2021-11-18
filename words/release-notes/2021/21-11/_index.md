---
title: "21.11 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-11/
aliases: [/aspose-words-cloud-21-11-release-notes/]
description: "Aspose Words Cloud 21.11 Release Notes"
weight: 20
---

The page contains release notes for Aspose.Words Cloud 21.11 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- "/info" endpoint is added to the Docker hub to access API usage details
- Various bug fixes and improvements

## PDF to Word conversion improvements

- Fixed `InvalidCastException` when a PDF reference is written in lower case format
- Improved handling of non-existent PDF elements to avoid `InvalidOperationException` and `ArgumentOutOfRangeException`
- Limited the maximum value of table line width to avoid `ArgumentOutOfRangeException`
- Fixed `NullReferenceException` in `CffEncodingData.Parser` logic (embedded font parameters)
- Added support for PDF documents without indirect references to `Info` section (which is required by PDF format spec)

## All changes

| #               | Summary                                                                                       | Category    |
|-----------------|-----------------------------------------------------------------------------------------------|-------------|
| WORDSCLOUD-1589 | Python SDK. Implement the `dependsOn` parameter in batch requests 	                          | New Feature |
| WORDSCLOUD-1812 | Provide access to API usage details for Aspose.Words Docker Container                         | New Feature |
| WORDSCLOUD-1608 | Errors when using Aspose.Words Cloud API from Scala + `sbt`                                   | Bug         |
| WORDSCLOUD-1762 | Invalid unit test for `WORDSCLOUD-1547` task                                                  | Bug         |
| WORDSCLOUD-1785 | Nested JSON objects lead to an error in LINQ Reporting Engine                                 | Bug         |
| WORDSCLOUD-1817 | Thread synchronization error in Node.js SDK                                                   | Bug         |
| PDF2WORD-910    | `InvalidCastException`: Unable to cast object of type `PdfInteger` to type `PdfName`          | Bug         |
| PDF2WORD-912    | `ArgumentOutOfRangeException`: Attempt to reference non-existent PDF object (parameter `internalObjNumber`) | Bug |
| PDF2WORD-913    | `InvalidOperationException`: Could not find object with #57 and generation number 0             | Bug         |
| PDF2WORD-927    | `InvalidOperationException`: Resource with a given name is not contained in the page resources  | Bug         |
| PDF2WORD-930    | `ArgumentOutOfRangeException`: Specified argument was out of the range of valid values (parameter `lineWidth`) | Bug |
| PDF2WORD-932    | `NullReferenceException` at `CffEncodingData.Parse`                                           | Bug         |
| PDF2WORD-939    | `InvalidOperationException`: Info element in the trailer dictionary must be Indirect object   | Bug         |

