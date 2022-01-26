---
title: "Read the Page Setup of a Section"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /sections/read/
aliases: [/read-the-page-setup-of-a-section/]
keywords: "page setup word,get sections,section break word,Section Break, Word, Microsoft Word, Word Documents"
description: "Read a page setup of a section in a Word document"
weight: 30
---

This REST API reads a page setup of a `Section`. 

The resource properties are the following:

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

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Sections/GetSectionPageSetup) defines a publicly accessible programming interface and lets you carry out REST interactions directly from a web browser.

You can use **cURL** command-line tool to access Aspose.Words web services easily. The following example shows how to make calls to Cloud API with cURL.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```bash
# cURL example to get setup of section
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/pageSetup" \
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
    "LeftMargin": 56.7,
    "LineNumberCountBy": 0,
    "LineNumberDistanceFromText": 0.0,
    "LineNumberRestartMode": "RestartPage",
    "LineStartingNumber": 1,
    "Orientation": "Portrait",
    "OtherPagesTray": 0,
    "PageHeight": 841.9,
    "PageNumberStyle": "Arabic",
    "PageStartingNumber": 1,
    "PageWidth": 595.3,
    "PaperSize": "A4",
    "RestartPageNumbering": false,
    "RightMargin": 56.7,
    "RtlGutter": true,
    "SectionStart": "NewPage",
    "SuppressEndnotes": false,
    "TopMargin": 56.7,
    "VerticalAlignment": "Top",
    "link": {
      "Href": "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/sections/0/pagesetup",
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
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetSectionPageSetupOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetSectionPageSetupOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetSectionPageSetupOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetSectionPageSetupOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetSectionPageSetupOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetSectionPageSetupOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetSectionPageSetupOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetSectionPageSetupOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetSectionPageSetupOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetSectionPageSetupOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
