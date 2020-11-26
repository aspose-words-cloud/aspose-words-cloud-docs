---
title: "Generate Report Online"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /report/build-online/
aliases: [/build-report-online/]
keywords: ""
description: "Generate a report online"
weight: 20
---

This REST API builds a report online.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Report/BuildReportOnline) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get a list of sections
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/Report/BuildReportOnline" \
-X PUT\
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Sections": {
    "SectionLinkList": [
      {
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections",
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

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="4" tabName1="C#" tabName2="PHP" tabName3="Golang" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "BuildReportOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "BuildReportOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "build_reports_online.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## See also

- Product page description: <a href="https://products.aspose.cloud/words/python/report" target="_blank">Python</a>, <a href="https://products.aspose.cloud/words/net/report" target="_blank">C#</a>, <a href="https://products.aspose.cloud/words/java/report" target="_blank">Java</a>, <a href="https://products.aspose.cloud/words/nodejs/report" target="_blank">Node.js</a>, <a href="https://products.aspose.cloud/words/php/report" target="_blank">PHP</a>, <a href="https://products.aspose.cloud/words/go/report" target="_blank">Go</a>
- <a href="https://products.aspose.app/words/assembly" target="_blank">Free online assembly app</a>
