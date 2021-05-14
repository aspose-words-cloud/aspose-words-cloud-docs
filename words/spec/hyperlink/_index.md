---
title: "Hyperlink"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/hyperlink/
description: "Hyperlink"
notoc: true
weight: 280
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumenthyperlinkbyindexonlinerequest">GetDocumentHyperlinkByIndexOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#hyperlinkresponse">HyperlinkResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#hyperlink">Hyperlink</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumenthyperlinkbyindexrequest">GetDocumentHyperlinkByIndexRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumenthyperlinksonlinerequest">GetDocumentHyperlinksOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#hyperlinksresponse">HyperlinksResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#hyperlinks">Hyperlinks</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumenthyperlinksrequest">GetDocumentHyperlinksRequest</a></td>
  </tr>
  </tbody>
</table>


## Hyperlink

Represents a hyperlink element.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [HyperlinkResponse](#hyperlinkresponse), [Hyperlinks](#hyperlinks).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| DisplayText          | <span style="color:SteelBlue;">string</span>  | Gets or sets the hypelink's display text. |
| Value                | <span style="color:SteelBlue;">string</span>  | Gets or sets the value. |


## Hyperlinks

Represents a collection of Hyperlink.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [HyperlinksResponse](#hyperlinksresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| HyperlinkList        | List&lt;[Hyperlink](#hyperlink)&gt;           | Gets or sets the array of Hyperlink. |


## HyperlinkResponse

Represents a REST response with a hyperlink.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Hyperlink            | [Hyperlink](#hyperlink)                       | Gets or sets the hyperlink. |


## HyperlinksResponse

Represents a REST response with a collection of hyperlinks.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Hyperlinks           | [Hyperlinks](#hyperlinks)                     | Gets or sets the collection of hyperlinks. |


## GetDocumentHyperlinkByIndexOnlineRequest

Represents a request model for [WordsApi.GetDocumentHyperlinkByIndexOnline()](/words/hyperlinks/get/) operation.

An object of the **GetDocumentHyperlinkByIndexOnlineRequest** class is created by the following constructor methods:

- GetDocumentHyperlinkByIndexOnlineRequest()
- GetDocumentHyperlinkByIndexOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***hyperlinkIndex***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***hyperlinkIndex*** | HyperlinkIndex       | <span style="color:SteelBlue;">int</span>     | The index of the hyperlink. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetDocumentHyperlinkByIndexRequest

Represents a request model for [WordsApi.GetDocumentHyperlinkByIndex()](/words/hyperlinks/get/) operation.

An object of the **GetDocumentHyperlinkByIndexRequest** class is created by the following constructor methods:

- GetDocumentHyperlinkByIndexRequest()
- GetDocumentHyperlinkByIndexRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***hyperlinkIndex***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***hyperlinkIndex*** | HyperlinkIndex       | <span style="color:SteelBlue;">int</span>     | The index of the hyperlink. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetDocumentHyperlinksOnlineRequest

Represents a request model for [WordsApi.GetDocumentHyperlinksOnline()](/words/hyperlinks/get-all/) operation.

An object of the **GetDocumentHyperlinksOnlineRequest** class is created by the following constructor methods:

- GetDocumentHyperlinksOnlineRequest()
- GetDocumentHyperlinksOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |



## GetDocumentHyperlinksRequest

Represents a request model for [WordsApi.GetDocumentHyperlinks()](/words/hyperlinks/get-all/) operation.

An object of the **GetDocumentHyperlinksRequest** class is created by the following constructor methods:

- GetDocumentHyperlinksRequest()
- GetDocumentHyperlinksRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password for opening an encrypted document. |


