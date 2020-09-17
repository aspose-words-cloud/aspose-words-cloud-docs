---
title: "Update Border Properties"
type: docs
url: /update-border-properties/
weight: 190
---

## **Introduction**
The REST API allows you to update the properties of the table border. It returns updated border data in XML/JSON format. The details of resource properties are given below:

|**Property Name**|**Type**|**Description**|
| :- | :- | :- |
|BorderType|BorderType|Gets the border type.|
|Color|Color|Specifies the border color.|
|DistanceFromText|double|Specifies distance of the border from text or from the page edge in points.|
|LineStyle|LineStyle|Specifies the border style.|
|LineWidth|LineWidth|Specifies the border width in points.|
|Shadow|bool|Specifies a value indicating whether the border has a shadow.|
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/words/#/Borders/UpdateBorder) lets you call this REST API directly from the browser. The description of the API and its parameters are also given there.
## **cURL Example**
**Input Document:** [TablesGet.docx](attachments/885355/1180119.docx)

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get JSON Web Token

// Please get your App Key and App SID from https://dashboard.aspose.cloud/#/apps. Kindly place App Key in "client\_secret" and App SID in "client\_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to update border properties

curl -v "https://api.aspose.cloud/v4.0/words/TablesGet.docx/tables/1/rows/0/cells/0/borders/left" \
-X PUT \
-d "{ 'Color': { 'Web': 'Lime' }, 'DistanceFromText': '9.66', 'LineStyle': 'DotDash', 'LineWidth': '3', 'Shadow': 'true' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

  "Border": {

    "BorderType": "Left",

    "Color": {

      "Web": "#00FF00"

    },

    "DistanceFromText": 9.0,

    "LineStyle": "DotDash",

    "LineWidth": 3.0,

    "Shadow": true,

    "link": null

  },

  "Code": 200,

  "Status": "OK"

}

```

{{< /tab >}}

{{< /tabs >}}
## **SDK Source**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words Cloud SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
{{< tabs tabTotal="8" tabID="4" tabName1="C#" tabName2="Java" tabName3="Python" tabName4="Ruby" tabName5="Node.js" tabName6="Android" tabName7="Swift" tabName8="Go" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "UpdateTableBorder.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "UpdateBorder.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "303ca1faad43f8d1b672fbeac98ad2e0" "update\_table\_border\_properties.py" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "5af73b7a7c08a9072ac1c05b0914df3f" "update\_border.rb" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "e5e9b0139962cb912eac42c9df06a1a2" "updateBorder.js" >}}

{{< /tab >}}

{{< tab tabNum="6" >}}

{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose\_Cloud\_Words\_UpdateBorder.java" >}}

{{< /tab >}}

{{< tab tabNum="7" >}}

{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose\_Words\_Swift\_UpdateBorder.swift" >}}

{{< /tab >}}

{{< tab tabNum="8" >}}

{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "UpdateBorder.go" >}}

{{< /tab >}}

{{< /tabs >}}
