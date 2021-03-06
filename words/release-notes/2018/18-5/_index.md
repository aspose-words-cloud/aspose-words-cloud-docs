---
title: "18.5 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2018/18-5/
aliases: [/aspose-words-for-cloud-18-5-release-notes/]
description: "Aspose Words Cloud 18.5 Release Notes"
weight: 70
---

The page contains release notes for Aspose.Words for Cloud update 18.5 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## Classification

18.5 is a major release introducing brand new API that performs [text and document classification](https://en.wikipedia.org/wiki/Document_classification) using machine learning and natural language processing techniques. Currently, text samples and documents are classified into [Interactive Advertising Bureau (IAB) taxonomy](https://www.iab.com/guidelines/taxonomy/) categories. More information about the API is available here.

## Headers/footers

PDF to Word conversion now supports detecting headers and footers. Sections of PDF pages containing page numbers, document names etc. will be converted as headers and footers in Word document that do not affect rest of the page layout and are not moved while the document is being edited.

## documentFileName

The following methods now support **documentFileName** parameter:

- [PUT /convert](https://apireference.aspose.cloud/words/#!/Convert/PutConvertDocument).
- [PUT /executeMailMerge](https://apireference.aspose.cloud/words/#!/MailMerge/PutExecuteMailMergeOnline).
- [PUT /executeTemplate](https://apireference.aspose.cloud/words/#!/MailMerge/PutExecuteTemplateOnline).

This new attribute is handy when resulting document has dynamic field for document name, and allows to specify that via API or SDK.
