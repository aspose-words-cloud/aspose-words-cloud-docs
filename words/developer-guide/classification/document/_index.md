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

**Note**: The SDKs in C#, Java, PHP, Ruby, Python, Node.js, Android, Swift and Go are available for download. Also the sample code are given below for each of the SDKs:

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Classification/ClassifyDocument) lets you call the REST API directly from the browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL, supplied with a sample **Input Document** [test_multi_pages.docx](test_multi_pages.docx).

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

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

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

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "ClassifyTaxonomyDocument.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "ClassifyTaxonomyDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "ClassifyTaxonomyDocument.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "ClassifyTaxonomyDocument.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "ClassifyTaxonomyDocument.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "ClassifyTaxonomyDocument.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_ClassifyTaxonomyDocument.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_ClassifyTaxonomyDocument.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "ClassifyWithTaxonomyDocuments.Go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
