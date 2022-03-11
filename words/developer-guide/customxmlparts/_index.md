---
title: "Custom XML Parts"
type: docs
url: /customxmlparts/
aliases: [/custom-xml-parts/, /custom-xml-part/]
description: "Learn how to work with Custom XML parts in a Word document"
weight: 40
---

With the release of Office 2007, Microsoft introduced developers to a new XML-based format for representing office documents — Open Office XML or OOXML for short. DOCX, XLSX and PPTX are well-known representatives of the OOXML format that underlies them.

OOXML quickly gained popularity as it allowed programmers to easily manipulate document data, as well as perform data integration with third-party software. Compared to previous binary office formats such as DOC, XLS, PPT, the new document format provided greater security and greater resistance to data corruption.


## What are 'Custom XML Parts'

'Custom XML Parts' is external arbitrary data embedded in a Word document. Once you've embedded XML in a document, you can bind it to a content control to visualize it. If you introduce changes to the data displayed on the content control, this will automatically lead to changes in the source XML data.
 
Programmatically, custom XML is a collection of XML data. You can create new data elements, modify or delete existing ones:

<table>
  <thead>
    <tr>
      <th style="text-align:center;"></th>
      <th><i>Request</i></th>
      <th><i>Response</i></th>
      <th><i>Model</i></th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Delete</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#deletecustomxmlpartonlinerequest">DeleteCustomXmlPartOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#deletecustomxmlpartrequest">DeleteCustomXmlPartRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#deletecustomxmlpartsonlinerequest">DeleteCustomXmlPartsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Dictionary<string,Stream></span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#deletecustomxmlpartsrequest">DeleteCustomXmlPartsRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" colspan="2"><span style="color:SteelBlue;">Task</span></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="4"><strong><i>Get</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#getcustomxmlpartonlinerequest">GetCustomXmlPartOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="/words/spec/customxmlpart/#customxmlpartresponse">CustomXmlPartResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="/words/spec/customxmlpart/#customxmlpart">CustomXmlPart</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#getcustomxmlpartrequest">GetCustomXmlPartRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#getcustomxmlpartsonlinerequest">GetCustomXmlPartsOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="/words/spec/customxmlpart/#customxmlpartsresponse">CustomXmlPartsResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><a href="/words/spec/customxmlpart/#customxmlpartscollection">CustomXmlPartsCollection</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#getcustomxmlpartsrequest">GetCustomXmlPartsRequest</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Insert</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#insertcustomxmlpartonlinerequest">InsertCustomXmlPartOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#insertcustomxmlpartonlineresponse">InsertCustomXmlPartOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#customxmlpartinsert">CustomXmlPartInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#insertcustomxmlpartrequest">InsertCustomXmlPartRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#customxmlpartresponse">CustomXmlPartResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#customxmlpart">CustomXmlPart</a></br><a href="/words/spec/customxmlpart/#customxmlpartinsert">CustomXmlPartInsert</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white" rowspan="2"><strong><i>Update</i><strong></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#updatecustomxmlpartonlinerequest">UpdateCustomXmlPartOnlineRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#updatecustomxmlpartonlineresponse">UpdateCustomXmlPartOnlineResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#customxmlpartupdate">CustomXmlPartUpdate</a></td>
  </tr>
  <tr>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#updatecustomxmlpartrequest">UpdateCustomXmlPartRequest</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#customxmlpartresponse">CustomXmlPartResponse</a></td>
    <td style="vertical-align:middle;" class="bg-white"><a href="/words/spec/customxmlpart/#customxmlpart">CustomXmlPart</a></br><a href="/words/spec/customxmlpart/#customxmlpartupdate">CustomXmlPartUpdate</a></td>
  </tr>
  </tbody>
</table>

## Usage examples with cURL and Postman

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

Download sample [compareTestDoc1.doc](compareTestDoc1.doc), [compareTestDoc2.doc](compareTestDoc2.doc) files for testing purposes.

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="cURL Request" tabName2="Postman Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetCustomXmlPartOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetCustomXmlPartOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Aspose.Words Cloud SDK Family

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Usage examples in Python, Java, C#, etc.

The following code samples show how to interact with the REST API using almost any mainstream programming language.

You can find a lot of other examples in [Python](https://gist.github.com/aspose-words-cloud-gists/e26813ced70692c544820cd8011ee7e0), [Java](https://gist.github.com/aspose-words-cloud-gists/caede439bfd2e57c3010befe504faff4), [C#](https://gist.github.com/aspose-words-cloud-gists/374e1e3dd4bca8f696f29d913645f549), [JavaScript](https://gist.github.com/aspose-words-cloud-gists/a9510e4b51613f1138e7c1ec09634c4a), [PHP](https://gist.github.com/aspose-words-cloud-gists/e2a72445b96362dc0117f06ab54bb94a), [C++](https://gist.github.com/aspose-words-cloud-gists/49aa5151a094849179bae8672c887a0e), [Golang](https://gist.github.com/aspose-words-cloud-gists/625ca80adffd779e8f6e3611551e14d5), [Ruby](https://gist.github.com/aspose-words-cloud-gists/339f3835a4c0a536c81ec941de29baf7), [Swift](https://gist.github.com/aspose-words-cloud-gists/790dbd2edd5d36f170732366f52cac4c), [Dart](https://gist.github.com/aspose-words-cloud-gists/6aae628cf2b878b78fea177c3171c6bf) on GitHub. All codes are thoroughly tested and ready for production use.

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="4" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetCustomXmlPartOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetCustomXmlPartOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetCustomXmlPartOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetCustomXmlPartOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetCustomXmlPartOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetCustomXmlPartOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetCustomXmlPartOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetCustomXmlPartOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "CompareDocumentOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "CompareDocumentOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
