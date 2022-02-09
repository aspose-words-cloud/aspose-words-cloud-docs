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

Request parameters are the following:

|Parameter Name|Type|Query String/HTTPBody|Description|
| :- | :- | :- | :- |
|pattern|string|Query String: pattern="pattern"|The regular expression used to find matches.|

## REST API calls using cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="1" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "SearchOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "SearchOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/0/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/0/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/1/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/1/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/2/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/2/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/3/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/3/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/4/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/4/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/5/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/5/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/6/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/6/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/7/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/7/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/8/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/8/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/9/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/9/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/10/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/10/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/11/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/11/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/12/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/12/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/13/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/13/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/14/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/14/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/15/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/15/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/16/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/16/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/17/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/17/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/18/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/18/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/19/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/19/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/20/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/20/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/21/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/0/paragraphs/21/runs/0",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/5/paragraphs/5/runs/1",
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
              "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/sections/5/paragraphs/5/runs/1",
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
      "Href": "https://api.aspose.cloud/v4.0/words/SampleWordDocument.docx/search?pattern=aspose",
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

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Code samples in Python, Java, C#, etc.

The following code samples show how to interact with REST API using almost any mainstream programming language (The following code samples show how to interact with REST API using almost any mainstream programming language (Python, Java, C#, JavaScript, PHP, C++, Golang, Ruby, Swift, Dart):

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "SearchOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "SearchOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "SearchOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "SearchOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "SearchOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "SearchOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "SearchOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "SearchOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "SearchOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "SearchOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
