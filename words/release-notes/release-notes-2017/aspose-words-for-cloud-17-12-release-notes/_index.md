---
title: "Aspose.Words for Cloud 17.12 Release Notes"
type: docs
url: /aspose-words-for-cloud-17-12-release-notes/
aliases: [/aspose-words-for-cloud-17-12-release-notes/]
weight: 10
---

{{% alert color="primary" %}} 

The page contains release notes for Aspose.Words for Cloud update 17.12 – [API Reference](https://apireference.aspose.cloud/words/)

{{% /alert %}} 

## Full List of Issues Covering all Changes in this Release

#### PHP SDK

A fully reworked version of Aspose.Words for Cloud PHP SDK has been released. PHP Cloud SDK is a wrapper around REST APIs, allowing to process documents in PHP 5.6 or higher quickly and easily, gaining all benefits of strong types and IDE highlights. The distribution is available at [Packagist](https://packagist.org/packages/aspose/words-sdk-php) and source code at [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-php).

New SDK is fully supported and has the following advantages over the previous versions:

- SDK is fully in sync with the API, all missing methods are added
- Classes, methods, and properties have comments and are IDE-friendly
- Better security
- Usage of Request/Response classes to represent long lists of parameters. This allows for cleaner code and easier backward-compatibility going forward

SDK is not backward compatible with the previous generation because of the last item. It should be straightforward to convert program code to using Request/Response objects, if you need any help on migration please ask at [Free Support Forums](https://forum.aspose.cloud/c/words).

#### PDF to Word: Image Conversion

This release improves support for images in [PDF to Word conversion](/working-with-pdf-documents/). The following cases are now supported:

- Semi-transparent images
- Rotated images
- Inline images (images that go "inside" the text, being a logical part of text paragraph)

The following restrictions still apply:

- Vector images (rendered via PDF paint operators) are not converted
