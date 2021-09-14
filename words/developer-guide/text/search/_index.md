---
title: "Search"
second_title: "Text in a Word Document"
type: docs
url: /text/search/
aliases: [/search-text-in-a-word-document/]
description: "Search text in a Word document"
weight: 20
---

This REST API searches text in a document. It finds all occurrences of a character pattern specified by a **Regular Expression**.

The request parameters are the following:

|Parameter Name|Type|Query String/HTTPBody|Description|
| :- | :- | :- | :- |
|pattern|string|Query String: pattern="pattern"|The regular expression used to find matches.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Search/Search) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to find all occurences of a character pattern specified by a regular expression
curl -v "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/search?pattern=aspose" \
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
{{< /nosnippet >}}

## Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs.

The following code examples demonstrate how to make calls to Aspose.Words web services using various SDKs:

{{< nosnippet >}}
{{< tabs tabTotal="5" tabID="4" tabName1="Java" tabName2="C#" tabName3="Golang" tabName4="Android" tabName5="Swift" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "Search.java" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "Search.cs" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "Search.go" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "fde11f9e52383a88af20b937c5e9b3d9" "Search.java" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "Search.swift" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
