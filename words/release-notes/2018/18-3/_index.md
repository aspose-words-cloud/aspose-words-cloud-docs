---
title: "Aspose.Words for Cloud 18.3 Release Notes"
type: docs
url: /release-notes/2018/18-3/
aliases: [/aspose-words-for-cloud-18-3-release-notes/]
weight: 90
---

The page contains release notes for Aspose.Words for Cloud update 18.3 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

#### Hyperlinks support for PDF to Word conversion

PDF to Word converter now properly converts style and destination of hyperlinks, both to URLs and local files.

## Cloud SDK Family

All currently [supported cloud SDKs](https://github.com/aspose-words-cloud) (.NET, PHP and Node.js) now have "Version" property for API Configuration classes. The attribute allows to target specific version. Supported versions are:

- v1 (default) - updated on monthly basis or more frequent
- v2 (stable) - updated once a quater
- v3 (frozen) - previous version of "stable", updated once a quater

#### Dropping support of deprecated PDF save option properties

Some PDF save options that have been deprecated in Aspose.Words .NET are now not available in Aspose.Words Cloud REST API as well. Full list of properties is as follows:

|Removed property|Property to use instead|
| :- | :- |
|PdfSaveOptions.HeadingsOutlineLevels|PdfSaveOptions.OutlineOptions.HeadingsOutlineLevels|
|PdfSaveOptions.ExpandedOutlineLevels|PdfSaveOptions.OutlineOptions.ExpandedOutlineLevels|
|PdfSaveOptions.BookmarksOutlineLevel|PdfSaveOptions.OutlineOptions.DefaultBookmarksOutlineLevel|
|PdfSaveOptions.EmbedStandardWindowsFonts|PdfSaveOptions.FontEmbeddingMode|
|PdfSaveOptions.ExportCustomPropertiesAsMetadata|PdfSaveOptions.CustomPropertiesExport|
|PdfSaveOptions.MetafileRenderingMode|PdfSaveOptions.MetafileRenderingOptions.RenderingMode|
|PdfSaveOptions.DownsampleImages|PdfSaveOptions.DownsampleOptions.DownsampleImages|
|PdfSaveOptions.DownsampleResolution|PdfSaveOptions.DownsampleOptions.Resolution|

See [Aspose.Words .NET 18.3 Release Notes](https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.3+Release+Notes) for more details.
