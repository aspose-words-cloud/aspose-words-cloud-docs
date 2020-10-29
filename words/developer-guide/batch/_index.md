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

To address these needs, Aspose.Words Cloud API provides the Batch Request feature designed to group multiple REST API requests into a single request. This technique can minimize the intensity of client-server interactions and provide the top speed of document processing at the same time.

## Batch Request Processing Model

Batch processing is commonly defined as "processing a number of cases simultaneously". The basic logic behind Batch Request processing is presented in the diagram below.

![batch.png](batch.png)

The batching technique comprises both concurrent and sequential request processing, where concurrent requests can be processed in an arbitrary order with the same result, and sequential requests depend on being processed step-by-step.

There is no restriction on the number of inner requests inside a single batch request. When processing of all operations in a batch is completed, a consolidated response is returned and the HTTPS connection is closed.

### Concurrent Request Processing

In a general case batch requests are processed concurrently. Parallel processing, as opposed to traditional serial request processing, is more efficient — tasks are split up and run independently on multiple processor cores to obtain results faster, and combined at the end again to get the integral response.

It may happen that one of the inner calls in a batch returns an error. In such a case this error does not interrupt the whole batch execution and all subsequent inner requests are carried out normally.

{{% alert style="info" %}}

Since correctness is the central issue of any concurrent model, writing a concurrent batch request may not be very simple. If you want to obtain the precise faultless processing logic, you need to design order-independent access to cloud storage files carefully.

{{% /alert %}}

### Sequential Request Processing

In some practical scenarios it is required to execute a series of operations in a certain order step-by-step. A developer is supposed to do it by creating a chain of sequentially connected inner requests, using the ***dependsOn*** parameter.

Sequential request processing is currently under development and will be activated in the immediate future.

## See Also

* [OData JSON Format Specification](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#_Toc38457781)
