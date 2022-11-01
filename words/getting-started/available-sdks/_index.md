---
title: "Available SDKs"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /getting-started/available-sdks/
aliases: [/available-sdks/]
description: "Available SDKs"
weight: 50
---

Aspose.Words Cloud is a modern REST API, that allows easy integration into existing systems.

Using an SDK is the quickest way to speed up the development. An SDK takes care of low-level details by making requests and handling responses and lets you focus on writing code specific to your particular project.

## SDK Benefits

Our supported SDKs are 100% tested. They are open source and released to the public under the MIT License. You can use them absolutely free of charge.

## Cloud SDK Family

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="1" tabName1=".NET" tabName2="C++" tabName3="Java" tabName4="PHP" tabName5="Ruby" tabName6="Python" tabName7="Node.js" >}}
{{< tab tabNum="1" >}}

**Aspose.Words Cloud SDK for .NET** allows you to work with Aspose.Words Cloud REST APIs in your .NET applications easily.

You can download the .NET SDK from the [GitHub repository](https://github.com/aspose-words-cloud/aspose-words-cloud-dotnet).

{{< /tab >}}
{{< tab tabNum="2" >}}

**Aspose.Words Cloud SDK for C++** empowers you to work with Aspose.Words Cloud REST APIs in your C++ applications.

You can download the C++ SDK from the [GitHub repository](https://github.com/aspose-words-cloud/aspose-words-cloud-cpp).

{{< /tab >}}
{{< tab tabNum="3" >}}

**Aspose.Words Cloud SDK for Java** provides a quick and easy mechanism to incorporate Aspose.Words Cloud APIs in your Java applications.

You can download the Java SDK from the [GitHub repository](https://github.com/aspose-words-cloud/aspose-words-cloud-java).

{{< /tab >}}
{{< tab tabNum="4" >}}

**Aspose.Words Cloud SDK for PHP** is a convenient approach to use Aspose.Words Cloud REST APIs in PHP applications.

You can download the PHP SDK from the [GitHub repository](https://github.com/aspose-words-cloud/aspose-words-cloud-php).

{{< /tab >}}
{{< tab tabNum="5" >}}

**Aspose.Words Cloud SDK for Ruby** is a Free approach of using Aspose.Words Cloud REST APIs in Ruby applications.

You can download the Ruby SDK from the [GitHub repository](https://github.com/aspose-words-cloud/aspose-words-cloud-ruby).

{{< /tab >}}
{{< tab tabNum="6" >}}

**Aspose.Words Cloud SDK for Python** is a convenient approach to incorporate Aspose.Words Cloud services in Python applications.

You can download the Python SDK from the [GitHub repository](https://github.com/aspose-words-cloud/aspose-words-cloud-python).

{{< /tab >}}
{{< tab tabNum="7" >}}

**Aspose.Words Cloud SDK for Node.js** provides the capabilities to work with Aspose.Words Cloud REST APIs in Node.js applications. Use the SDK to produce stunning applications.

You can download the Node.js SDK from the [GitHub repository](https://github.com/aspose-words-cloud/aspose-words-cloud-node).

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## cURL

cURL is a cross platform command-line tool for getting or sending data including files using URL syntax. It can be used to perform Aspose.Words Cloud [REST API](https://apireference.aspose.cloud/words/) requests.

To make these requests you need to get **JSON Web Token** (JWT).

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# Please get your `Client Id` and `Secret` credentials from https://dashboard.aspose.cloud/applications.
# Place `Client Id` in client_id argument. Place `Secret` in client_secret argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxxx&client_secret=xxxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "access_token": ".....",
  "expires_in": 86400,
  "token_type": "Bearer"
} 
```
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
