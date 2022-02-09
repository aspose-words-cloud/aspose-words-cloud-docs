---
title: "Other"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/other/
description: "Other"
notoc: true
weight: 340
---


## InfoAdditionalItem

Represents a info additional item.

This class is used in [InfoResponse](#inforesponse).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| Key                  | <span style="color:SteelBlue;">string</span>  | Gets or sets Key. |
| Value                | <span style="color:SteelBlue;">string</span>  | Gets or sets Value. |


## IRequestModel

Represents a common request for operations.


## ICanModifyDocumentRequest

Represents a request which can modify document.


## ICanSaveRevisionRequest

Represents a request which can save revisions in document.


## ICanSpecifyMailMergeParametersRequest

Represents a request for mail merge operations.


## ICanSpecifyOutputFormatRequest

Represents a request with format of output document.


## ICanUseCustomFontsRequest

Represents a request which can use custom fonts.


## InfoResponse

Represents a response with API info.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| AdditionalInfo       | List&lt;[InfoAdditionalItem](#infoadditionalitem)&gt; | Gets or sets additional info. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets application name. |
| Version              | <span style="color:SteelBlue;">string</span>  | Gets or sets version. |


## IPutExecuteRequest

Represents a interface to specify template and body for putexecute operations.


## IWordDocumentRequest

Represents a request for operation with word document.


## PublicKeyResponse

Represents a rEST response for RSA public key info.

This class is inherited from [WordsResponse](/words/spec/style#wordsresponse) and used in [WordsApi](/words/spec/wordsapi#wordsapi).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| RequestId            | <span style="color:SteelBlue;">string</span>  | Gets or sets the request Id. |
| Exponent             | <span style="color:SteelBlue;">string</span>  | Gets or sets RSA key exponent as Base64 string. |
| Modulus              | <span style="color:SteelBlue;">string</span>  | Gets or sets RSA key modulus as Base64 string. |


## GetInfoRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.


## GetPublicKeyRequest

Represents a request model for [WordsApi](/words/spec/wordsapi#wordsapi) operation.


## HeaderFooterNodePathBuilder

Represents a node path builder for headers / footers.

This class is inherited from [NodePathBuilderBase](#nodepathbuilderbase) and used in [SectionNodePathBuilder](#sectionnodepathbuilder).

An object of the **HeaderFooterNodePathBuilder** class is created by the following constructor methods:

- HeaderFooterNodePathBuilder([NodePathBuilderBase](#nodepathbuilderbase) ***parentBuilder***, <span style="color:SteelBlue;">int</span> ***index***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***parentBuilder***  | [NodePathBuilderBase](#nodepathbuilderbase)   | parent node path builder. |
| ***index***          | <span style="color:SteelBlue;">int</span>     | element node index. |


### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.
- [ParagraphNodePathBuilder](#paragraphnodepathbuilder) **Paragraphs**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for paragraph node.


## ListNodePathBuilder

Represents a node path builder for document lists.

This class is inherited from [NodePathBuilderBase](#nodepathbuilderbase) and used in [SectionBodyNodePathBuilder](#sectionbodynodepathbuilder), [SectionNodePathBuilder](#sectionnodepathbuilder).

An object of the **ListNodePathBuilder** class is created by the following constructor methods:

- ListNodePathBuilder([NodePathBuilderBase](#nodepathbuilderbase) ***parentBuilder***, <span style="color:SteelBlue;">int</span> ***index***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***parentBuilder***  | [NodePathBuilderBase](#nodepathbuilderbase)   | parent node path builder. |
| ***index***          | <span style="color:SteelBlue;">int</span>     | element node index. |


### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.
- [SimpleNodePathBuilder](#simplenodepathbuilder) **Levels**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for list level node collection.


## NodePathBuilderBase

Represents a base class for all node path builder.

### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.


## ParagraphNodePathBuilder

Represents a node path builder for paragraphs.

This class is inherited from [NodePathBuilderBase](#nodepathbuilderbase) and used in [HeaderFooterNodePathBuilder](#headerfooternodepathbuilder), [SectionBodyNodePathBuilder](#sectionbodynodepathbuilder), [SectionNodePathBuilder](#sectionnodepathbuilder), [TableCellNodePathBuilder](#tablecellnodepathbuilder).

An object of the **ParagraphNodePathBuilder** class is created by the following constructor methods:

- ParagraphNodePathBuilder([NodePathBuilderBase](#nodepathbuilderbase) ***parentBuilder***, <span style="color:SteelBlue;">int</span> ***index***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***parentBuilder***  | [NodePathBuilderBase](#nodepathbuilderbase)   | parent node path builder. |
| ***index***          | <span style="color:SteelBlue;">int</span>     | element node index. |


### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.


## SectionBodyNodePathBuilder

Represents a node path builder for section body.

An object of the **SectionBodyNodePathBuilder** class is created by the following constructor methods:

- SectionBodyNodePathBuilder([NodePathBuilderBase](#nodepathbuilderbase) ***parentBuilder***,  ***index***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***parentBuilder***  | [NodePathBuilderBase](#nodepathbuilderbase)   | parent node path builder. |
| ***index***          |                                               | element node index. |


### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.
- [ListNodePathBuilder](#listnodepathbuilder) **Lists**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for list nodes.
- [ParagraphNodePathBuilder](#paragraphnodepathbuilder) **Paragraphs**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for paragraph node collection.
- [TableNodePathBuilder](#tablenodepathbuilder) **Tables**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for table nodes.


## SectionNodePathBuilder

Represents a node path builder for fottnotes.

An object of the **SectionNodePathBuilder** class is created by the following constructor methods:

- SectionNodePathBuilder([NodePathBuilderBase](#nodepathbuilderbase) ***parentBuilder***, <span style="color:SteelBlue;">int</span> ***index***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***parentBuilder***  | [NodePathBuilderBase](#nodepathbuilderbase)   | parent node path builder. |
| ***index***          | <span style="color:SteelBlue;">int</span>     | element node index. |


### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.
- [HeaderFooterNodePathBuilder](#headerfooternodepathbuilder) **HeaderFooters**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for header / footer node collection.
- [ListNodePathBuilder](#listnodepathbuilder) **Lists**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for list nodes.
- [ParagraphNodePathBuilder](#paragraphnodepathbuilder) **Paragraphs**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for paragraph node collection.
- [TableNodePathBuilder](#tablenodepathbuilder) **Tables**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for table nodes.


## SimpleNodePathBuilder

Represents a class for simple node.

This class is inherited from [NodePathBuilderBase](#nodepathbuilderbase) and used in [ListNodePathBuilder](#listnodepathbuilder).

An object of the **SimpleNodePathBuilder** class is created by the following constructor methods:

- SimpleNodePathBuilder([NodePathBuilderBase](#nodepathbuilderbase) ***parentBuilder***, <span style="color:SteelBlue;">string</span> ***name***, <span style="color:SteelBlue;">int?</span> *index*)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***parentBuilder***  | [NodePathBuilderBase](#nodepathbuilderbase)   | parent node path builder. |
| ***name***           | <span style="color:SteelBlue;">string</span>  | name of node collection. |
| *index*              | <span style="color:SteelBlue;">int?</span>    | element node index. |


### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.


## TableCellNodePathBuilder

Represents a node path builder for table row cells.

This class is inherited from [NodePathBuilderBase](#nodepathbuilderbase) and used in [TableRowNodePathBuilder](#tablerownodepathbuilder).

An object of the **TableCellNodePathBuilder** class is created by the following constructor methods:

- TableCellNodePathBuilder([NodePathBuilderBase](#nodepathbuilderbase) ***parentBuilder***, <span style="color:SteelBlue;">int</span> ***index***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***parentBuilder***  | [NodePathBuilderBase](#nodepathbuilderbase)   | parent node path builder. |
| ***index***          | <span style="color:SteelBlue;">int</span>     | cell index. |


### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.
- [ParagraphNodePathBuilder](#paragraphnodepathbuilder) **Paragraphs**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for paragraph node collection.
- [TableNodePathBuilder](#tablenodepathbuilder) **Tables**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for table node.


## TableNodePathBuilder

Represents a node path builder for tables.

This class is inherited from [NodePathBuilderBase](#nodepathbuilderbase) and used in [SectionBodyNodePathBuilder](#sectionbodynodepathbuilder), [SectionNodePathBuilder](#sectionnodepathbuilder), [TableCellNodePathBuilder](#tablecellnodepathbuilder).

An object of the **TableNodePathBuilder** class is created by the following constructor methods:

- TableNodePathBuilder([NodePathBuilderBase](#nodepathbuilderbase) ***parentBuilder***, <span style="color:SteelBlue;">int</span> ***index***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***parentBuilder***  | [NodePathBuilderBase](#nodepathbuilderbase)   | parent node path builder. |
| ***index***          | <span style="color:SteelBlue;">int</span>     | element node index. |


### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.
- [TableRowNodePathBuilder](#tablerownodepathbuilder) **Rows**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for row node.


## TableRowNodePathBuilder

Represents a node path builder for table rows.

This class is inherited from [NodePathBuilderBase](#nodepathbuilderbase) and used in [TableNodePathBuilder](#tablenodepathbuilder).

An object of the **TableRowNodePathBuilder** class is created by the following constructor methods:

- TableRowNodePathBuilder([NodePathBuilderBase](#nodepathbuilderbase) ***parentBuilder***, <span style="color:SteelBlue;">int</span> ***index***)

, where:

| Argument             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| ***parentBuilder***  | [NodePathBuilderBase](#nodepathbuilderbase)   | parent node path builder. |
| ***index***          | <span style="color:SteelBlue;">int</span>     | element node index. |


### Methods

- <span style="color:SteelBlue;">string</span> **Build**() - build node path for given node.
- [TableCellNodePathBuilder](#tablecellnodepathbuilder) **Cells**(<span style="color:SteelBlue;">int</span> *index*) - gets a node path builder for cell nodes.

