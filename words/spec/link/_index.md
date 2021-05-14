---
title: "Link"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/link/
description: "Link"
notoc: true
weight: 290
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
  </tbody>
</table>


## FileLink

Represents a provides information for the file link.

This class is inherited from [Link](/words/spec/document#link) and used in [ModificationOperationResult](/words/spec/documentrevision#modificationoperationresult), [ProtectionDataResponse](/words/spec/documentprotection#protectiondataresponse), [ReplaceTextResponse](/words/spec/text#replacetextresponse), [SaveResult](/words/spec/document#saveresult), [SplitDocumentResult](/words/spec/document#splitdocumentresult), [StatDataResponse](/words/spec/documentstatistics#statdataresponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Href                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the "href" attribute with the link's IRI. atom:link elements MUST have an href attribute, whose value MUST be a IRI reference. |
| Rel                  | <span style="color:SteelBlue;">string</span>  | Gets or sets the option that controls whether atom:link elements MAY have a "rel" attribute that indicates the link relation type. If the "rel" attribute is not present, the link element MUST be interpreted as if the link relation type is "alternate". |
| Title                | <span style="color:SteelBlue;">string</span>  | Gets or sets the "title" attribute, that conveys human-readable information about the link. The content of the "title" attribute is Language-Sensitive. |
| Type                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the "type" attribute. The "type" attribute's value is an advisory media type: it is a hint about the type of the representation that is expected to be returned when the value of the href attribute is dereferenced. Note that the type attribute does not override the actual media type returned with the representation. |


## LinkElement

Represents a reference to a document.

This class is used in [DrawingObjectCollection](/words/spec/drawingobject#drawingobjectcollection), [HeaderFooter](/words/spec/headerfooter#headerfooter), [Section](/words/spec/section#section).

A single `Link` property is defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |


## NodeLink

Represents a reference to node.

This class is inherited from [LinkElement](#linkelement) and used in [DocumentPosition](/words/spec/document#documentposition), [HeaderFooter](/words/spec/headerfooter#headerfooter), [Paragraph](/words/spec/paragraph#paragraph), [Section](/words/spec/section#section), [StoryChildNodes](/words/spec/document#storychildnodes), [TableCell](/words/spec/tablecell#tablecell).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |


## OfficeMathLink

Represents a officeMath object link element.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Link                 | [WordsApiLink](/words/spec/wordsapi#wordsapilink) | Gets or sets the link to the document. |
| NodeId               | <span style="color:SteelBlue;">string</span>  | Gets or sets the node id. |

