---
title: "Get Footnotes from Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /footnotes/get-all/
aliases: [/get-footnotes-from-document/]
description: "Get footnotes from a Word document"
weight: 30
---

This REST API retrieves a collection of `Footnote` items.

## REST API

The following URIs are used to address REST resources:

```HTML
~/{file-name}/footnotes
~/{file-name}/{nodePath}/footnotes
```
, where:

- *{file-name}* is a filename of a document.
- *{nodePath}* is a path to a node in a document. If this parameter is used, elements contained within a specified node will be processed:
  - *sections/{sectionIndex}* - references a section.
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|FootnoteType|FootnoteType|Returns a value that specifies whether this is a footnote or endnote.|
|ReferenceMark|string|Specifies custom reference mark to be used for this footnote. The default value is System.String.Empty, meaning auto-numbered footnotes are used.|
|Text|string|This is a convenience property that allows to easily get or set the text of the footnote.|
|Position|DocumentPosition|Reference to marked run of text.|
|Content| |Content of footnote.|

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Footnotes/GetFootnotes) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL. Feel free to download and explore sample input [Footnote.doc](/words/footnotes/Footnote.doc) file designed to act as a demonstration and let you figure out the details quickly.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get footnotes from document
curl -v "https://api.aspose.cloud/v4.0/words/Footnote.doc/footnotes" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```
<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "Footnotes": {
    "List": [
      {
        "Position": {
          "Node": {
            "Text": " ",
            "NodeId": "0.0.1",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/0/runs/1",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          }
        },
        "FootnoteType": "Footnote",
        "ReferenceMark": null,
        "Text": " Footnote 1.\r\n",
        "Content": {
          "ChildNodes": [
            {
              "Text": " Footnote 1.",
              "NodeId": "0.0.2.0",
              "link": {
                "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/0/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "NodeId": "0.0.2",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/0/footnotes/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
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
        "Text": " Endnote 1.\r\n",
        "Content": {
          "ChildNodes": [
            {
              "Text": " Endnote 1.",
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
      {
        "Position": {
          "Node": {
            "Text": "This line also has a footnote.",
            "NodeId": "0.3.0",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/3/runs/0",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          }
        },
        "FootnoteType": "Footnote",
        "ReferenceMark": null,
        "Text": " Footnote 2.\r\n",
        "Content": {
          "ChildNodes": [
            {
              "Text": " Footnote 2.",
              "NodeId": "0.3.1.0",
              "link": {
                "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/3/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "NodeId": "0.3.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/3/footnotes/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Position": {
          "Node": {
            "Text": "This line also has an endnote.",
            "NodeId": "0.4.0",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/4/runs/0",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          }
        },
        "FootnoteType": "Endnote",
        "ReferenceMark": null,
        "Text": " Endnote 2.\r\n",
        "Content": {
          "ChildNodes": [
            {
              "Text": " Endnote 2.",
              "NodeId": "0.4.1.0",
              "link": {
                "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/4/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "NodeId": "0.4.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/4/footnotes/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Position": {
          "Node": {
            "Text": "Third",
            "NodeId": "0.6.0",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/6/runs/0",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          }
        },
        "FootnoteType": "Footnote",
        "ReferenceMark": null,
        "Text": " Footnote 3\r\n",
        "Content": {
          "ChildNodes": [
            {
              "Text": " Footnote 3",
              "NodeId": "0.6.1.0",
              "link": {
                "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/6/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "NodeId": "0.6.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/6/footnotes/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Position": null,
        "FootnoteType": "Footnote",
        "ReferenceMark": null,
        "Text": " fdsfsd\r\n",
        "Content": {
          "ChildNodes": [
            {
              "Text": " fdsfsd",
              "NodeId": "0.7.0.0",
              "link": {
                "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "NodeId": "0.7.0",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Position": {
          "Node": {
            "NodeId": "0.7.0",
            "link": {
              "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/0",
              "Rel": "self",
              "Type": null,
              "Title": null
            }
          }
        },
        "FootnoteType": "Endnote",
        "ReferenceMark": null,
        "Text": " footnote text\r\n",
        "Content": {
          "ChildNodes": [
            {
              "Text": " footnote text",
              "NodeId": "0.7.1.0",
              "link": {
                "Href": "https://api.aspose.cloud/v1.1/words/Footnote.doc/sections/0/paragraphs/7/footnotes/1/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "NodeId": "0.7.1",
        "link": {
          "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/1",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/Footnote.doc/footnotes",
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
{{< tabs tabTotal="10" tabID="5" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetFootnotesOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetFootnotesOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetFootnotesOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetFootnotesOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetFootnotesOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetFootnotesOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetFootnotesOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetFootnotesOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetFootnotesOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetFootnotesOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
