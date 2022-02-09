---
title: "Update Footnote Properties"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /footnotes/update/
aliases: [/update-footnote-properties/]
description: "Update footnote properties in a Word document"
weight: 50
---

This REST API updates `Footnote` properties.

## REST API

The following URIs are used to address REST resources:

```HTML
~/{file-name}/footnotes/{index}
~/{file-name}/{nodePath}/footnotes/{index}
```
, where:

- *{file-name}* is a filename of a document.
- *{nodePath}* is a path to a node in a document. If this parameter is used, elements contained within a specified node will be processed:
- *sections/{sectionIndex}* - references a section.
- *paragraphs/{paragraphIndex}* - references a paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.
- *{index}* is an index of a footnote.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|FootnoteType|FootnoteType|Returns a value that specifies whether this is a footnote or endnote.|
|ReferenceMark|string|Gets/sets custom reference mark to be used for this footnote. Default value is System.String.Empty, meaning auto-numbered footnotes are used.|
|Text|string|This is a convenience property that allows to easily get or set the text of the footnote.|
|Position|DocumentPosition|Reference to marked run of text.|
|Content| |Content of footnote.|

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Footnotes/UpdateFootnote) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [Footnote.doc](/words/footnotes/Footnote.doc) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="2" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
	{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "UpdateFootnoteOnline.curl" >}}
	<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< tab tabNum="2" >}}
	{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "UpdateFootnoteOnline.json" >}}
	<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>
{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "Footnote": {
    "Position": {
      "Node": {
        "Text": " ",
        "NodeId": "0.1.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/1/runs/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    },
    "FootnoteType": "Endnote",
    "ReferenceMark": null,
    "Text": " new text\r\n",
    "Content": {
      "ChildNodes": [
        {
          "Text": " new text",
          "NodeId": "0.1.2.0",
          "link": {
            "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/1/footnotes/0/paragraphs/0",
            "Rel": "self",
            "Type": null,
            "Title": null
          }
        }
      ]
    },
    "NodeId": "0.1.2",
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/1/footnotes/0",
      "Rel": "self",
      "Type": null,
      "Title": null
    }
  },
  "Code": 200,
  "Status": "OK"
}
```
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="11" tabID="5" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" tabName11="Curl" >}}
{{< tab tabNum="1" >}}
	{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "UpdateFootnoteOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
	{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "UpdateFootnoteOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
	{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "UpdateFootnoteOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
	{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "UpdateFootnoteOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
	{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "UpdateFootnoteOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
	{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "UpdateFootnoteOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
	{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
	{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "UpdateFootnoteOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
	{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "UpdateFootnoteOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
	{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "UpdateFootnoteOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
	{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "UpdateFootnoteOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
