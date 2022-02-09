---
title: "Range"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/range/
description: "Range"
notoc: true
weight: 400
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getrangetextonlinerequest">GetRangeTextOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2" colspan="2"><a href="#rangetextresponse">RangeTextResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="3"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getrangetextrequest">GetRangeTextRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Remove</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#removerangeonlinerequest">RemoveRangeOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><a href="#removerangeonlineresponse">RemoveRangeOnlineResponse</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#removerangerequest">RemoveRangeRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#documentresponse">DocumentResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/document#document">Document</a></td>
  </tr>
  </tbody>
</table>


## RangeDocumentDto

Represents a dTO container with a Range element.

A single `DocumentName` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| DocumentName         | <span style="color:SteelBlue;">string</span>  | Gets or sets the name for a new document. |


## ReplaceRangeDto

Represents a dTO container with a range element.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the range's text. |
| TextType             | [TextTypeEnum](#replacerange.texttypeenum)    | Gets or sets the range's text type. |


## RangeTextResponse

Represents a REST response with a range's text.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Text                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the range's text. |


## GetRangeTextOnlineRequest

Represents a request model for [WordsApi.GetRangeTextOnline()](/words/range/) operation.

An object of the **GetRangeTextOnlineRequest** class is created by the following constructor methods:

- GetRangeTextOnlineRequest()
- GetRangeTextOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***rangeStartIdentifier***, <span style="color:SteelBlue;">string</span> *rangeEndIdentifier*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***rangeStartIdentifier*** | RangeStartIdentifier | <span style="color:SteelBlue;">string</span>  | The range start identifier. |
| *rangeEndIdentifier* | RangeEndIdentifier   | <span style="color:SteelBlue;">string</span>  | The range end identifier. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetRangeTextRequest

Represents a request model for [WordsApi.GetRangeText()](/words/range/) operation.

An object of the **GetRangeTextRequest** class is created by the following constructor methods:

- GetRangeTextRequest()
- GetRangeTextRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***rangeStartIdentifier***, <span style="color:SteelBlue;">string</span> *rangeEndIdentifier*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***rangeStartIdentifier*** | RangeStartIdentifier | <span style="color:SteelBlue;">string</span>  | The range start identifier. |
| *rangeEndIdentifier* | RangeEndIdentifier   | <span style="color:SteelBlue;">string</span>  | The range end identifier. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## RemoveRangeOnlineRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **RemoveRangeOnlineRequest** class is created by the following constructor methods:

- RemoveRangeOnlineRequest()
- RemoveRangeOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***rangeStartIdentifier***, <span style="color:SteelBlue;">string</span> *rangeEndIdentifier*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***rangeStartIdentifier*** | RangeStartIdentifier | <span style="color:SteelBlue;">string</span>  | The range start identifier. |
| *rangeEndIdentifier* | RangeEndIdentifier   | <span style="color:SteelBlue;">string</span>  | The range end identifier. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## RemoveRangeOnlineResponse

Represents a response model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.

An object of the **RemoveRangeOnlineResponse** class is created by the following constructor methods:

- RemoveRangeOnlineResponse([DocumentResponse](/words/spec/document#documentresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DocumentResponse](/words/spec/document#documentresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## RemoveRangeRequest

Represents a request model for [WordsApi.RemoveRange()](/words/range/) operation.

An object of the **RemoveRangeRequest** class is created by the following constructor methods:

- RemoveRangeRequest()
- RemoveRangeRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***rangeStartIdentifier***, <span style="color:SteelBlue;">string</span> *rangeEndIdentifier*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***rangeStartIdentifier*** | RangeStartIdentifier | <span style="color:SteelBlue;">string</span>  | The range start identifier. |
| *rangeEndIdentifier* | RangeEndIdentifier   | <span style="color:SteelBlue;">string</span>  | The range end identifier. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |



## ReplaceRange.TextTypeEnum

The following values are defined: Text, Html.


## ReplaceRangeDto.TextTypeEnum

The following values are defined: Text, Html.

