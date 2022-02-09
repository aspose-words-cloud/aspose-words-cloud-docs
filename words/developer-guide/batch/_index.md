---
title: "Batch Requests"
type: docs
url: /batch/
aliases: [/batch-requests/]
description: "Group and combine multiple REST API calls with batch requests"
weight: 9
---

Since the speed of data processing may have a significant impact on business effectiveness, it is sometimes required to execute a higher number of operations per unit of time and boost the document processing speed in a limited-resource environment.

Consider the situation you are writing a document-processing solution that issues dozens of REST API calls per second during peak times. As each HTTPS connection results in a certain amount of processing overhead on the network efficiency, avoiding the time-consuming TCP negotiation becomes an important task. Combining multiple requests into a single batch may optimize network utilization and eliminate network latency issues.

To address these needs, Aspose.Words Cloud API provides the **Batch Request** feature designed to group multiple REST API requests into a single request. This technique can minimize the intensity of client-server interactions and provide the top speed of document processing at the same time.

## Batch Request Processing Model

Batch processing is commonly defined as "processing a number of cases simultaneously". The basic logic behind batch request processing is presented in the diagram below.

![batch.png](batch.png)

The batching technique comprises both concurrent and sequential request processing, where concurrent requests can be processed in an arbitrary order with the same result, and sequential requests depend on being processed step-by-step. There is no restriction on the number of inner requests inside a single batch request.

The requests in a batch are very similar to ordinary requests but have two new headers — `RequestId` for identification of a request and `DependsOn` for setting the dependency — and the `resultOf(RequestId)` placeholder which is set to the execution result of the corresponding inner request.

The `RequestId` and `DependsOn` headers are required to ensure sequential processing support. For that reason, all the `RequestId` values in a batch must be unique. There is normally no need to define `RequestId` and `DependsOn` for concurrent batch processing.

When the processing of all operations in a batch is completed, a consolidated response is returned and the HTTPS connection is closed.

### Concurrent Request Processing

In a general case batch requests are processed concurrently. Parallel processing, as opposed to traditional serial request processing, is more efficient — tasks are split up and run independently on multiple processor cores to obtain results faster, and combined at the end again to get the integral response.

It may happen that one of the inner requests in a batch returns an error. In such a case this error does not interrupt the whole batch execution and all subsequent inner requests are carried out normally.

{{% alert style="info" %}}

Since correctness is the central issue of any concurrent model, writing a concurrent batch request may not be very simple. If you want to obtain the precise faultless logic, you need to design order-independent access to files carefully.

{{% /alert %}}

### Sequential Request Processing

In some practical scenarios, it is required to execute a series of operations in a certain order step-by-step. A developer is supposed to do it by creating a chain of sequentially connected inner requests. These linked requests are executed in a definite order using the `dependsOn` property, which references the `RequestId` property of another inner request inside a batch.

To make it clear, let’s consider an example, in which we will take a document from cloud storage (request 1), remove all comments in a document (request 2) and save the output to PDF (request 3).

The batch request structure could be conditionally described by the following table:

<table>
  <tr>
    <th>#</th>
    <th>Properties</th>
  </tr>
  <tr>
    <td colspan="2"><p><strong>PUT https://api.aspose.cloud/v4.0/words/batch</strong><br>Host: api.aspose.cloud</p></td>
  </tr>
  <tr>
    <td>1</td>
    <td><p><strong>GET sample.docx?format=docx</strong><br>RequestId: request1</p></td>
  </tr>
  <tr>
    <td>2</td>
    <td><p><strong>PUT online/delete/comments</strong><br>RequestId: request2<br>DependsOn: request1<br>resultOf(request1)</p></td>
  </tr>
    <tr>
    <td>3</td>
    <td><p><strong>PUT convert?format=pdf</strong><br>DependsOn: request2<br>resultOf(request2)</p></td>
  </tr>
</table>

Note, that inner requests, as opposed to ordinary requests, should not have the https://api.aspose.cloud/v4.0/words/ prefix after the HTTP verbs, which are **GET** and **PUT** in the example. The server will reply with a multipart response containing data for every inner request. The third request will contain the resulting PDF document.

{{% alert style="info" %}}

Since there are 3 requests in a batch, the whole operation will be eventually charged as 3 requests.

{{% /alert %}}

## See Also

* [OData JSON Format Specification](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#_Toc38457781)
