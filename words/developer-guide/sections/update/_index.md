---
title: "Update the Page Setup of a Section"
type: docs
url: /sections/update/
aliases: [/update-the-page-setup-of-a-section/]
description: "Update page setup properties of a section in a Word document"
weight: 40
---

This REST API updates page setup properties of a section.

The important properties are described below:

|Property Name|Type|Description|
| :- | :- | :- |
|Bidi|bool|Specifies that this section contains bidirectional (complex scripts) text.|
|BorderAlwaysInFront|bool|Specifies where the page border is positioned relative to intersecting texts and objects.|
|BorderAppliesTo|PageBorderAppliesTo|Specifies which pages the page border is printed on.|
|BorderDistanceFrom|PageBorderDistanceFrom|Specifies a value that indicates whether the specified page border is measured from the edge of the page or from the text it surrounds.|
|BottomMargin|double|Specifies the distance (in points) between the bottom edge of the page and the bottom boundary of the body text.|
|DifferentFirstPageHeaderFooter|bool|True if a different header or footer is used on the first page.|
|FirstPageTray|int|Specifies the paper tray (bin) to use for the first page of a section. The value is implementation (printer) specific.|
|FooterDistance|double|Specifies the distance (in points) between the footer and the bottom of the page.|
|Gutter|double|Specifies the amount of extra space added to the margin for document binding.|
|HeaderDistance|double|Specifies the distance (in points) between the header and the top of the page.|
|LeftMargin|double|Specifies the distance (in points) between the left edge of the page and the left boundary of the body text.|
|LineNumberCountBy|int|Specifies the numeric increment for line numbers.|
|LineNumberDistanceFromText|double|Specifies the distance between the right edge of line numbers and the left edge of the document. Set this property to zero for the automatic distance between the line numbers and text of the document.|
|LineNumberRestartMode|LineNumberRestartMode|Specifies the way line numbering runs that is, whether it starts over at the beginning of a new page or section or runs continuously.|
|LineStartingNumber|int|Specifies the starting line number.|
|Orientation|Orientation|Specifies the orientation of the page. Changing 'Orientation' swaps 'PageWidth' and 'PageHeight'.|
|OtherPagesTray|int|Specifies the paper tray (bin) to be used for all but the first page of a section. The value is implementation (printer) specific.|
|PageHeight|double|Specifies the height of the page in points.|
|PageNumberStyle|NumberStyle|Specifies the page number format.|
|PageStartingNumber|int|Specifies the starting page number of the section. The 'RestartPageNumbering' property, if set to false, will override the 'PageStartingNumber' property so that page numbering can continue from the previous section.|
|PageWidth|double|Specifies the width of the page in points.|
|PaperSize|PaperSize|Specifies the paper size. Setting this property updates 'PageWidth' and 'PageHeight' values. Setting this value to 'Custom' does not change existing values.|
|RestartPageNumbering|bool|True if page numbering restarts at the beginning of the section. If set to false, the 'RestartPageNumbering' property will override the 'PageStartingNumber' property so that page numbering can continue from the previous section.|
|RightMargin|double|Specifies the distance (in points) between the right edge of the page and the right boundary of the body text.|
|RtlGutter|bool|Specifies whether Microsoft Word uses gutters for the section based on a right-to-left language or a left-to-right language.|
|SectionStart|SectionStart|Specifies the type of section break for the specified object.|
|SuppressEndnotes|bool|True if endnotes are printed at the end of the next section that doesn't suppress endnotes. Suppressed endnotes are printed before the endnotes in that section.|
|TopMargin|double|Specifies the distance (in points) between the top edge of the page and the top boundary of the body text.|
|VerticalAlignment|PageVerticalAlignment|Specifies the vertical alignment of text on each page in a document or section.|

## REST API

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Sections/UpdateSectionPageSetup) lets you call this REST API directly from a browser.

You can also use cURL command-line utility to test this REST API. The following are a few examples of using cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to update sections's page setup properties
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/pageSetup" \
-X PUT \
-d "{ 'LeftMargin': 99, 'Orientation': 'Landscape', 'PaperSize': 'A5' }" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

<p style="margin:0;font-size:80%;font-style:italic">To get a jwt token use this <a href="/words/getting-started/available-sdks/#curl">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}

```json
{
  "PageSetup": {
    "Bidi": false,
    "BorderAlwaysInFront": true,
    "BorderAppliesTo": "AllPages",
    "BorderDistanceFrom": "Text",
    "BottomMargin": 56.7,
    "DifferentFirstPageHeaderFooter": false,
    "FirstPageTray": 0,
    "FooterDistance": 42.5,
    "Gutter": 0.0,
    "HeaderDistance": 35.45,
    "LeftMargin": 99.0,
    "LineNumberCountBy": 0,
    "LineNumberDistanceFromText": 0.0,
    "LineNumberRestartMode": "RestartPage",
    "LineStartingNumber": 1,
    "Orientation": "Landscape",
    "OtherPagesTray": 0,
    "PageHeight": 419.55,
    "PageNumberStyle": "Arabic",
    "PageStartingNumber": 1,
    "PageWidth": 595.3,
    "PaperSize": "A5",
    "RestartPageNumbering": false,
    "RightMargin": 56.7,
    "RtlGutter": true,
    "SectionStart": "NewPage",
    "SuppressEndnotes": false,
    "TopMargin": 56.7,
    "VerticalAlignment": "Top",
    "link": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/pagesetup",
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

The following set of **Code Examples** for various SDKs demonstrates how to use this REST API in your projects:

{{< nosnippet >}}
{{< tabs tabTotal="9" tabID="4" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "19215e2ac3d61ca0fd78d1ca2f1c1023" "UpdateSectionPageSetup.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "UpdateSectionPageSetup.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-cloud" "163e730223a72524d163ef9c017f1b1a" "UpdateSectionPageSetup.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "UpdateSectionPageSetup.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "UpdateSectionPageSetup.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "UpdateSectionPageSetup.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_UpdateSectionPageSetup.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_GetSectionPage.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "UpdateSectionPageSetup.go" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
