---
title: "Add Footnote to Document"
type: docs
url: /add-footnote-to-document/
aliases: [/add-footnote-to-document/]
weight: 30
---

This REST API allows you to add a footnote to a document.

## Resource URI

```html

~/{file-name}/footnotes

~/{file-name}/{nodePath}/footnotes
```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to a specific node in the document. If this URI is used, only elements contained within a specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

The resource properties are:

|Property Name|Type|Description|
| :- | :- | :- |
|FootnoteType|FootnoteType|Returns a value that specifies whether this is a footnote or endnote.|
|ReferenceMark|string|Specifies custom reference mark to be used for this footnote. The default value is System.String.Empty, meaning auto-numbered footnotes are used.|
|Text|string|This is a convenience property that allows to easily get or set the text of the footnote.|
|Position|DocumentPosition|Reference to marked run of text.|
|Content| |Content of footnote.|
The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Footnotes/InsertFootnote) lets you call this REST API directly from a browser.

## cURL Example

cUrl is a popular command-line utility for transferring data and a perfect tool for testing REST APIs. The following are a few examples of using cURL.

*Input Document:** [Footnote.doc](attachments/885418/1180127.doc)

{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to add footnote to document
curl -v "https://api.aspose.cloud/v4.0/words/Footnote.doc/footnotes" \
-X POST \
-d "{ 'FootnoteType': 'Endnote', 'Text': 'footnote text' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
{
  "Footnote": {
    "Position": {
      "Node": {
        "NodeId": "0.7.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/0",
          "Rel": "self",
          "Type": null,
          "Title": null

        }
      }
    },
    "FootnoteType": "Endnote",
    "ReferenceMark": "",
    "Text": " footnote text\r\n",
    "Content": {
      "ChildNodes": [
        {
          "Text": " footnote text",
          "NodeId": "0.7.1.0",
          "link": {
            "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/1/paragraphs/0",
            "Rel": "self",
            "Type": null,
            "Title": null

          }
        }
      ]
    },
    "NodeId": "0.7.1",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/1",
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
## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

## SDK Examples

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="9" tabID="5" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "AddFootnoteToDocument.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PutFootnote.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "PutFootnote.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "PutFootnote.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "PutFootnote.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "PutFootnote.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PutFootnote.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PutFootnote.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "PutFootnote.go" >}}
{{< /tab >}}
{{< /tabs >}}
