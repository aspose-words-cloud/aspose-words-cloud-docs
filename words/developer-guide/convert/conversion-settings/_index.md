---
title: "Convert Document to Destination Format with Detailed Settings"
type: docs
url: /convert/conversion-settings/
aliases: [/convert-document-to-destination-format-with-detailed-settings-and-save-result-to-storage/]
keywords: "microsoft word document,convert to, word to doc, save word file as pdf,convert word document to html,word doc to html,convert pdf to word,tiff file,Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift"
description: "The API lets you convert word document to HTML, PDF, JPEG, or other formats with detailed settings. The list of supported formats is, BMP, DOC, DOCM, EMF, and more. The Apose.Words Cloud supports, Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift."
weight: 20
---

This API lets you convert Word-based document to another format, while specifying the target format options.

## Supported Formats

The following table lists the file formats, that Words Cloud API supports for data conversions.

|format Parameter Value|Request Types|
| :- | :- |
|bmp|BmpSaveOptions|
|doc|DocSaveOptions|
|docm|OoxmlSaveOptions|
|docx|OoxmlSaveOptions|
|dot|DocSaveOptions|
|dotm|OoxmlSaveOptions|
|dotx|OoxmlSaveOptions|
|emf|EmfSaveOptions|
|epub|EpubSaveOptions|
|flatopc/fopc|OoxmlSaveOptions|
|flatopc_macro/fopc_macro|OoxmlSaveOptions|
|flatopc_template/fopc_template|OoxmlSaveOptions|
|flatopc_template_macro/fopc_template_macro|OoxmlSaveOptions|
|gif|GifSaveOptions|
|html|HtmlSaveOptions|
|htmlfixed|HtmlFixedSaveOptions|
|jpeg/jpg|JpegSaveOptions|
|mhtml/mht|MhtmlSaveOptions|
|odt|OdtSaveOptions|
|openxps|XpsSaveOptions|
|ott|OdtSaveOptions|
|pcl|PclSaveOptions|
|pdf|PdfSaveOptions|
|png|PngSaveOptions|
|ps|PsSaveOptions|
|rtf|Rich Text Format File|
|svg|SvgSaveOptions|
|swf|Shockwave Flash Movie(removed)|
|text/txt|TextSaveOptions|
|tiff/tif|TiffSaveOptions|
|wordml/wml|WordMLSaveOptions|
|xamlfixed|XamlFixedSaveOptions|
|xamlflow|XamlFlowSaveOptions|
|xps|XpsSaveOptions|

The most important parameters of this API are listed in the following table:

|Parameter Name|Description|Default Value|
| :- | :- | :- |
|SaveFormat|Format of the output file.| |
|FileName|Name of the destination file.| |
|DmlRenderingMode|A value determining how DrawingML shapes are rendered. Fallback, DrawingML.|DrawingML|
|DmlEffectsRenderingMode|A value determining how DrawingML effects are rendered. Simplified, None, Fine.|Simplified|
|ZipOutput|A value determining zip output or not.|false|
|ColorMode|Gets or sets a value determining how colors are rendered.|Normal|
|UpdateSdtContent|Gets or sets a value determining whether the content of Aspose.Words.Markup.StructuredDocumentTag" is updated before saving.|True|
|UpdateFields|Gets or sets a value determining if fields should be updated before saving the document to a fixed page format.|True|

**NOTE**

All elements, except **SaveFormat** and **FileName**, can be omitted. If we omit an element, then the element will contain default value.

## REST API’s Resources

The [OpenAPI Specification](https://apireference.aspose.cloud/words/#/Convert/SaveAs) lets you call this REST API directly from a browser.

## cURL Example

The following are a few examples of using cURL:

{{< tabs tabTotal="2" tabID="25" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}

```JAVA
# Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
# Place App_Key in "client_secret" and App_SID in "client_id" argument.
curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

# cURL example to convert MS Word Document to PDF using PDFSaveOptions
curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/saveAs" \
-X PUT \
-d "{'SaveFormat':'pdf', 'FileName': 'test_multi_pages.pdf'}" \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>"
```

{{< /tab >}}
{{< tab tabNum="2" >}}

```JAVA
{
  "SaveResult": {
    "SourceDocument": {
      "Href": "http://api.aspose.cloud/v4.0/words/test_multi_pages.docx",
      "Rel": "self",
      "Type": null,
      "Title": null
    },
    "DestDocument": {
      "Href": "test_multi_pages.pdf",
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

## Boost the Development Process with Aspose Words Cloud SDK Family

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks.

Please check out the [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples.

A set of short code examples, demonstrating how to use this REST API with various SDKs, is presented below:

{{< tabs tabTotal="9" tabID="28" tabName1="C#" tabName2="Java" tabName3="PHP" tabName4="Python" tabName5="Ruby" tabName6="Node.js" tabName7="Android" tabName8="Swift" tabName9="Go" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-cloud" "9fa2e714041dd6cf1071eb307b623416" "ConvertWordDocumentToAnotherFormatWithDetailedSettings.cs" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-cloud" "7d6af3eba6f989851e6475842125f31d" "ConvertWordDocumentToAnotherFormatWithDetailedSettings.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "" "163e730223a72524d163ef9c017f1b1a" "ConvertWordDocumentToAnotherFormatWithDetailedSettings.php" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-cloud" "fb014f439299bbee24472cb0efa6d50b" "ConvertWordDocumentToAnotherFormatWithDetailedSettings.py" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-cloud" "3f3f4f7033ae386af05042ee2ad3aa06" "ConvertWordDocumentToAnotherFormatWithDetailedSettings.rb" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-cloud" "715d05011a94ac77f67b21213de5da7f" "ConvertWordDocumentToAnotherFormatWithDetailedSettings.js" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-cloud" "5240b25c9a3e98fb21785ad771a3876b" "Aspose_Cloud_Words_ConvertWordDocumentToAnotherFormatWithDetailedSettings.java" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-cloud" "982e9b4809b6aca96fbb13b47a1184d5" "Aspose_Words_Swift_ConvertWordDocumentToAnotherFormatWithDetailedSettings.swift" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-cloud" "068ce2149de5ad69ab516209b7ae82cf" "ConvertWordDocumentToAnotherFormatWithDetailedSettings.go" >}}
{{< /tab >}}
{{< /tabs >}}

## Saving a BMP Image

The **BmpSaveOptions** XML definition is presented below:

```XML
<BmpSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <ColorMode>{Normal | Grayscale }</ColorMode><!-- the default is 'Normal' -->
   <!-- specific part -->
   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- the default is 'false' -->
   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- the default is 'false' -->
   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- the default is 'true' -->
   <ImageBrightness>{float_number}</ImageBrightness><!-- the default is 0.5 -->
   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- the default is 'None' -->
   <ImageContrast>{float_number}</ImageContrast><!-- the default is 0.5 -->
   <GraphicsQualityOptions>
      <CompositingMode>{SourceOver | SourceOver}</CompositingMode><!-- the default is 'null' -->
      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality><!-- the default is 'null' -->
      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- the default is 'null' -->
      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- the default is 'null' -->
      <StringFormat>
        <Alignment>{Center | Far | Near} </Alignment><!-- the default is 'null' -->
        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags><!-- the default is 'null' -->
        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix><!-- the default is 'null' -->
        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming><!-- the default is 'null' -->
        <LineAlignment>{Center | Far | Near}</LineAlignment><!-- the default is 'null' -->
      </StringFormat>
      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- the default is 'null' -->
   </GraphicsQualityOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <MetafileRenderingOptions><!-- always present -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'Bitmap' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
      <EmulateRasterOperations>{true/false}</EmulateRasterOperations> <!-- Gets or sets a value determining whether or not the raster operations should be emulated. -->
   </MetafileRenderingOptions>
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <PaperColor>{color}</PaperColor><!-- the default is 'WHITE' -->
   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- the default is 'Format32BppArgb' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <Resolution>{float_number}</Resolution><!-- the default is '96' -->
   <HorizontalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <VerticalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <Scale>{float_number}</Scale><!-- the default is 1.0 -->
</BmpSaveOptions>
```

## Saving a Document (DOC, DOT)

The **DocSaveOptions** XML definition is presented below:

```XML
<DocSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <Password>{string}</Password><!-- the default is "" -->
   <SaveRoutingSlip>{true/false}</SaveRoutingSlip><!-- the default is 'true' -->
</DocSaveOptions>
```

## Saving an OOXML (DOCX, DOCM, DOTX, DOTM, FLATOPC)

The **OoxmlSaveOptions** XML definition is presented below:

```XML
<OoxmlSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <PrettyFormat>{true/false}</PrettyFormat><!-- the default is 'false' -->
   <Compliance>{Ecma376_2006/Iso29500_2008_Transitional}</Compliance><!-- the default is 'Ecma376_2006' -->
   <Password>{string}</Password><!-- the default is "" -->
</OoxmlSaveOptions>
```

## Saving an EMF Image

The **EmfSaveOptions** XML definition is presented below:

```XML
<EmfSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <ImageBrightness>{float_number}</ImageBrightness><!-- the default is 0.5 -->
   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- the default is 'None' -->
   <ImageContrast>{float_number}</ImageContrast><!-- the default is 0.5 -->
   <GraphicsQualityOptions>
      <CompositingMode>{SourceOver | SourceOver}</CompositingMode><!-- the default is 'null' -->
      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality><!-- the default is 'null' -->
      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- the default is 'null' -->
      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- the default is 'null' -->
      <StringFormat>
        <Alignment>{Center | Far | Near} </Alignment><!-- the default is 'null' -->
        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags><!-- the default is 'null' -->
        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix><!-- the default is 'null' -->
        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming><!-- the default is 'null' -->
        <LineAlignment>{Center | Far | Near}</LineAlignment><!-- the default is 'null' -->
      </StringFormat>
      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- the default is 'null' -->
   </GraphicsQualityOptions>
   <MetafileRenderingOptions><!-- always present -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'Bitmap' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <PaperColor>{color}</PaperColor><!-- the default is 'WHITE' -->
   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- the default is 'Format32BppArgb' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <Resolution>{float_number}</Resolution><!-- the default is '96' -->
   <HorizontalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <VerticalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <Scale>{float_number}</Scale><!-- defaulHtmlSaveOptionst value = 1.0 -->
   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- the default is 'true' -->
</EmfSaveOptions>
```

## Saving an EPUB Document

The **EpubSaveOptions** XML definition is presented below:

```XML
<EpubSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <PrettyFormat>{true/false}</PrettyFormat><!-- the default is 'false' -->
   <AllowNegativeIndent>{true/false}</AllowNegativeIndent><!-- the default is 'false' -->
   <CssStyleSheetType>{Embedded/External/Inline}</CssStyleSheetType><!-- the default is 'External' -->
   <DocumentSplitCriteria>{ColumnBreak/HeadingParagraph/None/PageBreak/SectionBreak}</DocumentSplitCriteria><!-- the default is 'HeadingParagraph' -->
   <DocumentSplitHeadingLevel>{number}</DocumentSplitHeadingLevel><!-- the default is '2' -->
   <Encoding>{string}</Encoding><!-- the default is "UTF-8" -->
   <EpubNavigationMapLevel>{number}</EpubNavigationMapLevel><!-- the default is '3' -->
   <ExportDocumentProperties>{true/false}</ExportDocumentProperties><!-- the default is 'false' -->
   <ExportFontsAsBase64>{true/false}</ExportFontsAsBase64><!-- the default is 'false' -->
   <ExportFontResources>{true/false}</ExportFontResources><!-- the default is false -->   <ExportHeadersFootersMode>{FirstSectionHeaderLastSectionFooter/None/PerSection}</ExportHeadersFootersMode><!-- the default is 'None' -->
   <ExportImagesAsBase64>{true/false}</ExportImagesAsBase64><!-- the default is 'false' -->
   <ExportLanguageInformation>{true/false}</ExportLanguageInformation><!-- the default is 'false' -->
   <ExportListLabels>{Auto/AsInlineText/ByHtmlTags}</ExportListLabels><!-- the default is 'Auto' -->
   <ExportMetafileAsRaster>{true/false}</ExportMetafileAsRaster><!-- the default is 'true' -->
   <ExportOriginalUrlForLinkedImages>{true/false}</ExportOriginalUrlForLinkedImages><!-- the default is 'false' -->
   <ExportPageSetup>{true/false}</ExportPageSetup><!-- the default is 'false' -->
   <ExportRelativeFontSize>{true/false}</ExportRelativeFontSize><!-- the default is 'false' -->
   <ExportRoundtripInformation>{true/false}</ExportRoundtripInformation><!-- the default is 'true' -->
   <ExportTextBoxAsSvg>{true/false}</ExportTextBoxAsSvg><!-- the default is 'false' -->
   <ExportTextInputFormFieldAsText>{true/false}</ExportTextInputFormFieldAsText><!-- the default is 'false' -->
   <ExportTocPageNumbers>{true/false}</ExportTocPageNumbers><!-- the default is 'false' -->
   <FontResourcesSubsettingSizeThreshold>{number}</FontResourcesSubsettingSizeThreshold><!-- the default is '0' -->
   <HtmlVersion>{Xhtml| Html5}</HtmlVersion><!-- the default is "Xhtml" -->
   <ImageResolution>{number}</ImageResolution><!-- the default is '96' -->
   <OfficeMathOutputMode>{Image/MathML/Text}</OfficeMathOutputMode><!-- the default is 'Image' -->
   <ResourceFolder>{string}</ResourceFolder><!-- the default is an empty string -->
   <ResourceFolderAlias>{string}</ResourceFolderAlias><!-- the default is an empty string -->
   <ScaleImageToShapeSize>{true/false}</ScaleImageToShapeSize><!-- the default is 'true' -->
   <TableWidthOutputMode>{All/None/RelativeOnly}</TableWidthOutputMode><!-- the default is 'All' -->
</EpubSaveOptions>
```

## Saving a GIF

The **GifSaveOptions** XML definition is presented below:

```XML
<GifSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <ColorMode>{Normal | Grayscale }</ColorMode><!-- the default is 'Normal' -->
   <!-- specific part -->
   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- the default is 'false' -->
   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- the default is 'false' -->
   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- the default is 'true' -->
   <ImageBrightness>{float_number}</ImageBrightness><!-- the default is 0.5 -->
   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- the default is 'None' -->
   <ImageContrast>{float_number}</ImageContrast><!-- the default is 0.5 -->
   <GraphicsQualityOptions>
      <CompositingMode>{SourceOver | SourceOver}</CompositingMode><!-- the default is 'null' -->
      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality><!-- the default is 'null' -->
      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- the default is 'null' -->
      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- the default is 'null' -->
      <StringFormat>
        <Alignment>{Center | Far | Near} </Alignment><!-- the default is 'null' -->
        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags><!-- the default is 'null' -->
        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix><!-- the default is 'null' -->
        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming><!-- the default is 'null' -->
        <LineAlignment>{Center | Far | Near}</LineAlignment><!-- the default is 'null' -->
      </StringFormat>
      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- the default is 'null' -->
   </GraphicsQualityOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <MetafileRenderingOptions><!-- always present -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'Bitmap' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
      <ScaleWmfFontsToMetafileSize>{true/false}</ScaleWmfFontsToMetafileSize> <!-- Gets or sets a value determining whether or not to scale fonts in WMF metafile according to metafile size on the page. -->
   </MetafileRenderingOptions>
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <PaperColor>{color}</PaperColor><!-- the default is 'WHITE' -->
   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- the default is 'Format32BppArgb' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <Resolution>{float_number}</Resolution><!-- the default is '96' -->
   <HorizontalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <VerticalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <Scale>{float_number}</Scale><!-- the default is 1.0 -->
</GifSaveOptions>
```

## Saving a HTML

The **HtmlSaveOptions** XML definition is presented below:

```XML
<HtmlSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <PrettyFormat>{true/false}</PrettyFormat><!-- the default is 'false' -->
   <AllowNegativeIndent>{true/false}</AllowNegativeIndent><!-- the default is 'false' -->
   <CssStyleSheetFileName>{string}</CssStyleSheetFileName><!-- the default is "" -->
   <CssStyleSheetType>{Embedded/External/Inline}</CssStyleSheetType><!-- the default is 'Inline' -->
   <DocumentSplitCriteria>{ColumnBreak/HeadingParagraph/None/PageBreak/SectionBreak}</DocumentSplitCriteria><!-- the default is 'None' -->
   <DocumentSplitHeadingLevel>{number}</DocumentSplitHeadingLevel><!-- the default is '2' -->
   <Encoding>{string}</Encoding><!-- the default is "UTF-8" -->
   <ExportDocumentProperties>{true/false}</ExportDocumentProperties><!-- the default is 'false' -->
   <ExportFontsAsBase64>{true/false}</ExportFontsAsBase64><!-- the default is 'false' -->
   <ExportFontResources>{true/false}</ExportFontResources><!-- the default is 'false' -->
   <ExportHeadersFootersMode>{FirstSectionHeaderLastSectionFooter/None/PerSection}</ExportHeadersFootersMode><!-- the default is 'PerSection' -->
   <ExportImagesAsBase64>{true/false}</ExportImagesAsBase64><!-- the default is 'false' -->
   <ExportLanguageInformation>{true/false}</ExportLanguageInformation><!-- the default is 'false' -->
   <ExportListLabels>{Auto/AsInlineText/ByHtmlTags}</ExportListLabels><!-- the default is 'Auto' -->
   <ExportMetafileAsRaster>{true/false}</ExportMetafileAsRaster><!-- the default is 'true' -->
   <ExportOriginalUrlForLinkedImages>{true/false}</ExportOriginalUrlForLinkedImages><!-- the default is 'false' -->
   <ExportPageSetup>{true/false}</ExportPageSetup><!-- the default is 'false' -->
   <ExportPageMargins>{true/false}</ExportPageMargins><!-- the default is 'false' -->
   <ExportRelativeFontSize>{true/false}</ExportRelativeFontSize><!-- the default is 'false' -->
   <ExportRoundtripInformation>{true/false}</ExportRoundtripInformation><!-- the default is 'true' -->
   <ExportTextBoxAsSvg>{true/false}</ExportTextBoxAsSvg><!-- the default is 'false' -->
   <ExportTextInputFormFieldAsText>{true/false}</ExportTextInputFormFieldAsText><!-- the default is 'false' -->
   <ExportTocPageNumbers>{true/false}</ExportTocPageNumbers><!-- the default is 'false' -->
   <ExportXhtmlTransitional>{true/false}</ExportXhtmlTransitional><!-- the default is 'false' -->
   <FontResourcesSubsettingSizeThreshold>{number}</FontResourcesSubsettingSizeThreshold><!-- the default is '0' -->
   <FontsFolder>{string}</FontsFolder><!-- the default is "" -->
   <FontsFolderAlias>{string}</FontsFolderAlias><!-- the default is "" -->
   <HtmlVersion>{Xhtml| Html5}</HtmlVersion><!-- the default is "Xhtml" -->
   <ImageResolution>{number}</ImageResolution><!-- the default is '96' -->
   <ImagesFolder>{string}</ImagesFolder><!-- the default is "" -->
   <ImagesFolderAlias>{string}</ImagesFolderAlias><!-- the default is "" -->
   <OfficeMathOutputMode>{Image/MathML/Text}</OfficeMathOutputMode><!-- the default is 'Image' -->
   <ResourceFolder>{string}</ResourceFolder><!-- the default is an empty string -->
   <ResourceFolderAlias>{string}</ResourceFolderAlias><!-- the default is an empty string -->
   <ScaleImageToShapeSize>{true/false}</ScaleImageToShapeSize><!-- the default is 'true' -->
   <TableWidthOutputMode>{All/None/RelativeOnly}</TableWidthOutputMode><!-- the default is 'All' -->
   <ExportDropDownFormFieldAsText>{true/false}</ExportDropDownFormFieldAsText><!-- the default is 'false' -->
   <ResolveFontNames>{true/false}</ResolveFontNames> <!-- Specifies whether font family names used in the document are resolved and substituted according to FontSettings when being written into HTML-based formats. -->
</HtmlSaveOptions>
```

## Saving a fixed HTML

The **HtmlFixedSaveOptions** XML definition is presented below:

```XML
<HtmlFixedSaveOptions>
   <!-- common part -->
   <CssClassNamesPrefix>{string}</CssClassNamesPrefix><!-- the default is 'aw' -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <ExportEmbeddedCss>{true/false}</ExportEmbeddedCss><!-- the default is 'false' -->
   <ExportEmbeddedFonts>{true/false}</ExportEmbeddedFonts><!-- the default is 'false' -->
   <ExportEmbeddedImages>{true/false}</ExportEmbeddedImages><!-- the default is 'false' -->
   <ExportFormFields>{true/false}</ExportFormFields><!-- the default is 'false' -->
   <Encoding>ASCII</Encoding><!-- the default is 'UTF8' -->
   <FontFormat>{Tft/Woff}</FontFormat><!-- the default is 'Woff' -->
   <JpegQuality>{number}</JpegQuality><!-- the default is '95' -->
   <MetafileRenderingOptions><!-- always present -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'VectorWithFallback' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageCount>{number}</PageCount><!-- the default is Int32.MaxValue -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <PageHorizontalAlignment>{Left/Center/Right}</PageHorizontalAlignment><!-- the default is "Center" -->
   <PageMargins>{double}</PageMargins><!-- the default is '10' -->
   <ResourcesFolder>{string}</ResourcesFolder><!-- the default is "" -->
   <ResourcesFolderAlias>{string}</ResourcesFolderAlias><!-- the default is "" -->
   <ShowPageBorder>{true/false}</ShowPageBorder><!-- the default is 'true' -->
</HtmlFixedSaveOptions>
```

## Saving a JPEG Image

The **JpegSaveOptions** XML definition is presented below:

```XML
<JpegSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- the default is 'false' -->
   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- the default is 'false' -->
   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- the default is 'true' -->
   <ImageBrightness>{float_number}</ImageBrightness><!-- the default is 0.5 -->
   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- the default is 'None' -->
   <ImageContrast>{float_number}</ImageContrast><!-- the default is 0.5 -->
   <GraphicsQualityOptions>
      <CompositingMode>{SourceOver | SourceOver}</CompositingMode><!-- the default is 'null' -->
      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality><!-- the default is 'null' -->
      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- the default is 'null' -->
      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- the default is 'null' -->
      <StringFormat>
        <Alignment>{Center | Far | Near} </Alignment><!-- the default is 'null' -->
        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags><!-- the default is 'null' -->
        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix><!-- the default is 'null' -->
        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming><!-- the default is 'null' -->
        <LineAlignment>{Center | Far | Near}</LineAlignment><!-- the default is 'null' -->
      </StringFormat>
      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- the default is 'null' -->
   </GraphicsQualityOptions>
   <JpegQuality>{number}</JpegQuality><!-- the default is '95' -->
   <MetafileRenderingOptions><!-- always present -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'Bitmap' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <PaperColor>{color}</PaperColor><!-- the default is 'WHITE' -->
   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- the default is 'Format32BppArgb' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <Resolution>{float_number}</Resolution><!-- the default is '96' -->
   <HorizontalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <VerticalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <Scale>{float_number}</Scale><!-- the default is 1.0 -->
</JpegSaveOptions>
```

## Saving a MHTML

The **MhtmlSaveOptions** XML definition is presented below:

```XML
<MhtmlSaveOptions>
 <!-- common part -->
 <SaveFormat>{string}</SaveFormat>
 <FileName>{string}</FileName>
 <!-- specific part -->
 <PrettyFormat>{true/false}</PrettyFormat><!-- the default is 'false' -->
 <AllowNegativeIndent>{true/false}</AllowNegativeIndent><!-- the default is 'false' -->
 <CssStyleSheetType>{Embedded/External/Inline}</CssStyleSheetType><!-- the default is 'Inline' -->
 <Encoding>{string}</Encoding><!-- the default is "UTF-8" -->
 <ExportDocumentProperties>{true/false}</ExportDocumentProperties><!-- the default is 'false' -->
 <ExportFontsAsBase64>{true/false}</ExportFontsAsBase64><!-- the default is 'false' -->
 <ExportFontResources>{true/false}</ExportFontResources><!-- the default is 'false' -->
 <ExportHeadersFootersMode>{FirstSectionHeaderLastSectionFooter/None/PerSection}</ExportHeadersFootersMode><!-- the default is 'PerSection' -->
 <ExportImagesAsBase64>{true/false}</ExportImagesAsBase64><!-- the default is 'false' -->
 <ExportLanguageInformation>{true/false}</ExportLanguageInformation><!-- the default is 'false' -->
 <ExportListLabels>{Auto/AsInlineText/ByHtmlTags}</ExportListLabels><!-- the default is 'Auto' -->
 <ExportMetafileAsRaster>{true/false}</ExportMetafileAsRaster><!-- the default is 'true' -->
 <ExportOriginalUrlForLinkedImages>{true/false}</ExportOriginalUrlForLinkedImages><!-- the default is 'false' -->
 <ExportPageSetup>{true/false}</ExportPageSetup><!-- the default is 'false' -->
 <ExportRelativeFontSize>{true/false}</ExportRelativeFontSize><!-- the default is 'false' -->
 <ExportRoundtripInformation>{true/false}</ExportRoundtripInformation><!-- the default is 'true' -->
 <ExportTextBoxAsSvg>{true/false}</ExportTextBoxAsSvg><!-- the default is 'false' -->
 <ExportTextInputFormFieldAsText>{true/false}</ExportTextInputFormFieldAsText><!-- the default is 'false' -->
 <ExportTocPageNumbers>{true/false}</ExportTocPageNumbers><!-- the default is 'false' -->
 <ExportXhtmlTransitional>{true/false}</ExportXhtmlTransitional><!-- the default is 'false' -->
 <FontResourcesSubsettingSizeThreshold>{number}</FontResourcesSubsettingSizeThreshold><!-- the default is '0' -->
 <HtmlVersion>{Xhtml| Html5}</HtmlVersion><!-- the default is "Xhtml" -->
 <ImageResolution>{number}</ImageResolution><!-- the default is '96' -->
 <OfficeMathOutputMode>{Image/MathML/Text}</OfficeMathOutputMode><!-- the default is 'Image' -->
 <ResourceFolder>{string}</ResourceFolder><!-- the default is an empty string -->
 <ResourceFolderAlias>{string}</ResourceFolderAlias><!-- the default is an empty string -->
 <ScaleImageToShapeSize>{true/false}</ScaleImageToShapeSize><!-- the default is 'true' -->
 <TableWidthOutputMode>{All/None/RelativeOnly}</TableWidthOutputMode><!-- the default is 'All' -->
</MhtmlSaveOptions>
```

## Saving an ODT, OTT

The **OdtSaveOptions** XML definition is presented below:

```XML
<OdtSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <PrettyFormat>{true/false}</PrettyFormat><!-- the default is 'false' -->
   <IsStrictSchema11>{true/false}</IsStrictSchema11><!-- the default is 'false' -->
</OdtSaveOptions>
```

## Saving a PCL

The **PclSaveOptions** XML definition is presented below:

```XML
<PclSaveOptions>
   <SaveFormat>pcl</SaveFormat>
   <FileName>{string}</FileName>
   <JpegQuality>{number}</JpegQuality><!-- the default is '100' -->
   <MetafileRenderingOptions><!-- always present -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'VectorWithFallback' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
  <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
  <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
  <PageCount>{number}</PageCount><!-- the default is Int32.MaxValue -->
  <PageIndex>{number}</PageIndex><!-- the default is '0' -->
  <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
  <FalllbackFontName>{string}</FalllbackFontName>
  <RasterizeTransformedElements>{true/false}</RasterizeTransformedElements><!-- the default is 'true' -->
</PclSaveOptions>
```

## Saving a PDF

The **PdfSaveOptions** XML definition is presented below:

```XML
<PdfSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <Compliance>{Pdf15/PdfA1b}</Compliance><!-- the default is 'Pdf15' -->
   <CreateNoteHyperlinks>{true/false}</CreateNoteHyperlinks><!-- the default is 'false' -->
   <CustomPropertiesExport>{None|Standart|Metadata}</CustomPropertiesExport><!-- the default is 'None' -->
   <DigitalSignatureDetails><!-- the default is 'null' -->
      <Certificate>{certificate_filename}</Certificate><!-- the default is 'null' -->
      <HashAlgorithm>{Md5/Sha1/Sha256/Sha384/Sha512}</HashAlgorithm><!-- the default is 'Sha512' -->
      <Location>{string}</Location><!-- the default is 'null' -->
      <Reason>{string}</Reason><!-- the default is 'null' -->
      <SignatureDate>{date_string}</SignatureDate><!-- the default is current time -->
   </DigitalSignatureDetails>
   <DisplayDocTitle>{true/false}</DisplayDocTitle><!-- the default is 'false' -->
   <DownsampleOptions>
      <DownsampleImages>{true/false}</DownsampleImages><!-- the default is 'true' -->
 	  <Resolution>{number}</Resolution><!-- the default is 220  -->
      <ResolutionThreshold>{number}</ResolutionThreshold><!-- the default is '0' -->
   </DownsampleOptions>
   <EmbedFullFonts>{true/false}</EmbedFullFonts><!-- the default is 'false' -->
   <FontEmbeddingMode>{true/false}</FontEmbeddingMode><!-- the default is 'true' -->
   <EncryptionDetails><!-- the default is 'null' -->
      <EncryptionAlgorithm>{RC4_128/RC4_40}</EncryptionAlgorithm><!-- the default is 'RC4_40' -->
      <OwnerPassword>{string}</OwnerPassword><!-- the default is 'null' -->
      <Permissions>{AllowAll/ContentCopy/ContentCopyForAccessibility/DisallowAll/DocumentAssembly/FillIn/HighResolutionPrinting/ModifyAnnotations/ModifyContents/Printing}</Permissions><!-- the default is 'DisallowAll' -->
      <UserPassword>{string}</UserPassword><!-- the default is 'null' -->
   </EncryptionDetails>
   <CustomPropertiesExport>{true/false}</CustomPropertiesExport><!-- the default is 'false' -->
   <ExportDocumentStructure>{true/false}</ExportDocumentStructure><!-- the default is 'false' -->
   <ImageCompression>{Auto/Jpeg}</ImageCompression><!-- the default is 'Auto' -->
   <JpegQuality>{number}</JpegQuality><!-- the default is '100' -->
   <MetafileRenderingOptions><!-- always present -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'VectorWithFallback' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OpenHyperlinksInNewWindow>{true/false}<OpenHyperlinksInNewWindow><!-- the default is 'false' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <OutlineOptions><!-- always present -->
      <BookmarksOutlineLevels><!-- the default is empty  list, i.e. <BookmarksOutlineLevels/> -->
         <BookmarksOutlineLevel name="{string}">{number}</BookmarksOutlineLevel>

         ...

      </BookmarksOutlineLevels>
      <DefaultBookmarksOutlineLevel>{number}</DefaultBookmarksOutlineLevel><!-- the default is '0' -->
      <ExpandedOutlineLevels>{number}</ExpandedOutlineLevels><!-- the default is '0' -->
      <HeadingsOutlineLevels>{number}</HeadingsOutlineLevels><!-- the default is '0' -->
   </OutlineOptions>
   <PageCount>{number}</PageCount><!-- the default is Int32.MaxValue -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <PageMode>{UseNone/UseOutlines/UseThumbs/FullScreen/UseOC}</PageMode><!-- the default is 'UseOutlines' -->
   <PreserveFormFields>{true/false}</PreserveFormFields><!-- the default is 'false' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <TextCompression>{Flate/None}</TextCompression><!-- the default is 'Flate' -->
   <UseBookFoldPrintingSettings>{true/false}</UseBookFoldPrintingSettings><!-- the default is 'false' -->
   <UseCoreFonts>{true/false}</UseCoreFonts><!-- the default is 'false' -->
   <ZoomBehavior>{None/ZoomFactor/FitPage/FitWidth/FitHeight/FitBox}<ZoomBehavior><!-- the default is 'None' -->
   <ZoomFactor>{number}</ZoomFactor><!-- the default is '0' -->
   <ImageColorSpaceExportMode>{Auto | SimpleCmyk}</ImageColorSpaceExportMode><!-- the default is 'Auto' -->
   <EscapeUri>{true/false}</EscapeUri> <!-- A flag specifying whether URI should be escaped before writing. The default value is 'true' -->
</PdfSaveOptions>
```

## Saving a PNG Image

The **PngSaveOptions** XML definition is presented below:

```XML
 <PngSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- the default is 'false' -->
   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- the default is 'false' -->
   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- the default is 'true' -->
   <ImageBrightness>{float_number}</ImageBrightness><!-- the default is 0.5 -->
   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- the default is 'None' -->
   <ImageContrast>{float_number}</ImageContrast><!-- the default is 0.5 -->
   <GraphicsQualityOptions>
      <CompositingMode>{SourceOver | SourceOver}</CompositingMode><!-- the default is 'null' -->
      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality><!-- the default is 'null' -->
      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- the default is 'null' -->
      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- the default is 'null' -->
      <StringFormat>
        <Alignment>{Center | Far | Near} </Alignment><!-- the default is 'null' -->
        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags><!-- the default is 'null' -->
        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix><!-- the default is 'null' -->
        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming><!-- the default is 'null' -->
        <LineAlignment>{Center | Far | Near}</LineAlignment><!-- the default is 'null' -->
      </StringFormat>
      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- the default is 'null' -->
   </GraphicsQualityOptions>
   <MetafileRenderingOptions><!-- always present -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'Bitmap' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <PaperColor>{color}</PaperColor><!-- the default is 'WHITE' -->
   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- the default is 'Format32BppArgb' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <Resolution>{float_number}</Resolution><!-- the default is '96' -->
   <HorizontalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <VerticalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <Scale>{float_number}</Scale><!-- the default is 1.0 -->
</PngSaveOptions>
```

## Saving a PostScript Document (PS)

The **PsSaveOptions** XML definition is presented below:

```XML
 <PsSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <JpegQuality>{number}</JpegQuality><!-- the default is '95' -->
   <MetafileRenderingOptions><!-- always present -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'VectorWithFallback' -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageCount>{number}</PageCount><!-- the default is Int32.MaxValue -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <UseBookFoldPrintingSettings>{true/false}</UseBookFoldPrintingSettings><!-- the default is 'false' -->
</PsSaveOptions>
```

## Saving an RTF Document

The **RtfSaveOptions** XML definition is presented below:

```XML
<RtfSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <PrettyFormat>{true/false}</PrettyFormat><!-- the default is 'false' -->
   <ExportCompactSize>{true/false}</ExportCompactSize><!-- the default is 'false' -->
   <ExportImagesForOldReaders>{true/false}</ExportImagesForOldReaders><!-- the default is 'true' -->
</RtfSaveOptions> 
```

## Saving an SVG Image

The **SvgSaveOptions** XML definition is presented below:

```XML
 <SvgSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <ExportEmbeddedImages>{true/false}</ExportEmbeddedImages><!-- the default is 'false' -->
   <FitToViewPort>{true/false}</FitToViewPort><!-- the default is 'false' -->
   <JpegQuality>{number}</JpegQuality><!-- the default is '95' -->
   <MetafileRenderingOptions><!-- always present -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'VectorWithFallback' -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageCount>{number}</PageCount><!-- the default is Int32.MaxValue -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <ResourcesFolder>{string}</ResourcesFolder><!-- the default is "" -->
   <ResourcesFolderAlias>{string}</ResourcesFolderAlias><!-- the default is "" -->
   <ShowPageBorder>{true/false}</ShowPageBorder><!-- the default is 'true' -->
   <TextOutputMode>{UsePlacedGlyphs/UseSvgFonts/UseTargetMachineFonts}</TextOutputMode><!-- the default is 'UseTargetMachineFonts' -->
</SvgSaveOptions>
```

## Saving a TIFF Image

The **TiffSaveOptions** XML definition is presented below:

```XML
 <TiffSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- the default is 'false' -->
   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- the default is 'false' -->
   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- the default is 'true' -->
   <ImageBrightness>{float_number}</ImageBrightness><!-- the default is 0.5 -->
   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- the default is 'None' -->
   <ImageContrast>{float_number}</ImageContrast><!-- the default is 0.5 -->
   <GraphicsQualityOptions>
      <CompositingMode>{SourceOver | SourceOver}</CompositingMode><!-- the default is 'null' -->
      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality><!-- the default is 'null' -->
      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- the default is 'null' -->
      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- the default is 'null' -->
      <StringFormat>
        <Alignment>{Center | Far | Near} </Alignment><!-- the default is 'null' -->
        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags><!-- the default is 'null' -->
        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix><!-- the default is 'null' -->
        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming><!-- the default is 'null' -->
        <LineAlignment>{Center | Far | Near}</LineAlignment><!-- the default is 'null' -->
      </StringFormat>
      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- the default is 'null' -->
   </GraphicsQualityOptions>
   <MetafileRenderingOptions><!-- always present -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'Bitmap' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageCount>{number}</PageCount><!-- the default is Int32.MaxValue -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <PaperColor>{color}</PaperColor><!-- the default is 'WHITE' -->
   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- the default is 'Format32BppArgb' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <Resolution>{float_number}</Resolution><!-- the default is '96' -->
   <HorizontalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <VerticalResolution>{float_number}</Resolution><!-- the default is '96' -->
   <Scale>{float_number}</Scale><!-- the default is 1.0 -->
   <TiffBinarizationMethod>{FloydSteinbergDithering/Threshold}</TiffBinarizationMethod><!-- the default is 'Threshold' -->
   <TiffCompression>{Ccitt3/Ccitt4/Lzw/None/Rle}</TiffCompression><!-- the default is 'Lzw' -->
</TiffSaveOptions>
```

## Saving a Plain-Text Document

The **TextSaveOptions** XML definition is presented below:

```XML
<TextSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <Encoding>{string}</Encoding><!-- the default is "UTF-8" -->
   <ForcePageBreaks>{true/false}</ForcePageBreaks"><!-- the default is 'false' -->
   <ParagraphBreak>{string}</ParagraphBreak><!-- the default is "\r\n" -->
   <PreserveTableLayout>{true/false}</PreserveTableLayout><!-- the default is 'false' -->
   <SimplifyListLabels>{true/false}</SimplifyListLabels><!-- the default is 'false' -->
</TextSaveOptions>
```

## Saving a WordML Document

The **WordMLSaveOptions** XML definition is presented below:

```XML
<WordMLSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <PrettyFormat>{true/false}</PrettyFormat><!-- the default is 'false' -->
</WordMLSaveOptions>
```

## Saving a XAML Fixed Document

The **XamlFixedSaveOptions** XML definition is presented below:

```XML
<XamlFixedSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <JpegQuality>{number}</JpegQuality><!-- the default is '95' -->
   <!-- specific part -->
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <PageCount>{number}</PageCount><!-- the default is Int32.MaxValue -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <ResourcesFolder>string</ResourcesFolder>
   <ResourcesFolderAlias>string</ResourcesFolderAlias>
</XamlFixedSaveOptions>
```

## Saving a XAML Flow Document

The **XamlFlowSaveOptions** XML definition is presented below:

```XML
<XamlFlowSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <ImagesFolder>{string}</ImagesFolder><!-- the default is "" -->
   <ImagesFolderAlias>{string}</ImagesFolderAlias><!-- the default is "" -->
</XamlFlowSaveOptions>
```

## Saving a XPS Document (OpenXPS, XPS)

The **XpsSaveOptions** XML definition is presented below:

```XML
<XpsSaveOptions>
   <!-- common part -->
   <SaveFormat>{string}</SaveFormat>
   <FileName>{string}</FileName>
   <!-- specific part -->
   <BookmarksOutlineLevel>{number}</BookmarksOutlineLevel><!-- the default is '0' -->
   <HeadingsOutlineLevels>{number}</HeadingsOutlineLevels><!-- the default is '0' -->
   <JpegQuality>{number}</JpegQuality><!-- the default is '95' -->
   <MetafileRenderingOptions><!-- always present -->
      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- the default is 'VectorWithFallback' -->
      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- the default is 'EmfPlusWithFallback' -->
      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- the default is 'true' -->
   </MetafileRenderingOptions>
   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- the default is 'European' -->
   <OptimizeOutput>{true/false}</OptimizeOutput><!-- the default is 'false' -->
   <OutlineOptions><!-- always present -->
      <BookmarksOutlineLevels><!-- the default is empty  list, i.e. <BookmarksOutlineLevels/> -->
         <BookmarksOutlineLevel name="{string}">{number}</BookmarksOutlineLevel>

         ...

      </BookmarksOutlineLevels>
      <DefaultBookmarksOutlineLevel>{number}</DefaultBookmarksOutlineLevel><!-- the default is '0' -->
      <ExpandedOutlineLevels>{number}</ExpandedOutlineLevels><!-- the default is '0' -->
      <HeadingsOutlineLevels>{number}</HeadingsOutlineLevels><!-- the default is '0' -->
      <CreateMissingOutlineLevels>{true/false}</CreateMissingOutlineLevels> <!-- Gets or sets a value determining whether or not to create missing outline levels when the document is exported. -->
   </OutlineOptions>
   <PageCount>{number}</PageCount><!-- the default is Int32.MaxValue -->
   <PageIndex>{number}</PageIndex><!-- the default is '0' -->
   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- the default is 'Fallback' -->
   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- the default is 'Simplified' -->
   <UseBookFoldPrintingSettings>{true/false}</UseBookFoldPrintingSettings><!-- default is 'false' -->
</XpsSaveOptions>
```

## Color Definition

You can use the following synthax to define colors:

```HTML
{color} = ColorName | (R,G,B)

{ColorName} = known color name, e.g. Black

R,G,B = 0..255
```
