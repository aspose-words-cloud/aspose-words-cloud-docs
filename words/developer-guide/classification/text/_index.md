---
title: "Text Classification"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /classification/text
aliases: [/text-classification/]
description: "Classify the text documents into one or many categories."
weight: 20
---

Aspose.Words Cloud supports [text and document classification](https://en.wikipedia.org/wiki/Document_classification) into the [Interactive Advertising Bureau (IAB) taxonomy](https://www.iab.com/guidelines/taxonomy/) categories. Document classification is often used in various business processes to automate the flow of documents through the organization.

Text classification is a lightweight version of classification API that processes text snippets. You do not need to store the snippet on any storage, instead, it is supplied in the request body.

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Classification/Classify) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
	{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "Classify.curl" >}}
	<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< tab tabNum="2" >}}
	{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "Classify.json" >}}
	<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "BestClassName": "Movies",
  "BestClassProbability": 36.64,
  "BestResults": [
    {
      "ClassName": "Movies",
      "ClassProbability": 36.64
    },
    {
      "ClassName": "Education",
      "ClassProbability": 12.81
    },
    {
      "ClassName": "News_and_Politics",
      "ClassProbability": 9.13
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
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
	{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "Classify.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
	{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "Classify.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
	{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "Classify.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
	{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "Classify.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
	{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "Classify.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
	{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "Classify.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
	{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
	{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "Classify.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
	{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "Classify.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
	{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Classify.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
	{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "Classify.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
