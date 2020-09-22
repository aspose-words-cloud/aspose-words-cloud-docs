---
title: "Replace Document Text"
type: docs
url: /replace-document-text/
aliases: [/replace-document-text/]
weight: 20
---

This REST API allows you to replace text in a document. The API replaces all occurrences of a specified string with another string. If a captured or replacement string contains one or more special characters: paragraph break, cell break, section break, field start, field separator, field end, inline picture, drawing object, footnote, the API returns HTTP 400 error response.

The request parameters are the following:

|Parameter Name|Type|Description|
| :- | :- | :- |
|OldValue|string|Old text value (or regex pattern (see "IsOldValueRegex")) to replace.|
|NewValue|string|New text value to replace by.|
|IsMatchCase|bool|Flag, true means the search is case-sensitive; false means the search is not case-sensitive. Not used if "IsOldValueRegex" is set.|
|IsMatchWholeWord|bool|The flag means that only whole word matched are replaced. Not used if "IsOldValueRegex" is set.|
|IsOldValueRegex|bool|The flag means that "OldValue" contains regex expression.|
Moreover, resource properties are the following:

|Property Name|Type|Description|
| :- | :- | :- |
|Matches|integer|Returns the number of matches.|

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/ReplaceText/ReplaceText) lets you call this REST API directly from the browser.  

## cURL Example

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```java

// Please get your App_Key and App_SID from https://dashboard.aspose.cloud/#/apps. Place your App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to replace document text

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/replaceText" \
-X PUT \
-d "{ 'OldValue': 'aspose', 'NewValue': 'aspose new', 'IsMatchCase': true, 'IsMatchWholeWord': false }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}
{{< tab tabNum="2" >}}

```java

{

  "Matches": 0,
  "DocumentLink": {

    "Href": "test_multi_pages.docx",
    "Rel": "self",
    "Type": null,
    "Title": null

  },
  "Code": 200,
  "Status": "OK"

}

```

{{< /tab >}}
{{< /tabs >}}

## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "ReplaceDocumentText.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "PostReplaceText.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "post_replace_text.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "post_replace_text.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "postReplaceText.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_PostReplaceText.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_PostReplaceText.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "ReplaceText.go" >}}
{{< /tab >}}
{{< /tabs >}}
