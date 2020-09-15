---
title: "Text Classification"
type: docs
url: /text-classification/
weight: 20
---

# **Introduction**
Aspose.Words Cloud supports [text and document classification](https://en.wikipedia.org/wiki/Document_classification) into the [Interactive Advertising Bureau (IAB) taxonomy](https://www.iab.com/guidelines/taxonomy/) categories. Document classification is often used in various business processes to automate the flow of documents through the organization.

Text classification is a lightweight version of classification API that processes text snippets. You do not need to store the snippet on any storage, instead, it is supplied in the request body.
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Classification/Classify) lets you call this REST API directly from the browser. The description of the API and its parameters is also given there.
## **cURL Example**
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \

-X POST \

-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"



// cURL example to classify raw text

curl -v "https://api.aspose.cloud/v4.0/words/classify?bestClassesCount=3" \

-X PUT \

-d "'text to classify'" \

-H "Content-Type: application/json" \

-H "Accept: application/json" \

-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

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

      "ClassName": "News\_and\_Politics",

      "ClassProbability": 9.13

    }

  ],

  "Code": 200,

  "Status": "OK"

} 

```

{{< /tab >}}

{{< /tabs >}}
# **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "RawTextClassification.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "RawTextClassification.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "RawTextClassification.php" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "RawTextClassification.py" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "RawTextClassification.rb" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "RawTextClassification.js" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_RawTextClassification.java" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_RawTextClassification.swift" >}}

{{< /tab >}}

{{< tab tabNum="9" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "ClassifyRawText.go" >}}

{{< /tab >}}

{{< /tabs >}}
