---
title: "Batch"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/batch/
description: "Batch"
notoc: true
weight: 100
---


<table>
  <thead>
    <tr>
      <th style="text-align:center;"></th>
      <th><i>Request</i></th>
      <th><i>Response</i></th>
      <th><i>Model</i></th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><strong><i></i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#batchpartrequest">BatchPartRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">object</span></td>
    <td style="vertical-align:middle;" class="bg-white"></td>
  </tr>
  </tbody>
</table>


## BatchPartRequest

Represents a IRequestModel wrapper to add batch part features.

This class is used in [WordsApi](/words/spec/wordsapi#wordsapi).

An object of the **BatchPartRequest** class is created by the following constructor methods:

- BatchPartRequest([IRequestModel](/words/spec/other#irequestmodel) ***request***)

### Properties

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets request ID. |
| ParentRequestId      | <span style="color:SteelBlue;">string</span>  | Gets or sets parent request ID. |

### Methods

- <span style="color:SteelBlue;">Stream</span> **UseAsSource**() - use a binary response of the request as an input for another request.

