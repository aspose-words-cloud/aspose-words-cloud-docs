---
title: "Range"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /range/
aliases: [/working-with-range/]
description: "Learn how to work with a Range in a Word document"
weight: 210
---

The concept of Range is similar to [Range Object in MS Word API](https://docs.microsoft.com/en-us/office/vba/word/Concepts/Working-with-Word/working-with-range-objects). Working with a range is much closer to how a user interacts with a document in MS Word.

A range is basically a contiguous area in a document. It is signified as a pair of positions (START, END), where a coordinate of START always less than a coordinate of END. It may span across multiple sections, paragraphs, etc., in other words, across different nodes of the [DOM tree](https://docs.aspose.com/display/wordsnet/Aspose.Words+Document+Object+Model). Thus, a user can ignore the underlying model of the document. Such an approach is going to make the usage of API much more friendly.

## Ways to Specify a Range

A range can be specified in one of the three ways:

### Position in a document based on nodes IDs

```HTML
/range/{startId}/{endId}
```

, where:

- *{startId}* - id of the node from which the range starts (included). Required.
- *{endId}* - id of the node at which the range ends (excluded). Optional. If missed, the end of the range corresponds to the end of the node with id = startId, i.e. the range is limited by the bounds of "startId node".

The following is an example of a range consisting of the second and third paragraphs:

```HTML
/range/id0.1/id0.3
```

### Position in a document based on nodes pseudo names

```HTML
/range/{startPseudoName}/{endPseudoName}
```

, where:

- *{startPseudoName}* - a pseudo name of the node from which the range starts (included). Required.
- *{endPseudoName}* - a pseudo name of the node at which the range ends (excluded). Optional. If missed, the end of the range corresponds to the end of the node with pseudoname = startPseudoName, i.e. the range is limited by the bounds of "startPseudoName node".

The following **PseudoNames** are available:

- *TableN* for tables.
- *ImageN* for images.

An example of a range, consisting of the text from the first table and after the table till the second table, is presented below:

```HTML
/range/table0/table1
```

### Positions inside nodes

A certain position inside a node can be specified with a selector that is separated from a node identifier with a colon.

```HTML
/range/{startIdentifier}:{startSelector}/{endIdentifier}:{endSelector}
```

, where:

- *{startIdentifier}* - an identifier (id or a pseudo name) of the node from which the range starts (included). Required.
- *{endIdentifier}* - an identifier (id or a pseudo name) of the node at which the range ends (excluded). Optional. If missed, the end of the range corresponds to the end of the node with identifier = startIdentifier, i.e. the range is limited by the bounds of "startIdentifier node".
- *{startSelector}* - a selector that specifies a certain position inside the start node (included). Optional. If missed, the start of the range corresponds to the beginning of the start node.
- *{endSelector}* - a selector that specifies a certain position inside the end node (excluded). Optional. If missed, the end of the range corresponds to the element before the beginning of the end node.

Selectors cannot be used without a node identifier.

The following **Selectors** are available:

- *end* - specifies the end of the node ("end" here is supposed to be a virtual node after the last child node, i.e. it means that the whole content of the node should be included for an end node).

An example of a range, consisting of all nodes starting from the end of the 1st table till the beginning of the 6th paragraph, is presented below:

```HTML
/range/table0:end/id0.5
```

## Operations with a Range

The following operations can be defined on a range:

### Get the text from the range

Get the text from all nodes in the range. You may use one of the following two APIs to get the text from the range:

- [GET /words/{name}/range/{rangeStartIdentifier}/{rangeEndIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/GetRangeText).
- [GET /words/{name}/range/{rangeStartIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/GetRangeText2).

### Remove the text from the range

With the following APIs you can remove the text from the range. Text from all nodes inside the range would be removed.

- [DELETE /words/{name}/range/{rangeStartIdentifier}/{rangeEndIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/RemoveRange).
- [DELETE /words/{name}/range/{rangeStartIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/RemoveRange2).

### Replace the content in the range

The replacement should be done according to MS Word rules. For example, several nodes, except the case when all nodes are runs of one paragraph, should be replaced with one new paragraph. However, several runs in one paragraph should be replaced with the new run(s). The style should be consistent to removed nodes.

Content in the range can be replaced with one of the following two APIs:

- [POST /words/{name}/range/{rangeStartIdentifier}/{rangeEndIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/ReplaceWithText).
- [POST /words/{name}/range/{rangeStartIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/ReplaceWithText2).

### Save the selected range as a new document

The range should be saved as a separate document. The original document must not be changed. The said task can be achieved with one of the following two APIs:

- [POST /words/{name}/range/{rangeStartIdentifier}/{rangeEndIdentifier}/SaveAs](https://apireference.aspose.cloud/words/#/RangeApi/SaveAsRange).
- [POST /words/{name}/range/{rangeStartIdentifier}/SaveAs](https://apireference.aspose.cloud/words/#/RangeApi/SaveAsRange2).

