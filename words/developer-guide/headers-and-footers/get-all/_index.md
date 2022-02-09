---
title: "Get all"
second_title: "Headers and Footers in a Document"
type: docs
url: /headers-and-footers/get-all/
aliases: [/get-all-header-and-footers-in-a-document/]
description: "Get all headers and footers in a Word document"
weight: 50
---

This REST API retrieves all Headers and Footers.

## REST API calls using cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetHeaderFootersOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetHeaderFootersOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "HeaderFooters": {
    "List": [
      {
        "Type": "HeaderEven",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "HeaderPrimary",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "FooterEven",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/2",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "FooterPrimary",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/3",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "HeaderFirst",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/4",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Type": "FooterFirst",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/sections/0/headersfooters/5",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/HeadersFooters.doc/headersfooters",
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

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Code samples in Python, Java, C#, etc.

The following code samples show how to interact with REST API using almost any mainstream programming language (Python, Java, C#, JavaScript, PHP, C++, Golang, Ruby, Swift, Dart):

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetHeaderFootersOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetHeaderFootersOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetHeaderFootersOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetHeaderFootersOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetHeaderFootersOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetHeaderFootersOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetHeaderFootersOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetHeaderFootersOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetHeaderFootersOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetHeaderFootersOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
