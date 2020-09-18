---
title: "Search Text in a Word Document"
type: docs
url: /search-text-in-a-word-document/
aliases: [/search-text-in-a-word-document/]
weight: 10
---

## **Introduction**
This REST API allows you to search text in a word document. In other words, the API finds all occurrences of a character pattern specified by a regular expression. The request parameters are the following:

|**Parameter Name**|**Type**|**Query String/HTTPBody**|**Description**|
| :- | :- | :- | :- |
|pattern|string|Query String: pattern="pattern"|The regular expression used to find matches.|
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Search/Search) lets you call this REST API directly from the browser.  
## **cURL Example**
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/oauth2/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to find all occurences of a character pattern specified by a regular expression

curl -v "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/search?pattern=aspose" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "SearchingPattern": "aspose",

  "SearchResults": {

    "ResultsList": [

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/products/words/cloud",

            "NodeId": "0.0.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/0/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/products/words/cloud",

            "NodeId": "0.0.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/0/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/products/words/cloud",

            "NodeId": "0.1.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/1/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/products/words/cloud",

            "NodeId": "0.1.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/1/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/products/words/cloud",

            "NodeId": "0.2.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/2/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/products/words/cloud",

            "NodeId": "0.2.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/2/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/products/words/cloud",

            "NodeId": "0.3.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/3/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/products/words/cloud",

            "NodeId": "0.3.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/3/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.4.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/4/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.4.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/4/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.5.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/5/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.5.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/5/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.6.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/6/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.6.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/6/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.7.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/7/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.7.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/7/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.8.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/8/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.8.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/8/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.9.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/9/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.9.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/9/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.10.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/10/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.10.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/10/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.11.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/11/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.11.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/11/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.12.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/12/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.12.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/12/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.13.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/13/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.13.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/13/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.14.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/14/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.14.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/14/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.15.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/15/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.15.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/15/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.16.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/16/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.16.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/16/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.17.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/17/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.17.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/17/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.18.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/18/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.18.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/18/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.19.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/19/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.19.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/19/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Nod\* Connection #0 to host api.aspose.cloud left intact e": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.20.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/20/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.20.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/20/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.21.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/21/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 65

        },

        "RangeEnd": {

          "Node": {

            "Text": "Created in the cloud1234 with Aspose.Words for Cloud. http://www.aspose.com/cloud/word-api.aspx",

            "NodeId": "0.21.0",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/21/runs/0",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 71

        }

      },

      {

        "RangeStart": {

          "Node": {

            "Text": " HYPERLINK \"http://www.aspose.com\" ",

            "NodeId": "5.5.2",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/5/paragraphs/5/runs/1",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 23

        },

        "RangeEnd": {

          "Node": {

            "Text": " HYPERLINK \"http://www.aspose.com\" ",

            "NodeId": "5.5.2",

            "link": {

              "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/5/paragraphs/5/runs/1",

              "Rel": "self",

              "Type": null,

              "Title": null

            }

          },

          "Offset": 29

        }

      }

    ],

    "link": {

      "Href": "http://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/search?pattern=aspose",

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
## **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "SearchText.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "SearchText.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "search_text.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "search_text.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "search_text.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_SearchText.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_SearchText.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "SearchText.go" >}}

{{< /tab >}}

{{< /tabs >}}
