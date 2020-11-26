---
title: "Document Classification"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /classification/document
aliases: [/document-classification/]
keywords: "Document Classification, Taxanomy, IAB-2 taxonomy, Document Taxonomy, Word, Microsoft Word"
description: "Learn how to work with document classification"
weight: 10
---

The businesses are now receiving different kind of text-based documents. These documents might be brochures, emails, letters, support tickets and many more. It becomes more challenging when executives or any concerned people need an immediate insight from the all text-based documents. The organizations know well that their data should be accumulated categorically. Hence, they are creating taxonomies. When the data is indexed in a taxonomy, users can find what they actually required.

The [Taxonomy (general)](https://en.wikipedia.org/wiki/Taxonomy_\(general\)) is the practice and science of classification of things or concepts, including the principles that underlie such classification. In our case, this is a list of text categories. The Aspose.Words Cloud support two taxonomies for now:

- **IAB-2 taxonomy**: <https://www.iab.com/guidelines/taxonomy/>
- **Documents taxonomy:**
   - ADVE - advertisements, brochures
   - Email
   - Form
   - Letter
   - Memo - memorandums
   - News - articles, including news articles
   - Invoice
   - Report
   - Resume
   - Scientific - scientific papers
   - Other - the other classes of documents or cases where the classifier is not sure

The following is a description of the most important parameters:

- **Parameter Name**: bestClassesCount
- **Description**: Count of top classes for the target text
- **Parameter Name**: taxonomy
- **Description**: Taxonomy to classify with. If the field is empty or "default" then IAB-2 taxonomy will be used. Documents taxonomy will be used in other cases.

Document classification supports classifying documents stored on Aspose Storage or any of [the supported storage](https://docs.aspose.cloud/display/storagecloud/How+to+Configure+3rd+Party+Cloud+Storages). API supports all document formats [supported by other Aspose.Words Cloud methods](https://products.aspose.cloud/words/cloud), including PDF which will be implicitly [converted to Word format](/words/convert/pdf-to-word/).


{{% alert style="info" %}}

The SDKs in C#, Java, PHP, Ruby, Python, Node.js, Android, Swift and Go are available for download. Also the sample code are given below for each of the SDKs:

{{% /alert %}}

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Classification/ClassifyDocument) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [test_multi_pages.docx](test_multi_pages.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to classify document
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/classify?bestClassesCount=3&taxonomy=documents" \
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
  "BestClassName": "Report",
  "BestClassProbability": 50.0,
  "BestResults": [
    {
      "ClassName": "Report",
      "ClassProbability": 50.0
    },
    {
      "ClassName": "Letter",
      "ClassProbability": 25.0
    },
    {
      "ClassName": "Memo",
      "ClassProbability": 12.5
    }
  ],
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
{{< tabs tabTotal="9" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="Golang" tabName7="Ruby" tabName8="Android" tabName9="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "ClassifyTaxonomyDocument.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "ClassifyTaxonomyDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "ClassifyTaxonomyDocument.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "ClassifyTaxonomyDocument.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "ClassifyTaxonomyDocument.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "ClassifyWithTaxonomyDocuments.Go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "ClassifyTaxonomyDocument.rb" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_ClassifyTaxonomyDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_ClassifyTaxonomyDocument.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
