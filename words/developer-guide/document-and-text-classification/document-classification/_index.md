---
title: "Document Classification"
type: docs
url: /document-classification/
aliases: [/document-classification/]
keywords: "Document Classification, Taxanomy, IAB-2 taxonomy, Document Taxonomy, Word, Microsoft Word, Java, .NET, PHP, Ruby, Python, NodeJS, Swift, Android ,Go"
description: "The businesses are now receiving different kind of text-based documents. These documents might be brochures, emails, letters, support tickets and many more. It becomes more challenging when executives or any concerned people need an immediate insight from the all text-based documents. The organizations know well that their data should be accumulated categorically. Hence, they are creating taxonomies. When the data is indexed in a taxonomy, users can find what they actually required.The Taxonomy (general) is the practice and science of classification of things or concepts, including the principles that underlie such classification. In our case, this is a list of text categories. The Aspose.Words Cloud support two taxonomies for now: IAB-2 taxonomy: Documents taxonomy:ADVE - advertisements, brochuresEmailFormLetterMemo - memorandumsNews - articles, including news articlesInvoiceReportResumeScientific - scientific papersOther - the other classes of documents or cases where the classifier is not sure"
weight: 10
---

The businesses are now receiving different kind of text-based documents. These documents might be brochures, emails, letters, support tickets and many more. It becomes more challenging when executives or any concerned people need an immediate insight from the all text-based documents. The organizations know well that their data should be accumulated categorically. Hence, they are creating taxonomies. When the data is indexed in a taxonomy, users can find what they actually required.

The [Taxonomy (general)](https://en.wikipedia.org/wiki/Taxonomy_\(general\)) is the practice and science of classification of things or concepts, including the principles that underlie such classification. In our case, this is a list of text categories. The Aspose.Words Cloud support two taxonomies for now:

1. **IAB-2 taxonomy**: <https://www.iab.com/guidelines/taxonomy/>
1. **Documents taxonomy:**
   1. ADVE - advertisements, brochures
   1. Email
   1. Form
   1. Letter
   1. Memo - memorandums
   1. News - articles, including news articles
   1. Invoice
   1. Report
   1. Resume
   1. Scientific - scientific papers
   1. Other - the other classes of documents or cases where the classifier is not sure

The API important parameters are:

1. **Parameter Name:** bestClassesCount
   **Description:** Count of top classes for the target text
1. **Parameter Name:** taxonomy
   **Description:** Taxonomy to classify with. If the field is empty or "default" then IAB-2 taxonomy will be used. Documents taxonomy will be used in other cases.

Document classification supports classifying documents stored on Aspose Storage or any of [the supported storage](https://docs.aspose.cloud/display/storagecloud/How+to+Configure+3rd+Party+Cloud+Storages). API supports all document formats [supported by other Aspose.Words Cloud methods](https://products.aspose.cloud/words/cloud), including PDF which will be implicitly [converted to Word format](/convert-pdf-document-to-word/).

**Note:** The SDKs in C#, Java, PHP, Ruby, Python, Node.js, Android, Swift and Go are available for download. Also the sample code are given below for each of the SDKs:

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Classification/ClassifyDocument) lets you call the REST API directly from the browser. The description of the API and its parameters is also given there.

## cURL Example

**Input Document:** [test_multi_pages.docx](attachments/884752/1180129.docx)

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to classify document

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/classify?bestClassesCount=3&taxonomy=documents" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
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
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples.

## SDK Examples

Code examples for various SDKs are presented below:
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
