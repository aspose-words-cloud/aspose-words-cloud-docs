---
title: "Aspose.Words for Cloud 18.2 Release Notes"
type: docs
url: /release-notes/2018/18-2/
aliases: [/aspose-words-for-cloud-18-2-release-notes/]
weight: 100
---

The page contains release notes for Aspose.Words for Cloud update 18.2 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

#### Node.js SDK

Fully reworked version of Aspose Cloud Node.js SDK has been released. Node.js Cloud SDK is a wrapper around REST API, allowing to process documents in Node.js 4.8 or higher quickly and easily, gaining all benefits of strong types and IDE highlights. The distribution is available at [npm](https://www.npmjs.com/package/asposewordscloud) and source code at [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-node).

New SDK is fully supported and has the following advantages over the previous versions:

- SDK is fully in sync with the API, all missing methods are added
- Classes, methods, and properties have comments and are IDE-friendly
- Better security
- Usage of Request/Response classes to represent long lists of parameters. This allows for cleaner code and easier backward-compatibility going forward

SDK is not backward compatible with the previous generation because of the last item. It should be straightforward to convert program code to using Request/Response objects, if you need any help on migration please ask at [Free Support Forums](https://forum.aspose.cloud/).

#### Conversion of encrypted PDF files to Word

Aspose.Words now supports encrypted PDF files for **PDF to Word conversion**.

#### Dropping support for Word to SWF conversion

Based on Adobe's [deprecation of Flash](https://theblog.adobe.com/adobe-flash-update/), conversion to SWF is no longer supported by Words Cloud API.

#### Dropping support of deprecated save option properties

Some save options that have been deprecated in Aspose.Words .NET are now not available in Aspose.Words Cloud REST API as well. Full list of properties is as follows:

|Removed Property|Property to use instead|
| :- | :- |
|HtmlSaveOptions.AllowNegativeLeftIndent|HtmlSaveOptions.AllowNegativeIndent|
|HtmlSaveOptions.ExportHeadersFooters|HtmlSaveOptions.ExportHeadersFootersMode|
|HtmlFixedSaveOptions.MetafileRenderingMode|HtmlFixedSaveOptions.MetafileRenderingOptions.RenderingMode|
|SvgSaveOptions.MetafileRenderingMode|SvgSaveOptions.MetafileRenderingOptions.RenderingMode|
|XpsSaveOptions.HeadingsOutlineLevels|XpsSaveOptions.OutlineOptions.HeadingsOutlineLevels|
|XpsSaveOptions.BookmarksOutlineLevel|XpsSaveOptions.OutlineOptions.DefaultBookmarksOutlineLevel|
|XpsSaveOptions.MetafileRenderingMode|XpsSaveOptions.MetafileRenderingOptions.RenderingMode|

See [Aspose.Words .NET 18.2 Release Notes](https://docs.aspose.com/display/wordsnet/Aspose.Words+for+.NET+18.2+Release+Notes) for more details.

Please note that other deprecated save options may be dropped in the future as well, specifically in PdfSaveOptions class.
