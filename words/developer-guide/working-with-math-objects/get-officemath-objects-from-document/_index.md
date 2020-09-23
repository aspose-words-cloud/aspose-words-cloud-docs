---
title: "Get OfficeMath Objects from Document"
type: docs
url: /get-officemath-objects-from-document/
aliases: [/get-officemath-objects-from-document/]
weight: 10
---

This REST API allows you to get all OfficeMath objects that are defined in the document.

## Resource URI

```java
~/{file-name}/officeMathObjects

~/{file-name}/{nodePath}/officeMathObjects
```

*{file-name}* is the name of the Word document containing elements.
*{nodePath}* is the path to a specific node in the document. If this URI is used, only elements contained within a specific node will be returned. Supported syntax:

- *sections/{sectionIndex}* - references specific section.
- *paragraphs/{paragraphIndex}* - references specific paragraph.
- *sections/{sectionIndex}/paragraphs/{paragraphIndex}* - references specific paragraph within section.

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/OfficeMathObjects/GetOfficeMathObjects) lets you call this REST API directly from a browser.  

## cURL Example

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

// cURL example to get all officeMath objects from the document
curl -v "https://api.aspose.cloud/v4.0/words/MathObjects.docx/OfficeMathObjects" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
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
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs, supplied with short and clear code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="8" tabID="5" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetOfficeMathObjects.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetOfficeMathObjects.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_office_math_objects.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_office_math_objects.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getOfficeMathObjects.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetOfficeMathObjects.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetOfficeMathObjects.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetOfficeMathObjects.go" >}}
{{< /tab >}}
{{< /tabs >}}
