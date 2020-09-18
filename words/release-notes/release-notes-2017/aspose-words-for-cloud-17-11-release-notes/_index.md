---
title: "Aspose.Words for Cloud 17.11 Release Notes"
type: docs
url: /aspose-words-for-cloud-17-11-release-notes/
aliases: [/aspose-words-for-cloud-17-11-release-notes/]
weight: 20
---

{{% alert color="primary" %}} 

The page contains release notes for Aspose.Words for Cloud update 17.11 – [API Reference](https://apireference.aspose.cloud/words/)

{{% /alert %}} 
## Full List of Issues Covering all Changes in this Release

|**Key**|**Summary**|**Category**|
| :- | :- | :- |
|WORDSCLOUD-241|DOCX to PDF conversion issue with SmartArt rendering|Bug|
|WORDSCLOUD-266|` `Horizontal and Vertical Merge properties of Cell are updated incorrectly|Bug|
|WORDSCLOUD-308|Footer missing in converting from Word to PDF|Bug|
## Important changes and new Features
A fully reworked version of Aspose Cloud .NET SDK has been released. .NET Cloud SDK is a wrapper around REST API, allowing to process documents in C# quickly and easily, gaining all benefits of strong types and IDE highlights. The distribution is available at [NuGet](https://www.nuget.org/packages/Aspose.Words-Cloud/) and source code at [GitHub](https://github.com/asposecloud/Aspose.Words-Cloud/tree/master/SDKs/NET).

New SDK is fully supported and has the following advantages over the previous versions:

- SDK is fully in sync with the API, all missing methods are added
- Classes, methods, and properties have comments and are IDE-friendly
- Better security
- Usage of Request/Response classes to represent long lists of parameters. This allows for cleaner code and easier backward-compatibility going forward

The SDK is not backward compatible with the previous generation because of the last item. It should be straightforward to convert program code to using Request/Response objects, if you need any help on migration please ask at [Free Support Forums](https://forum.aspose.cloud/c/words).
#### PDF to Word: Image Conversion Support
This release introduces support for images in [PDF to Word conversion](/working-with-pdf-documents/). Some limitations still apply:

- Semi-transparent images are not converted properly
- Rotated images are not supported
- Inline images (logical parts of text paragraphs) are converted as standalone images
