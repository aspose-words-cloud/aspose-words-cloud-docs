---
title: "Convert Document to TIFF with Detailed Settings"
type: docs
url: /convert-document-to-tiff-with-detailed-settings/
aliases: [/convert-document-to-tiff-with-detailed-settings/]
keywords: "tiff file, microsoft word document,convert to, word to doc, save word file as pdf,convert word document to html,tiff file,Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift"
description: "API lets you convert MS Word document to the TIFF file with additional settings and save the result to storage. The API SDKs are available in Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift. The resulting image save to the same folder and storage where the original document is. A relative path can be used here for some sub-folder of the document folder."
weight: 30
---

[PUT /words/{name}/saveAs/tiff](https://apireference.aspose.cloud/words/#/Convert/SaveAsTiff) API lets you convert MS Word document to *TIFF file* with additional settings and save the result to storage. The resulting image save to the same folder and storage where the original document is. A relative path can be used here for some sub-folder of the document folder.

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Convert/SaveAsTiff) lets you call this REST API directly from the browser. The description of the API and its parameters is also given there.

## cURL Example

**Input Document:** [test_multi_pages.docx](attachments/885301/1180092.docx) 

**Output Document:** [abc.tiff](attachments/885301/1180091.tiff)** 

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to convert MS Word Document to TIFF
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/saveAs/tiff" \
-X PUT \
-d "{'SaveFormat':'tiff', 'FileName': 'abc.tiff'}" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
{
  "SaveResult": {
    "SourceDocument": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx",
      "Rel": "self",
      "Type": null,
      "Title": null

    },
    "DestDocument": {
      "Href": "abc.tiff",
      "Rel": "saved",
      "Type": null,
      "Title": null

    },
    "AdditionalItems": [
    ]

  },
  "Code": 200,
  "Status": "OK"

} 
```

{{< /tab >}}
{{< /tabs >}}
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples.

## SDK Examples

Code examples for various SDKs are presented below:
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "ConvertWordDocumentToTiffWithDetailedSettings.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "ConvertWordDocumentToTiffWithDetailedSettings.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "ConvertWordDocumentToTiffWithDetailedSettings.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "ConvertWordDocumentToTiffWithDetailedSettings.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "ConvertWordDocumentToTiffWithDetailedSettings.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "ConvertWordDocumentToTiffWithDetailedSettings.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_ConvertWordDocumentToTiffWithDetailedSettings.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_ConvertWordDocumentToTiffWithDetailedSettings.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "ConvertWordDocumentToTiffWithDetailedSettings.go" >}}
{{< /tab >}}
{{< /tabs >}}
