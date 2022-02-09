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

The SDKs in C#, Java, PHP, Ruby, Python, Node.js, Swift and Go are available for download. Also the sample code are given below for each of the SDKs:

{{% /alert %}}

## Usage examples with cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

Download sample [test_multi_pages.docx](test_multi_pages.docx) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "ClassifyDocumentOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "ClassifyDocumentOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
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

## Aspose.Words Cloud SDK Family

Using SDK is the best way to speed up the development. Our Cloud SDKs take care of low-level details and let you focus on your primary tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs.

## Usage examples in Python, Java, C#, etc.

The following code samples show how to interact with REST API using almost any mainstream programming language. You can find a lot of The following code samples show how to interact with REST API using almost any mainstream programming language. You can find a lot of other code examples in [Python](https://gist.github.com/aspose-words-cloud-gists/e26813ced70692c544820cd8011ee7e0), [Java](https://gist.github.com/aspose-words-cloud-gists/caede439bfd2e57c3010befe504faff4), [C#](https://gist.github.com/aspose-words-cloud-gists/374e1e3dd4bca8f696f29d913645f549), [JavaScript](https://gist.github.com/aspose-words-cloud-gists/a9510e4b51613f1138e7c1ec09634c4a), [PHP](https://gist.github.com/aspose-words-cloud-gists/e2a72445b96362dc0117f06ab54bb94a), [C++](https://gist.github.com/aspose-words-cloud-gists/49aa5151a094849179bae8672c887a0e), [Golang](https://gist.github.com/aspose-words-cloud-gists/625ca80adffd779e8f6e3611551e14d5), [Ruby](https://gist.github.com/aspose-words-cloud-gists/339f3835a4c0a536c81ec941de29baf7), [Swift](https://gist.github.com/aspose-words-cloud-gists/790dbd2edd5d36f170732366f52cac4c), [Dart](https://gist.github.com/aspose-words-cloud-gists/6aae628cf2b878b78fea177c3171c6bf) on GitHub. All codes are thoroughly tested and ready for production use.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "ClassifyDocumentOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "ClassifyDocumentOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "ClassifyDocumentOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "ClassifyDocumentOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "ClassifyDocumentOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "ClassifyDocumentOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "ClassifyDocumentOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "ClassifyDocumentOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "ClassifyDocumentOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "ClassifyDocumentOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
