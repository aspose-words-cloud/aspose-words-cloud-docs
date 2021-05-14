---
title: "DocumentClassification"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/documentclassification/
description: "DocumentClassification"
notoc: true
weight: 150
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="3"><strong><i>Classify</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#classifydocumentonlinerequest">ClassifyDocumentOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="3"><a href="#classificationresponse">ClassificationResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="3"><a href="#classificationresult">ClassificationResult</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#classifydocumentrequest">ClassifyDocumentRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#classifyrequest">ClassifyRequest</a></td>
  </tr>
  </tbody>
</table>


## ClassificationResult

Represents a single classification result.

This class is used in [ClassificationResponse](#classificationresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ClassName            | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the class. |
| ClassProbability     | <span style="color:SteelBlue;">double</span>  | Gets or sets the probability of class. |


## ClassificationResponse

Represents a REST response with data on multi-class text classification.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| BestClassName        | <span style="color:SteelBlue;">string</span>  | Gets or sets the best class name. |
| BestClassProbability | <span style="color:SteelBlue;">double</span>  | Gets or sets the best class probability. |
| BestResults          | List&lt;[ClassificationResult](#classificationresult)&gt; | Gets or sets the array of best classes results. |


## ClassifyDocumentOnlineRequest

Represents a request model for [WordsApi.ClassifyDocumentOnline()](/words/classification/document) operation.

An object of the **ClassifyDocumentOnlineRequest** class is created by the following constructor methods:

- ClassifyDocumentOnlineRequest()
- ClassifyDocumentOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *bestClassesCount*, <span style="color:SteelBlue;">string</span> *taxonomy*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *bestClassesCount*   | BestClassesCount     | <span style="color:SteelBlue;">string</span>  | The number of the best classes to return. |
| *taxonomy*           | Taxonomy             | <span style="color:SteelBlue;">string</span>  | The taxonomy to use. |



## ClassifyDocumentRequest

Represents a request model for [WordsApi.ClassifyDocument()](/words/classification/document) operation.

An object of the **ClassifyDocumentRequest** class is created by the following constructor methods:

- ClassifyDocumentRequest()
- ClassifyDocumentRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *bestClassesCount*, <span style="color:SteelBlue;">string</span> *taxonomy*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The document name. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |
| *bestClassesCount*   | BestClassesCount     | <span style="color:SteelBlue;">string</span>  | The number of the best classes to return. |
| *taxonomy*           | Taxonomy             | <span style="color:SteelBlue;">string</span>  | The taxonomy to use. |



## ClassifyRequest

Represents a request model for [WordsApi.Classify()](/words/classification/text) operation.

An object of the **ClassifyRequest** class is created by the following constructor methods:

- ClassifyRequest()
- ClassifyRequest(<span style="color:SteelBlue;">string</span> ***text***, <span style="color:SteelBlue;">string</span> *bestClassesCount*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***text***           | Text                 | <span style="color:SteelBlue;">string</span>  | The text to classify. |
| *bestClassesCount*   | BestClassesCount     | <span style="color:SteelBlue;">string</span>  | The number of the best classes to return. |


