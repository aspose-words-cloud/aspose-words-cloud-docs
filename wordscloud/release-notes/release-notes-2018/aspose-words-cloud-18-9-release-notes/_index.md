---
title: "Aspose.Words Cloud 18.9 Release Notes"
type: docs
url: /aspose-words-cloud-18-9-release-notes/
weight: 30
---

{{% alert color="primary" %}} 

The page contains release notes for Aspose.Words Cloud 18.9 – [API Reference](https://apireference.aspose.cloud/words/)

{{% /alert %}} 
## **Important Changes and New Features**
#### **Java SDK**
Fully reworked version of Aspose Cloud Java SDK has been released. Java Cloud SDK is a wrapper around REST API, allowing to process documents in Java 1.7+ quickly and easily, gaining all benefits of strong types and IDE highlights. The distribution is available at [Maven ](https://artifact.aspose.cloud/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words-cloud)and source code at [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-java).

New SDK is fully supported and has the following advantages over the previous versions:

- SDK is fully in sync with the API, all missing methods are added
- Classes, methods, and properties have comments and are IDE-friendly
- Better security
- Usage of Request/Response classes to represent long lists of parameters. This allows for cleaner code and easier backward-compatibility going forward
  SDK is not backward compatible with the previous generation because of the last item. It should be straightforward to convert program code to using Request/Response objects, if you need any help on migration please ask at Free Support Forums.
#### **Added new saveoptions**
1. HtmlFixedSaveOptions.SaveFontFaceCssSeparately
1. MtmlSaveOption.ExportCidUrlsForMhtmlResources
#### **Added "paragraph format" resource**
It provides access to the paragraph formatting properties:

- [Represents all the formatting for a paragraph](https://apireference.aspose.cloud/words/#!/Paragraphs/GetDocumentParagraphFormat)
- [Updates paragraph format properties, returns updated format properties](https://apireference.aspose.cloud/words/#!/Paragraphs/PostDocumentParagraphFormat)
