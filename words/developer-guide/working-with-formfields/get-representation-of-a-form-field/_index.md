---
title: "Get Representation of a Form Field"
type: docs
url: /get-representation-of-a-form-field/
aliases: [/get-representation-of-a-form-field/]
weight: 20
---

This REST API allows you to get one of the form fields contained in the paragraph.

## Resource URI

```html

~/{paragraph}/formfields/{formFieldIndex}
```

[Swagger UI](https://apireference.aspose.cloud/words/#/FormFields/GetFormField) lets you call this REST API directly from the browser.  

## cURL Example

**Input Document:** [FormFilled.docx](attachments/885421/1180128.docx)

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

// cURL example to get one of the form field

curl -v "https://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/formfields/0" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}
```java
{
  "FormField": {
    "NodeId": "0.1.0.0.0.1",
    "Name": "FullName",
    "Enabled": true,
    "StatusText": "",
    "OwnStatus": false,
    "HelpText": "",
    "OwnHelp": false,
    "CalculateOnExit": true,
    "EntryMacro": "",
    "ExitMacro": "",
    "TextInputFormat": "UPPERCASE",
    "TextInputType": "Regular",
    "TextInputDefault": "123",
    "MaxLength": 0,
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/FormFilled.docx/sections/0/tables/0/rows/0/cells/0/paragraphs/0/formfields/0",
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
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "GetFormField.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "GetFormField.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "get_form_field.py" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "get_form_field.rb" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "getFormField.js" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_GetFormField.java" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetFormField.swift" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "GetFormField.go" >}}
{{< /tab >}}
{{< /tabs >}}
