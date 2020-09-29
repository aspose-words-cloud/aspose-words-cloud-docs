---
title: "19.12 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2019/19-12/
aliases: [/aspose-words-cloud-19-12-release-notes/]
description: "Aspose.Words Cloud 19.12 Release Notes"
weight: 10
---

## Important Changes and New Features

## API

- Fixed issue with "borderType" parameter in "border" endpoints in swagger and SDKs
- Increased max size of uploaded files (now it is 100mb).

## PDF

- improved default font replacement logic;
- an OutOfMemory error doesn't occur on large documents anymore;
- added support for more color spaces (CalGrey, CalRGB, Lab).

## Bug

|WORDSCLOUD-960|Incorrect "borderType" parameter name in swagger|Bug|
| :- | :- | :- |
|WORDSCLOUD-992|Uploading a large file throws request body too large exception|Bug|

## Aspose.Words

- ColorMode property has been moved from SaveOptionsData to FixedPageSaveOptionsData
