---
title: "Working with cURL"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /getting-started/using-curl/
description: "Using the curl utility to interact with REST APIs"
weight: 80
---

HTTP requests are composed of several components: HTTP method, URI, headers, query parameters, and request body. Each of these components plays an important role in communicating information between a client and a server.

The `curl` command is a popular command-line tool for making HTTP requests. It provides a way to specify each of the components of an HTTP request using command line parameters. When making requests to the Aspose.Words Cloud API, you can use `curl` to specify each of the HTTP request components.

Let's take a closer look at each of the HTTP request components and how they relate to `curl` command line parameters:

* **HTTP method**. The HTTP method specifies the action that the client wants the server to take. The most commonly used HTTP methods are `GET`, `POST`, `PUT`, and `DELETE`. In `curl`, The `-X` option is used to specify the HTTP method. In this example, we are using `curl` to send a GET request to retrieve the paragraphs of the first section in a Word document:

```
curl -X GET "https://api.aspose.cloud/v4.0/words/document.docx/sections/0/paragraphs"
```


* **URI**. The Uniform Resource Identifier (URI) specifies the target resource being accessed. The URI is simply specified as the final argument in the `curl` command. 

  Let's take a look at the structure of the URI above. It consists of a scheme (`https`), a hostname (`api.aspose.cloud`), an API version (`v4.0`), a resource type (`words`), a document name (`document.docx`), and a resource endpoint (`/sections/0/paragraphs`). The resource endpoint specifies the path to the resource we want to access, which in this case is the paragraphs of the first section of a Word document. The endpoint contains two path segments separated by slashes: `sections` and `paragraphs`. `sections/0` specifies the first section of the document, and `paragraphs` specifies the paragraphs within that section

* **HTTP Headers**. HTTP headers provide additional information about the request, such as the content type, authorization token, and more. In `curl`, headers can be specified using the `-H` option. For example, to include an authorization token in the request header, you would use the following command:

```
curl -X GET -H "Authorization: Bearer [ACCESS_TOKEN]" "https://api.aspose.cloud/v4.0/words/document.docx"
```


* **Request Body**. The request body contains the data being sent as part of the request, such as form data or JSON payload. This component is optional, and not all requests will have a request body.
  In curl, the `-F` and `-d` options are used to specify the data to be sent in the request body. The `-F` option is used to send data in the form of name-value pairs, including files. This option uses the `multipart/form-data` content type to encode the data, which allows for the transmission of binary data as well as text data. The `-F` option is typically used when submitting web forms.

  Let's look at an example of sending data in the request body.

```
curl -X POST "https://api.aspose.cloud/v4.0/words/convert" \
     -H "Content-Type: multipart/form-data" \
     -F "file=@/path/to/file.docx" \
     -F "format=pdf" \
     -d '{"fileName": "output.pdf"}' \
     -H "Authorization: Bearer [ACCESS_TOKEN]"
```

In this example, we are using `curl` to convert a Word document to PDF format. The `-F` option is used to specify the file to be uploaded and the desired output format. The `-d` option is used to provide additional data in the request body, in this case, the output file name. Note that the data provided with `-d` is in JSON format and needs to be enclosed in quotes to ensure it is treated as a single string.

