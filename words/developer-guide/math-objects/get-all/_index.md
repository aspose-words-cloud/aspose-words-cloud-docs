---
title: "Get OfficeMath Objects from Document"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /math-objects/get-all/
aliases: [/get-officemath-objects-from-document/]
description: "Get all officemath objects from a Word document"
weight: 20
---

This REST API retrieves all `OfficeMath` objects from a document.

## REST API

```JAVA
~/{file-name}/officeMathObjects

~/{file-name}/{nodePath}/officeMathObjects
```
, where:

- *{file-name}* is a filename of a document.
- *{nodePath}* is a path to a node in a document. If this parameter is used, elements contained within a specified node will be processed:
  - *sections/{sectionIndex}* - references a section.
  - *paragraphs/{paragraphIndex}* - references a paragraph.
  - *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references a paragraph within a section.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/OfficeMathObjects/GetOfficeMathObjects) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="2" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get all officeMath objects from the document
curl -v "https://api.aspose.cloud/v4.0/words/MathObjects.docx/OfficeMathObjects" \
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
  "OfficeMathObjects": {
    "List": [
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.0.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/0/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.0.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/0/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.1.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/1/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.1.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/1/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.2.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/2/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.2.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/2/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.3.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/3/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.3.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/3/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.4.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/4/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.4.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/4/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.5.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/5/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.5.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/5/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.6.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/6/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.6.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/6/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.7.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/7/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.7.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/7/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.8.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/8/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup"\*Connection#0tohostapi.aspose.cloudleftintact,
        "MathObjectType": "OMathPara",
        "NodeId": "0.8.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/8/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.9.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/9/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.9.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/9/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.10.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/10/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.10.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/10/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.11.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/11/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.11.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/11/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.12.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/12/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.12.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/12/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.13.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/13/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.13.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/13/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.14.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/14/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.14.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/14/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      },
      {
        "Content": {
          "ChildNodes": [
            {
              "NodeId": "0.15.0.0",
              "link": {
                "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/15/OfficeMathObjects/0/OfficeMathObjects/0",
                "Rel": "self",
                "Type": null,
                "Title": null
              }
            }
          ]
        },
        "DisplayType": "Display",
        "Justification": "CenterGroup",
        "MathObjectType": "OMathPara",
        "NodeId": "0.15.0",
        "link": {
          "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/15/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/MathObjects.docx/OfficeMathObjects",
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
{{< tabs tabTotal="5" tabID="5" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetOfficeMathObjects.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetOfficeMathObjects.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetOfficeMathObjects.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Aspose_Cloud_Words_GetOfficeMathObjects.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Aspose_Words_Swift_GetOfficeMathObjects.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
