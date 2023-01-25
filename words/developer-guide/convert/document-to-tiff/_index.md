---
title: "Convert Word document to TIFF image format"
second_title: " online"
articleTitle: "Convert Word document to TIFF image format"
linktitle: "Convert Word document to TIFF image format"
type: docs
url: /convert/document-to-tiff/
description: "Convert Word document to TIFF image format programmatically via Cloud API."
weight: 30
---

Aspose.Words Cloud API includes a `SaveAsTiffOnline` method that allows developers to convert a Word document to the TIFF image format using detailed conversion settings.
The TIFF (Tagged Image File Format) format is a widely used graphics format. One of the key features of the TIFF format is its ability to support multiple pages. This makes it a popular choice when working with documents such as multi-page drawings, photographs, and scanned documents. TIFF files can also be saved in a variety of color depths, including grayscale, which makes it a versatile format for a wide range of applications.
Another advantage of the TIFF format is its support for lossless compression. When a TIFF image is compressed, no information is lost, and the image can be restored to its original quality. This feature makes the TIFF format ideal for archiving and editing images, as well as for high-quality printing. Compared to other image formats such as JPG and PNG, TIFF is a more suitable for printing, as it supports CMYK color model while JPG and PNG support RGB.

## Convert Word document to TIFF image format REST API

| Server                         | Method | Endpoint             |
|--------------------------------|--------|----------------------|
| https://api.aspose.cloud/v4.0  | PUT    | /words/online/put/saveAs/tiff |

You can use the following parameters in a REST request:

| Parameter Name       | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `loadEncoding`       | string    | Optional           | Encoding that will be used to load an HTML (or TXT) document if the encoding is not specified in HTML. |
| `password`           | string    | Optional           | Password of protected Word document. Use the parameter to pass a password via SDK. SDK encrypts it automatically. We don't recommend to use the parameter to pass a plain password for direct call of API. |
| `encryptedPassword`  | string    | Optional           | Password of protected Word document. Use the parameter to pass an encrypted password for direct calls of API. See SDK code for encyption details. |
| `useAntiAliasing`    | boolean   | Optional           | The flag indicating whether to use antialiasing.             |
| `useHighQualityRendering` | boolean   | Optional           | The flag indicating whether to use high quality.             |
| `imageBrightness`    | number(double) | Optional           | The level of brightness for the generated images.            |
| `imageColorMode`     | string    | Optional           | The color mode for the generated images.                     |
| `imageContrast`      | number(double) | Optional           | The contrast for the generated images.                       |
| `numeralFormat`      | string    | Optional           | The images numeral format.                                   |
| `pageCount`          | integer(int32) | Optional           | The number of pages to render.                               |
| `pageIndex`          | integer(int32) | Optional           | The index of the page to start rendering.                    |
| `paperColor`         | string    | Optional           | The background image color.                                  |
| `pixelFormat`        | string    | Optional           | The pixel format of the generated images.                    |
| `resolution`         | number(double) | Optional           | The resolution of the generated images.                      |
| `scale`              | number(double) | Optional           | The zoom factor for the generated images.                    |
| `tiffCompression`    | string    | Optional           | The compression tipe.                                        |
| `dmlRenderingMode`   | string    | Optional           | The optional dml rendering mode. The default value is Fallback. |
| `dmlEffectsRenderingMode` | string    | Optional           | The optional dml effects rendering mode. The default value is Simplified. |
| `tiffBinarizationMethod` | string    | Optional           | The optional TIFF binarization method. Possible values are: FloydSteinbergDithering, Threshold. |
| `zipOutput`          | boolean   | Optional           | The flag indicating whether to ZIP the output.               |
| `fontsLocation`      | string    | Optional           | Folder in filestorage with custom fonts.                     |


Use `$multipart/form-data` request to combine one or more properties into a single body:

| Property Name        | Data Type | Required/Optional  | Description                     |
|----------------------|-----------|--------------------|---------------------------------|
| `document`           | string(binary) | Required           | The document.                                                |
| `saveOptions`        | TiffSaveOptionsData | Required           | Tiff save options.                                           |

{{% alert style="info" %}}
**Note**: to access this REST API, you need to register and get personal credentials. Use the '[Quick Start](/words/getting-started/quickstart/)' guide to go through the procedure in a couple of minutes.
{{% /alert %}}


## Convert Word document to TIFF image format usage examples

Let's look at practical examples of using the web service. You can do this both with cURL and Postman utilities, and from your code in various programming languages: Python, Java, JavaScript, C#, PHP, C++, Go, Ruby, Swift, Dart.

### How to convert Word document to TIFF image format with cURL or Postman

One of the easiest and fastest ways to call a REST API is to use cURL or Postman:

{{< nosnippet >}}
{{< tabs tabTotal="2" tabID="1" tabName1="cURL Request" tabName2="Postman Request" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "SaveAsTiffOnline.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "SaveAsTiffOnline.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use these <a href="/words/getting-started/quickstart/">instructions</a></p>

{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


### How to convert Word document to TIFF image format in Python, Java, C#, C++, JavaScript and other programming languages

Using SDK is the quickest way to speed up the development. Please take a look at the provided code examples to quickly call this web service from your favourite programming language:

{{< nosnippet >}}
{{< tabs tabTotal="10" tabID="2" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "SaveAsTiffOnline.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "SaveAsTiffOnline.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "SaveAsTiffOnline.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "SaveAsTiffOnline.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "SaveAsTiffOnline.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "SaveAsTiffOnline.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "SaveAsTiffOnline.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "SaveAsTiffOnline.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "SaveAsTiffOnline.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "SaveAsTiffOnline.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}


## See Also

 * [GitHub repository](https://github.com/aspose-words-cloud) — explore Aspose.Words Cloud SDK Family. These software libraries take care of all low-level document-processing details.


