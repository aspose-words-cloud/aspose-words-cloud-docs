---
title: "Working with Range"
type: docs
url: /working-with-range/
aliases: [/working-with-range/]
weight: 210
---

## Overview
The concept of Range is similar to [Range Object in MS Word API](https://docs.microsoft.com/en-us/office/vba/word/Concepts/Working-with-Word/working-with-range-objects). Working with a range is much closer to how a user interacts with a document in MS Word.

A range is basically a contiguous area in a document. It is signified as a pair of positions (START, END), where a coordinate of START always less than a coordinate of END. It may span across multiple sections, paragraphs, etc., in other words, across different nodes of the [DOM tree](https://docs.aspose.com/display/wordsnet/Aspose.Words+Document+Object+Model). Thus, a user can ignore the underlying model of the document. Such an approach is going to make the usage of API much more friendly.
## Ways to Specify a Range
A range can be specified in one of the three ways:
### Position in a document based on nodes IDs
/range/{startId}/{endId}

- {startId} - id of the node from which the range starts (included). Required.
- {endId} - id of the node at which the range ends (excluded). Optional. If missed, the end of the range corresponds to the end of the node with id = startId, i.e. the range is limited by the bounds of "startId node".
#### Example
A range consisting of the second and third paragraphs.

/range/id0.1/id0.3
### Position in a document based on nodes pseudo names
/range/{startPseudoName}/{endPseudoName}

- {startPseudoName} - a pseudo name of the node from which the range starts (included). Required.
- {endPseudoName} - a pseudo name of the node at which the range ends (excluded). Optional. If missed, the end of the range corresponds to the end of the node with pseudoname = startPseudoName, i.e. the range is limited by the bounds of "startPseudoName node".

**Available pseudonames**

- TableN for tables.
- ImageN for images.
#### Example
A range consisting of the text from the first table and after the table till the second table.

/range/table0/table1
### Positions inside nodes
A certain position inside a node can be specified with a selector that is separated from a node identifier with a colon.

/range/{startIdentifier}:{startSelector}/{endIdentifier}:{endSelector}

- {startIdentifier} - an identifier (id or a pseudo name) of the node from which the range starts (included). Required.
- {endIdentifier} - an identifier (id or a pseudo name) of the node at which the range ends (excluded). Optional. If missed, the end of the range corresponds to the end of the node with identifier = startIdentifier, i.e. the range is limited by the bounds of "startIdentifier node".
- {startSelector} - a selector that specifies a certain position inside the start node (included). Optional. If missed, the start of the range corresponds to the beginning of the start node.
- {endSelector} - a selector that specifies a certain position inside the end node (excluded). Optional. If missed, the end of the range corresponds to the element before the beginning of the end node.

Selectors cannot be used without a node identifier.

**Available selectors**

end - specifies the end of the node ("end" here is supposed to be a virtual node after the last child node, i.e. it means that the whole content of the node should be included for an end node).
#### Example
A range consisting of all nodes starting from the end of the 1st table till the beginning of the 6th paragraph.

/range/table0:end/id0.5
## Operations with a Range
The following operations can be defined on a range:
### Get the text from the range
Get the text from all nodes in the range. You may use one of the following two APIs to get the text from the range:

- [GET /words/{name}/range/{rangeStartIdentifier}/{rangeEndIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/GetRangeText)
- [GET /words/{name}/range/{rangeStartIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/GetRangeText2)
### Remove the text from the range
With the following APIs you can remove the text from the range. Text from all nodes inside the range would be removed.

- [DELETE /words/{name}/range/{rangeStartIdentifier}/{rangeEndIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/RemoveRange)
- [DELETE /words/{name}/range/{rangeStartIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/RemoveRange2)
### Replace the content in the range
The replacement should be done according to MS Word rules. For example, several nodes, except the case when all nodes are runs of one paragraph, should be replaced with one new paragraph. However, several runs in one paragraph should be replaced with the new run(s). The style should be consistent to removed nodes.

Content in the range can be replaced with one of the following two APIs:

- [POST /words/{name}/range/{rangeStartIdentifier}/{rangeEndIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/ReplaceWithText)
- [POST /words/{name}/range/{rangeStartIdentifier}](https://apireference.aspose.cloud/words/#/RangeApi/ReplaceWithText2)
### Save the selected range as a new document
The range should be saved as a separate document. The original document must not be changed. The said task can be achieved with one of the following two APIs:

- [POST /words/{name}/range/{rangeStartIdentifier}/{rangeEndIdentifier}/SaveAs](https://apireference.aspose.cloud/words/#/RangeApi/SaveAsRange)
- [POST /words/{name}/range/{rangeStartIdentifier}/SaveAs](https://apireference.aspose.cloud/words/#/RangeApi/SaveAsRange2)
## Use cases
**Use case 1: A user wants to get a text from the first two paragraphs in the document.**

First, he needs to call [Paragraph API](https://apireference.aspose.cloud/words/#/Paragraphs/GetParagraphs) to get a list of paragraphs that are contained in the document.

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get a list of paragraphs that are contained in the document or in the section

curl -v "https://api.aspose.cloud/v4.0/words/MyDocument.docx/paragraphs" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Paragraphs": {

    "ParagraphLinkList": [

      {

        "Text": "You might find it useful to extract only the text from a document. This is useful if you are passing the text to another API service. All the text in a document is contained in text runs of paragraph elements. Text can appear in three types of the document's structural elements.",

        "NodeId": "0.0",

        "link": {

          "Href": "https://api.aspose.cloud/v4.0/words/MyDocument.docx/sections/0/paragraphs/0",

          "Rel": "self"

        }

      },

      {

        "Text": "",

        "NodeId": "0.1",

        "link": {

          "Href": "https://api.aspose.cloud/v4.0/words/MyDocument.docx/sections/0/paragraphs/1",

          "Rel": "self"

        }

      },

      {

        "Text": "The resulting dump can help you understand the structure of Google Docs files in general, or help you troubleshoot issues around the structure and content of a particular document.",

        "NodeId": "0.2",

        "link": {

          "Href": "https://api.aspose.cloud/v4.0/words/MyDocument.docx/sections/0/paragraphs/2",

          "Rel": "self"

        }

      }

    ],

    "link": {

      "Href": "https://api.aspose.cloud/v4.0/words/MyDocument.docx/paragraphs",

      "Rel": "self"

    }

  }

}

```

{{< /tab >}}

{{< /tabs >}}

He sees that the first two paragraphs correspond to id0.0 and id0.2 (NodeId in the response), so he calls Range API to get the text he requires:

{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// cURL example to get the text from the range.

curl -v "https://api.aspose.cloud/v4.0/words/MyDocument.docx/range/id0.0/id0.2:end" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Text": "You might find it useful to extract only the text from a document. This is useful if you are passing the text to another API service. All the text in a document is contained in text runs of paragraph elements. Text can appear in three types of the document's structural elements.  The resulting dump can help you understand the structure of Google Docs files in general, or help you troubleshoot issues around the structure and content of a particular document. "

}

```

{{< /tab >}}

{{< /tabs >}}

**Use case 2: A user wants to save the selected range as a new document.**

First, he needs to call [Paragraph API](https://apireference.aspose.cloud/words/#/Paragraphs/GetParagraphs) to get a list of paragraphs that are contained in the document.

{{< tabs tabTotal="2" tabID="7" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client_secret" and App SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to get a list of paragraphs that are contained in the document or in the section

curl -v "https://api.aspose.cloud/v4.0/words/MyDocument.docx/paragraphs" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Paragraphs": {

    "ParagraphLinkList": [

      {

        "Text": "You might find it useful to extract only the text from a document. This is useful if you are passing the text to another API service. All the text in a document is contained in text runs of paragraph elements. Text can appear in three types of the document's structural elements.",

        "NodeId": "0.0",

        "link": {

          "Href": "https://api.aspose.cloud/v4.0/words/MyDocument.docx/sections/0/paragraphs/0",

          "Rel": "self"

        }

      },

      {

        "Text": "",

        "NodeId": "0.1",

        "link": {

          "Href": "https://api.aspose.cloud/v4.0/words/MyDocument.docx/sections/0/paragraphs/1",

          "Rel": "self"

        }

      },

      {

        "Text": "The resulting dump can help you understand the structure of Google Docs files in general, or help you troubleshoot issues around the structure and content of a particular document.",

        "NodeId": "0.2",

        "link": {

          "Href": "https://api.aspose.cloud/v4.0/words/MyDocument.docx/sections/0/paragraphs/2",

          "Rel": "self"

        }

      }

    ],

    "link": {

      "Href": "https://api.aspose.cloud/v4.0/words/MyDocument.docx/paragraphs",

      "Rel": "self"

    }

  }

}

```

{{< /tab >}}

{{< /tabs >}}

Now, he calls the following API to save the first two paragraphs (correspond to id0.0 and id0.2 in the response) as a new document:** 

{{< tabs tabTotal="2" tabID="10" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// cURL example to save the selected range as a new document.

curl -v "https://api.aspose.cloud/v4.0/words/MyDocument.docx/range/id0.0/id0.2:end/saveas" \
-X POST \
-d "{ 'DocumentName': 'SelectedRanage.docx' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Document": {

    "Links": [

      {

        "Href": "SelectedRanage.docx",

        "Rel": "self"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=doc",

        "Rel": "alternate",

        "Type": "application/msword",

        "Title": "Download as DOC"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=dot",

        "Rel": "alternate",

        "Type": "application/msword",

        "Title": "Download as DOT"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=docx",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",

        "Title": "Download as DOCX"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=docm",

        "Rel": "alternate",

        "Type": "application/vnd.ms-word.document.macroEnabled.12",

        "Title": "Download as DOCM"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=dotx",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.template",

        "Title": "Download as DOTX"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=dotm",

        "Rel": "alternate",

        "Type": "application/vnd.ms-word.template.macroEnabled.12",

        "Title": "Download as DOTM"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=flatopc",

        "Rel": "alternate",

        "Type": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",

        "Title": "Download as FLATOPC"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=rtf",

        "Rel": "alternate",

        "Type": "application/rtf",

        "Title": "Download as RTF"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=wml",

        "Rel": "alternate",

        "Type": "text/xml",

        "Title": "Download as WML"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=odt",

        "Rel": "alternate",

        "Type": "application/vnd.oasis.opendocument.text",

        "Title": "Download as ODT"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=ott",

        "Rel": "alternate",

        "Type": "application/vnd.oasis.opendocument.text-template",

        "Title": "Download as OTT"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=txt",

        "Rel": "alternate",

        "Type": "text/plain",

        "Title": "Download as TXT"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=mhtml",

        "Rel": "alternate",

        "Type": "multipart/related",

        "Title": "Download as MHTML"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=epub",

        "Rel": "alternate",

        "Type": "application/epub+zip",

        "Title": "Download as EPUB"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=pdf",

        "Rel": "alternate",

        "Type": "application/pdf",

        "Title": "Download as PDF"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=xps",

        "Rel": "alternate",

        "Type": "application/vnd.ms-xpsdocument",

        "Title": "Download as XPS"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=tiff",

        "Rel": "alternate",

        "Type": "image/tiff",

        "Title": "Download as TIFF"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=png",

        "Rel": "alternate",

        "Type": "image/png",

        "Title": "Download as PNG"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=jpeg",

        "Rel": "alternate",

        "Type": "image/jpeg",

        "Title": "Download as JPEG"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=bmp",

        "Rel": "alternate",

        "Type": "image/bmp",

        "Title": "Download as BMP"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=gif",

        "Rel": "alternate",

        "Type": "image/gif",

        "Title": "Download as GIF"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=svg",

        "Rel": "alternate",

        "Type": "image/svg+xml",

        "Title": "Download as SVG"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=html",

        "Rel": "alternate",

        "Type": "text/html",

        "Title": "Download as HTML"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=htmlfixed",

        "Rel": "alternate",

        "Type": "text/html",

        "Title": "Download as HTMLFIXED"

      },

      {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx?format=pcl",

        "Rel": "alternate",

        "Type": "application/x-pcl",

        "Title": "Download as PCL"

      }

    ],

    "FileName": "SelectedRanage.docx",

    "SourceFormat": "Docx",

    "IsEncrypted": false,

    "IsSigned": false,

    "DocumentProperties": {

      "link": {

        "Href": "https://api.aspose.cloud/v4.0/words/SelectedRanage.docx/documentProperties",

        "Rel": "self"

      }

    }

  }

}

```

{{< /tab >}}

{{< /tabs >}}
## SDKs
Using an SDK is the best way to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## SDK Examples
**Use case 1: Get text from the first two paragraphs in the document.**

{{< tabs tabTotal="4" tabID="13" tabName1="C#" tabName2="Android" tabName3="Swift" tabName4="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetParagraphsText.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetParagraphsText.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetParagraphsText.swift" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetParagraphsText.go" >}}

{{< /tab >}}

{{< /tabs >}}

**Use case 2: Save the selected range as a new document.**

{{< tabs tabTotal="4" tabID="14" tabName1="C#" tabName2="Android" tabName3="Swift" tabName4="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "SaveTheSelectedRanageAsANewDocument.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_SaveTheSelectedRanageAsANewDocument.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_SaveTheSelectedRanageAsANewDocument.swift" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "SaveTheSelectedRanageAsANewDocument.go" >}}

{{< /tab >}}

{{< /tabs >}}

