---
title: "Read Field Names"
second_title: "Mail Merge"
type: docs
url: /mail-merge/read-field-names/
aliases: [/read-mailmerge-document-field-names/]
keywords: "Read, mustache template, online, Mail Merge, Word, Microsoft Word"
description: "Get MailMerge field names in a Word document"
weight: 50
---

This example explains how to get **Mail Merge** field names.

The following is a description of the most important parameters:

- **useNonMergeFields**. Result includes "mustache" field names if UseNonMergeFields is true

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/MailMerge/GetDocumentFieldNamesOnline) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use `cURL` command-line tool to easily interact with Aspose.Words web services. The following example demonstrates how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to read MailMerge document Field Names
curl -v "https://api.aspose.cloud/v4.0/words/SampleMailMergeTemplate.docx/mailMerge/FieldNames" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
    "FieldNames": {
        "Names": [
            "FullName",
            "Company",
            "Address",
            "Address2",
            "City",
            "FullName"

        ],
        "link": {
            "Href": "http://api.aspose.cloud/v4.0/words/SampleMailMergeTemplate.docx/mailmerge/getFieldNames",
            "Rel": "self",
            "Type": null,
            "Title": null
        }
    },
    "Code": 200,
    "Status": "OK"
}
```

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "GetDocumentFieldNames.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetDocumentFieldNames.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "GetDocumentFieldNames.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetDocumentFieldNames.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetDocumentFieldNames.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetDocumentFieldNames.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetDocumentFieldNames.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetDocumentFieldNames.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetDocumentFieldNames.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
