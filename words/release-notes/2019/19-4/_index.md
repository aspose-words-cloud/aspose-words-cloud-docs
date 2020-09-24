---
title: "19.4 Release Notes"
second_title: "Aspose Words Cloud"
type: docs
url: /release-notes/2019/19-4/
aliases: [/aspose-words-cloud-19-4-release-notes/]
weight: 60
---

The page contains release notes for Aspose.Words Cloud 19.4 – [API Reference](https://apireference.aspose.cloud/words/).

## Important Changes and New Features

## API

1. Added "Storage" endpoints.
1. Changed PUT to POST (and vice versa): from now on, all idempotent methods are PUT and non-idempotent ones are POST.
1. "destFileName" parameter: now it contains absolute (instead of relative) path to save result file.
1. Fixed serialization of "SourceFormat" property in "Document" response.
1. "nodepath" parameter is always "path" type now.
1. Removed "envelop" from all responses.

## PDF

1. Improved recognition for multi-line headers and footers.
1. Fixed an error while several documents are processing in parallel.
