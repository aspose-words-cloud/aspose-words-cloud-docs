---
title: "Aspose.Words Cloud 18.8 Release Notes"
type: docs
url: /release-notes/2018/18-8/
aliases: [/aspose-words-cloud-18-8-release-notes/]
weight: 40
---

The page contains release notes for Aspose.Words Cloud 18.8 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

#### Vector graphics support for PDF to Word conversion

PDF to Word converter now supports basic vector graphics.

#### Table detection and recognition improvements for PDF to Word conversion

Accuracy of table detection was significantly improved. Almost all simple tables are detected properly now.

#### Ruby SDK

Fully reworked version of Aspose Cloud Ruby SDK has been released. Ruby Cloud SDK is a wrapper around REST API, allowing to process documents in Ruby 2.3 quickly and easily, gaining all benefits of strong types and IDE highlights. The distribution is available at [rubygems.org ](https://rubygems.org/gems/aspose_words_cloud)and source code at [GitHub ](https://github.com/aspose-words-cloud/aspose-words-cloud-ruby).

New SDK is fully supported and has the following advantages over the previous versions:

- SDK is fully in sync with the API, all missing methods are added
- Classes, methods, and properties have comments and are IDE-friendly
- Better security
- Usage of Request/Response classes to represent long lists of parameters. This allows for cleaner code and easier backward-compatibility going forward
  SDK is not backward compatible with the previous generation because of the last item. It should be straightforward to convert program code to using Request/Response objects, if you need any help on migration please ask at Free Support Forums.

#### Python SDK

Fully reworked version of Aspose Cloud Python SDK has been released. Python Cloud SDK is a wrapper around REST API, allowing to process documents in Python 2.7, or higher (>=3.6) quickly and easily, gaining all benefits of strong types and IDE highlights. The distribution is available at [pypi.org ](https://pypi.org/project/asposewordscloud)and source code at [GitHub ](https://github.com/aspose-words-cloud/aspose-words-cloud-python).

New SDK is fully supported and has the following advantages over the previous versions:

- SDK is fully in sync with the API, all missing methods are added
- Classes, methods, and properties have comments and are IDE-friendly
- Better security
- Usage of Request/Response classes to represent long lists of parameters. This allows for cleaner code and easier backward-compatibility going forward
  SDK is not backward compatible with the previous generation because of the last item. It should be straightforward to convert program code to using Request/Response objects, if you need any help on migration please ask at Free Support Forums.

#### Added new saveoptions

- OutlineOptions.CreateOutlinesForHeadingsInTables
- OPdfSaveOption.HeaderFooterBookmarksExportMode

#### Added "taxonomy" parameter to document classification

The "taxonomy" parameter is responsible for the list of classifier classes. By default, the classification is performed according to the "IAB-2" taxonomy (10 news classes), if the parameter is not specified or is set to "default".

IAB-2 taxonomy: <https://www.iab.com/guidelines/taxonomy/>.

Alternatively, there is a taxonomy "documents" (10 classes of documents). If the taxonomy parameter is set to "documents", the classification will be performed using "documents" taxonomy.

Please check this article for details:
