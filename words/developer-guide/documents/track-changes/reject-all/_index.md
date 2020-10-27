---
title: "Reject all"
second_title: "Revisions in a Word Document"
type: docs
url: /documents/track-changes/reject-all/
aliases: [/reject-all-revisions-in-a-document/]
keywords: "word revision tracking, track changes, track changes in word"
description: "Reject all revisions in a Word document"
weight: 20
---

This REST API rejects all revisions in a document.

The request parameters are the following:

|Parameter Name|Type|Query String/HTTP Body|Description|
| :- | :- | :- | :- |
|destFileName|string|Query string: destFileName=AfterAcceptAll.doc|Result path of the document after the operation. If this parameter is omitted then the result of the operation will be saved as the source document.|
|folder|string|Query string: folder=MyFolder|Original document folder.|
|storage|string|Query string: storage=MyAmazonS3Storage|Original document storage.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Revisions/RejectAllRevisions) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to reject all revisions in a document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/revisions/rejectAll" \
-X PUT \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Content-Length: 0" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Result": {
    "Source": {
      "Href": "test_multi_pages.docx",
      "Rel": "self",
      "Type": null,
      "Title": null
    },
    "Dest": {
      "Href": "test_multi_pages.docx",
      "Rel": "result",
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

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< nosnippet >}}
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "RejectAllRevisions.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "RejectAllRevisions.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "reject_all_revisions.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "reject_all_revisions.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "rejectAllRevisions.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_RejectAllRevisions.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_RejectAllRevisions.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "RejectAllRevisions.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
