---
title: "Aspose.Words for Cloud 17.5 Release Notes"
type: docs
url: /aspose-words-for-cloud-17-5-release-notes/
aliases: [/aspose-words-for-cloud-17-5-release-notes/]
weight: 80
---

{{% alert color="primary" %}} 

The page contains release notes for Aspose.Words for Cloud update 17.5 – [API Version 1.1](http://api.aspose.com/v1.1/swagger/ui/index)

{{% /alert %}} 
#### Swagger Notation Optimization
Swagger notation was reworked to merge similar methods into one, making overall method list more consise. Specifically, the following variables are introduced into methods' paths (note that they are optional in some methods):

- *\{nodePath\}* - specifies path to a node (section or paragraph). Sample syntaxes:
  - *sections/\{sectionIndex\}* - references specific section
  - *paragraphs/\{paragraphIndex\}* - references specific paragraph
  - *sections/\{sectionIndex\}/paragraphs/\{paragraphIndex\}* - references specific paragraph within section.
- *\{paragraphPath\}* - specifies path to a paragraph. Sample syntaxes:
  - *paragraphs/\{paragraphIndex\}* - references specific paragraph
  - *sections/\{sectionIndex\}/paragraphs/\{paragraphIndex\}* - references specific paragraph within section
- *\{sectionPath\}* - specifies path to a section. Sample syntax:
  - *sections/\{sectionIndex\}* - references specific section
- *\{tablePath\}* - specifies path to a table. Sample syntax:
  - *\{nodePath\}/tables/\{tableIndex\}* - references specific table in paragraph or section

Note that certain elements can be nested in cells or headersFooters, e.g. paragraph could be referenced by */sections/1/tables/1/rows/1/cells/1/paragraph/1*.
#### Detail Issues with Associated IDs

|**Key**|**Summary**|**Category**|
| :- | :- | :- |
|WORDSCLOUD-163|<p>Render complex document parts</p><p>The following elements support rendering as of 17.5</p><p>- page</p><p>- paragraph</p><p>- table</p><p>- drawingObject</p><p>- officeMathObject</p><p>The following formats are supported:</p><p>- bmp</p><p>- gif</p><p>- jpeg</p><p>- png</p><p>- svg</p><p>- tiff</p><p> </p>|Feature|
|WORDSCLOUD-173|If storage does not exist, server returns "Object reference not set to an instance of an object|Bug|
|WORDSCLOUD-178|Sequence contains no matching element" Exception in GetComments method|Bug|
|WORDSCLOUD-181|Unable to Add Text to a Header in a Word Document|Bug|
|WORDSCLOUD-182 |<p>Create DELETE /v/words/{name}/{nodePath}/fields/{index} method</p><p>Deletes specific field from node (section or paragraph)</p>|Feature|
|WORDSCLOUD-183 |<p>Create GET /v/words/{name}/{nodePath}/fields method</p><p>Returns all fields for the given nodepath</p>|Feature|
|WORDSCLOUD-184|<p>Create GET /v/words/{name}/{paragraphPath}/runs</p><p>Returns all runs in specified paragraph</p>|Feature|

