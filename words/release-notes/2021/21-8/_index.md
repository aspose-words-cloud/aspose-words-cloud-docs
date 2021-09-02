---
title: "21.8 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2021/21-8/
aliases: [/aspose-words-cloud-21-8-release-notes/]
description: "Aspose Words Cloud 21.8 Release Notes"
weight: 40
---

The page contains release notes for Aspose.Words Cloud 21.8 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Words Cloud Changes

- Implemented several API methods to get, insert, update and delete custom XML parts from documents
- Added a new parameter to the 'Comparison' API (`ResultDocumentFormat`)

## PDF to Word conversion improvements

- Fixed a `ZlibException` caused by extra spaces in `FlateDecode` PDF streams
- Fixed a `ZlibException` caused by data streams with incorrect checksums (some PDF software doesn't follow the specification)
- Fixed an `InvalidOperationException` related to PDF filter processing
- Fixed an `InvalidOperationException` appeared as "Operator should take 1 operand" message

## All changes

| #               | Summary                                                                                       | Category |
|-----------------|-----------------------------------------------------------------------------------------------|----------|
| PDF2WORD-810    | Thin lines are processed as separate paragraphs                                               | Bug      |
| PDF2WORD-811    | Incorrect image position                                                                      | Bug      |
| PDF2WORD-817    | `ZlibException`: Bad state (unknown compression method (0x20))                                | Bug      |
| PDF2WORD-821    | `InvalidOperationException`: Operator should take 1 operands                                  | Bug      |
| PDF2WORD-844    | The contents of a page is mistakenly shifted when column detection is enabled                 | Bug      |
| PDF2WORD-847    | `InvalidOperationException`: Filter entry of stream object must be either PDF name or PDF Array | Bug    |
| PDF2WORD-855    | Implement the ability to specify footer distance                                              | Task     |
| PDF2WORD-856    | `ZlibException`: Bad state (incorrect data check)                                             | Bug      |