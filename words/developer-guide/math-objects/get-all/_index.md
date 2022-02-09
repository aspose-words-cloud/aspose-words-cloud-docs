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

You can use **cURL** and **Postman** to access Aspose.Words Cloud API. The following examples demonstate how to do it. Please refer to the <a href="/words/getting-started/quickstart/">instructions</a> to get a 'JWT_TOKEN' for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="2" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetOfficeMathObjectsOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetOfficeMathObjectsOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/0/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/0/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/1/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/1/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/2/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/2/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/3/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/3/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/4/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/4/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/5/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/5/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/6/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/6/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/7/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/7/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/8/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/8/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/9/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/9/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/10/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/10/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/11/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/11/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/12/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/12/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/13/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/13/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/14/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/14/OfficeMathObjects/0",
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
                "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/15/OfficeMathObjects/0/OfficeMathObjects/0",
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
          "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/sections/0/paragraphs/15/OfficeMathObjects/0",
          "Rel": "self",
          "Type": null,
          "Title": null
        }
      }
    ],
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/MathObjects.docx/OfficeMathObjects",
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
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetOfficeMathObjectsOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetOfficeMathObjectsOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetOfficeMathObjectsOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetOfficeMathObjectsOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetOfficeMathObjectsOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetOfficeMathObjectsOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetOfficeMathObjectsOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetOfficeMathObjectsOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetOfficeMathObjectsOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetOfficeMathObjectsOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
