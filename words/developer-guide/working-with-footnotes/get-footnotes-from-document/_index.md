---
title: "Get Footnotes from Document"
type: docs
url: /get-footnotes-from-document/
aliases: [/get-footnotes-from-document/]
weight: 10
---

This REST API allows you to get a list of footnotes that are contained in the document.

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
[Swagger UI](https://apireference.aspose.cloud/words/#/Footnotes/GetFootnotes) lets you call this REST API directly from the browser.  

## cURL Example

**Input Document:** [Footnote.doc](attachments/885418/1180127.doc)

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

// cURL example to get footnotes from document

curl -v "https://api.aspose.cloud/v4.0/words/Footnote.doc/footnotes" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java

{
  "Footnotes": {
    "List": [
      {
        "Position": {
          "Node": {
            "Text": " ",
            "NodeId": "0.0.1",
            "link": {
              "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/0/runs/1",
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
                "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/0/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null

              }
            }
          ]

        },
        "NodeId": "0.0.2",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/0/footnotes/0",
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
              "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/1/runs/1",
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
                "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/1/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null

              }
            }
          ]

        },
        "NodeId": "0.1.2",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/1/footnotes/0",
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
              "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/3/runs/0",
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
                "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/3/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null

              }
            }
          ]

        },
        "NodeId": "0.3.1",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/3/footnotes/0",
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
              "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/4/runs/0",
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
                "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/4/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null

              }
            }
          ]

        },
        "NodeId": "0.4.1",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/4/footnotes/0",
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
              "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/6/runs/0",
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
                "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/6/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null

              }
            }
          ]

        },
        "NodeId": "0.6.1",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/6/footnotes/0",
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
                "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/0/paragraphs/0",
                "Rel": "self",
                "Type": null,
                "Title": null

              }
            }
          ]

        },
        "NodeId": "0.7.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/0",
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
              "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/sections/0/paragraphs/7/footnotes/0",
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
                "Href": "http://api.aspose.cl\* Connection #0 to host api.aspose.cloud left intact oud/v1.1/words/Footnote.doc/sections/0/paragraphs/7/footnotes/1/paragraphs/0",
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
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/Footnote.doc/footnotes",
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
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="9" tabID="5" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetFootnotes.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetFootnotes.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "GetFootnotes.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "GetFootnotes.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "GetFootnotes.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "GetFootnotes.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetFootnotes.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetFootnotes.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetFootnotes.go" >}}
{{< /tab >}}
{{< /tabs >}}
