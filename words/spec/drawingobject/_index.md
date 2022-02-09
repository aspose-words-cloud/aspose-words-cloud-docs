---
title: "DrawingObject"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/drawingobject/
description: "DrawingObject"
notoc: true
weight: 220
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
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Delete</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletedrawingobjectonlinerequest">DeleteDrawingObjectOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">System.IO.Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#deletedrawingobjectrequest">DeleteDrawingObjectRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="8"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentdrawingobjectbyindexonlinerequest">GetDocumentDrawingObjectByIndexOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#drawingobjectresponse">DrawingObjectResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#drawingobject">DrawingObject</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentdrawingobjectbyindexrequest">GetDocumentDrawingObjectByIndexRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentdrawingobjectimagedataonlinerequest">GetDocumentDrawingObjectImageDataOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4" colspan="2"><span style="color:SteelBlue;">System.IO.Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentdrawingobjectimagedatarequest">GetDocumentDrawingObjectImageDataRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentdrawingobjectoledataonlinerequest">GetDocumentDrawingObjectOleDataOnlineRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentdrawingobjectoledatarequest">GetDocumentDrawingObjectOleDataRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentdrawingobjectsonlinerequest">GetDocumentDrawingObjectsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#drawingobjectsresponse">DrawingObjectsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="#drawingobjectcollection">DrawingObjectCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#getdocumentdrawingobjectsrequest">GetDocumentDrawingObjectsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertdrawingobjectonlinerequest">InsertDrawingObjectOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertdrawingobjectonlineresponse">InsertDrawingObjectOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#drawingobjectinsert">DrawingObjectInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#insertdrawingobjectrequest">InsertDrawingObjectRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#drawingobjectresponse">DrawingObjectResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#drawingobject">DrawingObject</a></br><a href="#drawingobjectinsert">DrawingObjectInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Render</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#renderdrawingobjectonlinerequest">RenderDrawingObjectOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2" colspan="2"><span style="color:SteelBlue;">System.IO.Stream</span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#renderdrawingobjectrequest">RenderDrawingObjectRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatedrawingobjectonlinerequest">UpdateDrawingObjectOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatedrawingobjectonlineresponse">UpdateDrawingObjectOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#drawingobjectupdate">DrawingObjectUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="#updatedrawingobjectrequest">UpdateDrawingObjectRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#drawingobjectresponse">DrawingObjectResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="#drawingobject">DrawingObject</a></br><a href="#drawingobjectupdate">DrawingObjectUpdate</a></td>
  </tr>
  </tbody>
</table>


## DrawingObject

Represents a dTO container with a DrawingObject.

This class is inherited from [DrawingObjectLink](#drawingobjectlink) and used in [DrawingObjectResponse](#drawingobjectresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |
| Height               | <span style="color:SteelBlue;">double</span>  | Gets or sets the height of the DrawingObject in points. |
| ImageDataLink        | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to image data. Can be null if shape does not have an image. |
| Left                 | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance in points from the origin to the left side of the image. |
| OleDataLink          | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to OLE object. Can be null if shape does not have OLE data. |
| RelativeHorizontalPosition | [RelativeHorizontalPositionEnum](#drawingobject.relativehorizontalpositionenum) | Gets or sets the relative horizontal position, from which the distance to the image is measured. |
| RelativeVerticalPosition | [RelativeVerticalPositionEnum](#drawingobject.relativeverticalpositionenum) | Gets or sets the relative vertical position, from which the distance to the image is measured. |
| RenderLinks          | List&lt;[WordsApiLink](/words/spec/wordsapi#wordsapilink)&gt; | Gets or sets the list of links that originate from this DrawingObjectDto. |
| Top                  | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance in points from the origin to the top side of the image. |
| Width                | <span style="color:SteelBlue;">double</span>  | Gets or sets the width of the DrawingObjects in points. |
| WrapType             | [WrapTypeEnum](#drawingobject.wraptypeenum)   | Gets or sets the option that controls how to wrap text around the image. |


## DrawingObjectCollection

Represents a dTO container with a collection of DrawingObjects links.

This class is inherited from [LinkElement](/words/spec/link#linkelement) and used in [DrawingObjectsResponse](#drawingobjectsresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| List                 | List&lt;[LinkElement](/words/spec/link#linkelement)&gt; | Gets or sets the collection of DrawingObjects links. |


## DrawingObjectInsert

Represents a drawing object element for insert.

This class is used in [InsertDrawingObjectOnlineRequest](#insertdrawingobjectonlinerequest), [InsertDrawingObjectRequest](#insertdrawingobjectrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Height               | <span style="color:SteelBlue;">double</span>  | Gets or sets the height of the DrawingObject in points. |
| Left                 | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance in points from the origin to the left side of the image. |
| Position             | [DocumentPosition](/words/spec/document#documentposition) | Gets or sets the position, before which the DrawingObject will be inserted. |
| RelativeHorizontalPosition | [RelativeHorizontalPositionEnum](#drawingobject.relativehorizontalpositionenum) | Gets or sets the relative horizontal position, from which the distance to the image is measured. |
| RelativeVerticalPosition | [RelativeVerticalPositionEnum](#drawingobject.relativeverticalpositionenum) | Gets or sets the relative vertical position, from which the distance to the image is measured. |
| Top                  | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance in points from the origin to the top side of the image. |
| Width                | <span style="color:SteelBlue;">double</span>  | Gets or sets the width of the DrawingObjects in points. |
| WrapType             | [WrapTypeEnum](#drawingobject.wraptypeenum)   | Gets or sets the option indicating how to wrap text around the image. |


## DrawingObjectLink

Represents a link for Drawing Object DTO.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |


## DrawingObjectUpdate

Represents a drawing object element for update.

This class is used in [UpdateDrawingObjectOnlineRequest](#updatedrawingobjectonlinerequest), [UpdateDrawingObjectRequest](#updatedrawingobjectrequest).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Height               | <span style="color:SteelBlue;">double</span>  | Gets or sets the height of the DrawingObject in points. |
| Left                 | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance in points from the origin to the left side of the image. |
| RelativeHorizontalPosition | [RelativeHorizontalPositionEnum](#drawingobject.relativehorizontalpositionenum) | Gets or sets the relative horizontal position, from which the distance to the image is measured. |
| RelativeVerticalPosition | [RelativeVerticalPositionEnum](#drawingobject.relativeverticalpositionenum) | Gets or sets the relative vertical position, from which the distance to the image measured. |
| Top                  | <span style="color:SteelBlue;">double</span>  | Gets or sets the distance in points from the origin to the top side of the image. |
| Width                | <span style="color:SteelBlue;">double</span>  | Gets or sets the width of the DrawingObjects in points. |
| WrapType             | [WrapTypeEnum](#drawingobject.wraptypeenum)   | Gets or sets the option that controls how to wrap text around the image. |


## DrawingObjectsResponse

Represents a REST response with a collection of DrawingObjects.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| DrawingObjects       | [DrawingObjectCollection](#drawingobjectcollection) | Gets or sets the collection of DrawingObjects. |


## DeleteDrawingObjectOnlineRequest

Represents a request model for [WordsApi.DeleteDrawingObjectOnline()](/words/drawing-objects/delete/) operation.

An object of the **DeleteDrawingObjectOnlineRequest** class is created by the following constructor methods:

- DeleteDrawingObjectOnlineRequest()
- DeleteDrawingObjectOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DeleteDrawingObjectRequest

Represents a request model for [WordsApi.DeleteDrawingObject()](/words/drawing-objects/delete/) operation.

An object of the **DeleteDrawingObjectRequest** class is created by the following constructor methods:

- DeleteDrawingObjectRequest()
- DeleteDrawingObjectRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DrawingObjectResponse

Represents a REST response with a DrawingObject.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi), [InsertDrawingObjectOnlineResponse](#insertdrawingobjectonlineresponse), [UpdateDrawingObjectOnlineResponse](#updatedrawingobjectonlineresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| DrawingObject        | [DrawingObject](#drawingobject)               | Gets or sets the DrawingObject. |


## GetDocumentDrawingObjectByIndexOnlineRequest

Represents a request model for [WordsApi.GetDocumentDrawingObjectByIndexOnline()](/words/drawing-objects/get/) operation.

An object of the **GetDocumentDrawingObjectByIndexOnlineRequest** class is created by the following constructor methods:

- GetDocumentDrawingObjectByIndexOnlineRequest()
- GetDocumentDrawingObjectByIndexOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentDrawingObjectByIndexRequest

Represents a request model for [WordsApi.GetDocumentDrawingObjectByIndex()](/words/drawing-objects/get/) operation.

An object of the **GetDocumentDrawingObjectByIndexRequest** class is created by the following constructor methods:

- GetDocumentDrawingObjectByIndexRequest()
- GetDocumentDrawingObjectByIndexRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentDrawingObjectImageDataOnlineRequest

Represents a request model for [WordsApi.GetDocumentDrawingObjectImageDataOnline()](/words/drawing-objects/get-image-data/) operation.

An object of the **GetDocumentDrawingObjectImageDataOnlineRequest** class is created by the following constructor methods:

- GetDocumentDrawingObjectImageDataOnlineRequest()
- GetDocumentDrawingObjectImageDataOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentDrawingObjectImageDataRequest

Represents a request model for [WordsApi.GetDocumentDrawingObjectImageData()](/words/drawing-objects/get-image-data/) operation.

An object of the **GetDocumentDrawingObjectImageDataRequest** class is created by the following constructor methods:

- GetDocumentDrawingObjectImageDataRequest()
- GetDocumentDrawingObjectImageDataRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentDrawingObjectOleDataOnlineRequest

Represents a request model for [WordsApi.GetDocumentDrawingObjectOleDataOnline()](/words/drawing-objects/get-ole-file/) operation.

An object of the **GetDocumentDrawingObjectOleDataOnlineRequest** class is created by the following constructor methods:

- GetDocumentDrawingObjectOleDataOnlineRequest()
- GetDocumentDrawingObjectOleDataOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentDrawingObjectOleDataRequest

Represents a request model for [WordsApi.GetDocumentDrawingObjectOleData()](/words/drawing-objects/get-ole-file/) operation.

An object of the **GetDocumentDrawingObjectOleDataRequest** class is created by the following constructor methods:

- GetDocumentDrawingObjectOleDataRequest()
- GetDocumentDrawingObjectOleDataRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentDrawingObjectsOnlineRequest

Represents a request model for [WordsApi.GetDocumentDrawingObjectsOnline()](/words/drawing-objects/get-all/) operation.

An object of the **GetDocumentDrawingObjectsOnlineRequest** class is created by the following constructor methods:

- GetDocumentDrawingObjectsOnlineRequest()
- GetDocumentDrawingObjectsOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## GetDocumentDrawingObjectsRequest

Represents a request model for [WordsApi.GetDocumentDrawingObjects()](/words/drawing-objects/get-all/) operation.

An object of the **GetDocumentDrawingObjectsRequest** class is created by the following constructor methods:

- GetDocumentDrawingObjectsRequest()
- GetDocumentDrawingObjectsRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |



## InsertDrawingObjectOnlineRequest

Represents a request model for [WordsApi.InsertDrawingObjectOnline()](/words/drawing-objects/add/) operation.

An object of the **InsertDrawingObjectOnlineRequest** class is created by the following constructor methods:

- InsertDrawingObjectOnlineRequest()
- InsertDrawingObjectOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [DrawingObjectInsert](#drawingobjectinsert) ***drawingObject***, <span style="color:SteelBlue;">Stream</span> ***imageFile***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***drawingObject***  | DrawingObject        | [DrawingObjectInsert](#drawingobjectinsert)   | Drawing object parameters. |
| ***imageFile***      | ImageFile            | <span style="color:SteelBlue;">Stream</span>  | File with image. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## InsertDrawingObjectOnlineResponse

Represents a response model for [WordsApi.InsertDrawingObjectOnline()](/words/drawing-objects/add/) operation.

An object of the **InsertDrawingObjectOnlineResponse** class is created by the following constructor methods:

- InsertDrawingObjectOnlineResponse([DrawingObjectResponse](#drawingobjectresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DrawingObjectResponse](#drawingobjectresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## InsertDrawingObjectRequest

Represents a request model for [WordsApi.InsertDrawingObject()](/words/drawing-objects/add/) operation.

An object of the **InsertDrawingObjectRequest** class is created by the following constructor methods:

- InsertDrawingObjectRequest()
- InsertDrawingObjectRequest(<span style="color:SteelBlue;">string</span> ***name***, [DrawingObjectInsert](#drawingobjectinsert) ***drawingObject***, <span style="color:SteelBlue;">Stream</span> ***imageFile***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***drawingObject***  | DrawingObject        | [DrawingObjectInsert](#drawingobjectinsert)   | Drawing object parameters. |
| ***imageFile***      | ImageFile            | <span style="color:SteelBlue;">Stream</span>  | File with image. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## RenderDrawingObjectOnlineRequest

Represents a request model for [WordsApi.RenderDrawingObjectOnline()](/words/documents/render-into-image/) operation.

An object of the **RenderDrawingObjectOnlineRequest** class is created by the following constructor methods:

- RenderDrawingObjectOnlineRequest()
- RenderDrawingObjectOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, <span style="color:SteelBlue;">string</span> ***format***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *fontsLocation*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***format***         | Format               | <span style="color:SteelBlue;">string</span>  | The destination format. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *fontsLocation*      | FontsLocation        | <span style="color:SteelBlue;">string</span>  | Folder in filestorage with custom fonts. |



## RenderDrawingObjectRequest

Represents a request model for [WordsApi.RenderDrawingObject()](/words/documents/render-into-image/) operation.

An object of the **RenderDrawingObjectRequest** class is created by the following constructor methods:

- RenderDrawingObjectRequest()
- RenderDrawingObjectRequest(<span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">string</span> ***format***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *fontsLocation*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***format***         | Format               | <span style="color:SteelBlue;">string</span>  | The destination format. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *fontsLocation*      | FontsLocation        | <span style="color:SteelBlue;">string</span>  | Folder in filestorage with custom fonts. |



## UpdateDrawingObjectOnlineRequest

Represents a request model for [WordsApi.UpdateDrawingObjectOnline()](/words/drawing-objects/update/) operation.

An object of the **UpdateDrawingObjectOnlineRequest** class is created by the following constructor methods:

- UpdateDrawingObjectOnlineRequest()
- UpdateDrawingObjectOnlineRequest(<span style="color:SteelBlue;">Stream</span> ***document***, [DrawingObjectUpdate](#drawingobjectupdate) ***drawingObject***, <span style="color:SteelBlue;">Stream</span> ***imageFile***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document. |
| ***drawingObject***  | DrawingObject        | [DrawingObjectUpdate](#drawingobjectupdate)   | Drawing object parameters. |
| ***imageFile***      | ImageFile            | <span style="color:SteelBlue;">Stream</span>  | File with image. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## UpdateDrawingObjectOnlineResponse

Represents a response model for [WordsApi.UpdateDrawingObjectOnline()](/words/drawing-objects/update/) operation.

An object of the **UpdateDrawingObjectOnlineResponse** class is created by the following constructor methods:

- UpdateDrawingObjectOnlineResponse([DrawingObjectResponse](#drawingobjectresponse) ***model***, <span style="color:SteelBlue;">Stream</span> ***document***)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***model***          | Model                | [DrawingObjectResponse](#drawingobjectresponse) | The response model. |
| ***document***       | Document             | <span style="color:SteelBlue;">Stream</span>  | The document after modification. |



## UpdateDrawingObjectRequest

Represents a request model for [WordsApi.UpdateDrawingObject()](/words/drawing-objects/update/) operation.

An object of the **UpdateDrawingObjectRequest** class is created by the following constructor methods:

- UpdateDrawingObjectRequest()
- UpdateDrawingObjectRequest(<span style="color:SteelBlue;">string</span> ***name***, [DrawingObjectUpdate](#drawingobjectupdate) ***drawingObject***, <span style="color:SteelBlue;">Stream</span> ***imageFile***, <span style="color:SteelBlue;">int</span> ***index***, <span style="color:SteelBlue;">string</span> *nodePath*, <span style="color:SteelBlue;">string</span> *folder*, <span style="color:SteelBlue;">string</span> *storage*, <span style="color:SteelBlue;">string</span> *loadEncoding*, <span style="color:SteelBlue;">string</span> *password*, <span style="color:SteelBlue;">string</span> *encryptedPassword*, <span style="color:SteelBlue;">string</span> *destFileName*, <span style="color:SteelBlue;">string</span> *revisionAuthor*, <span style="color:SteelBlue;">string</span> *revisionDateTime*)

Each of those arguments initializes the corresponding self-titled property:

| Argument             | Property             | Type                                          | Description |
|----------------------|----------------------|-----------------------------------------------|-------------|
| ***name***           | Name                 | <span style="color:SteelBlue;">string</span>  | The filename of the input document. |
| ***drawingObject***  | DrawingObject        | [DrawingObjectUpdate](#drawingobjectupdate)   | Drawing object parameters. |
| ***imageFile***      | ImageFile            | <span style="color:SteelBlue;">Stream</span>  | File with image. |
| ***index***          | Index                | <span style="color:SteelBlue;">int</span>     | Object index. |
| *nodePath*           | NodePath             | <span style="color:SteelBlue;">string</span>  | The path to the node in the document tree. |
| *folder*             | Folder               | <span style="color:SteelBlue;">string</span>  | Original document folder. |
| *storage*            | Storage              | <span style="color:SteelBlue;">string</span>  | Original document storage. |
| *loadEncoding*       | LoadEncoding         | <span style="color:SteelBlue;">string</span>  | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| *password*           | Password             | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| *encryptedPassword*  | EncryptedPassword    | <span style="color:SteelBlue;">string</span>  | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| *destFileName*       | DestFileName         | <span style="color:SteelBlue;">string</span>  | Result path of the document after the operation. If this parameter is omitted then result of the operation will be saved as the source document. |
| *revisionAuthor*     | RevisionAuthor       | <span style="color:SteelBlue;">string</span>  | Initials of the author to use for revisions.If you set this parameter and then make some changes to the document programmatically, save the document and later open the document in MS Word you will see these changes as revisions. |
| *revisionDateTime*   | RevisionDateTime     | <span style="color:SteelBlue;">string</span>  | The date and time to use for revisions. |



## DrawingObject.RelativeHorizontalPositionEnum

The following values are defined: Margin, Page, Column, Default, Character, LeftMargin, RightMargin, InsideMargin, OutsideMargin.


## DrawingObject.RelativeVerticalPositionEnum

The following values are defined: Margin, TableDefault, Page, Paragraph, TextFrameDefault, Line, TopMargin, BottomMargin, InsideMargin, OutsideMargin.


## DrawingObject.WrapTypeEnum

The following values are defined: Inline, TopBottom, Square, None, Tight, Through.


## DrawingObjectInsert.RelativeHorizontalPositionEnum

The following values are defined: Margin, Page, Column, Default, Character, LeftMargin, RightMargin, InsideMargin, OutsideMargin.


## DrawingObjectInsert.RelativeVerticalPositionEnum

The following values are defined: Margin, TableDefault, Page, Paragraph, TextFrameDefault, Line, TopMargin, BottomMargin, InsideMargin, OutsideMargin.


## DrawingObjectInsert.WrapTypeEnum

The following values are defined: Inline, TopBottom, Square, None, Tight, Through.


## DrawingObjectUpdate.RelativeHorizontalPositionEnum

The following values are defined: Margin, Page, Column, Default, Character, LeftMargin, RightMargin, InsideMargin, OutsideMargin.


## DrawingObjectUpdate.RelativeVerticalPositionEnum

The following values are defined: Margin, TableDefault, Page, Paragraph, TextFrameDefault, Line, TopMargin, BottomMargin, InsideMargin, OutsideMargin.


## DrawingObjectUpdate.WrapTypeEnum

The following values are defined: Inline, TopBottom, Square, None, Tight, Through.

