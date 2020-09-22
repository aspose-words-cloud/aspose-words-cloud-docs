---
title: "Convert Document to Destination Format with Detailed Settings and Save Result to Storage"
type: docs
url: /convert-document-to-destination-format-with-detailed-settings-and-save-result-to-storage/
aliases: [/convert-document-to-destination-format-with-detailed-settings-and-save-result-to-storage/]
keywords: "microsoft word document,convert to, word to doc, save word file as pdf,convert word document to html,word doc to html,convert pdf to word,tiff file,Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift"
description: "The API lets you convert word document to HTML, PDF, JPEG, or other formats with detailed settings. The list of supported formats is, BMP, DOC, DOCM, EMF, and more. The Apose.Words Cloud supports, Python, C#, Java, Ruby, PHP, NodeJS, Go, Android, Swift."
weight: 20
---

[PUT /words/{name}/saveAs](https://apireference.aspose.cloud/words/#/Convert/SaveAs) API lets you convert *Microsoft Word document* to another format with details settings. The list of supported formats are:

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
The important parameters of this API are:

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

## Save Options

All elements, except **SaveFormat** and **FileName**, can be omitted. If we omit an element, then the element will contain default value (default values for elements you can see in a comment after the corresponding element).

- **Request for saving images BMP:**

**BmpSaveOptions**

```html

<BmpSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <ColorMode>{Normal | Grayscale }</ColorMode><!-- default value = Normal -->

   <!-- specific part -->

   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- default value = false -->

   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- default value = false -->

   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- default value = true-->

   <ImageBrightness>{float_number}</ImageBrightness><!-- default value = 0.5 -->

   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- default value = None -->

   <ImageContrast>{float_number}</ImageContrast><!-- default value = 0.5 -->

   <GraphicsQualityOptions>

      <CompositingMode>{SourceOver | SourceOver}</CompositingMode> <!-- default value = null-->

      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality> <!-- default value = null-->

      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- default value = null-->

      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- default value = null-->

      <StringFormat>

        <Alignment>{Center | Far | Near} </Alignment> <!-- default value = null -->

        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags> <!-- default value = null -->

        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix> <!-- default value = null -->

        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming> <!-- default value = null -->

        <LineAlignment>{Center | Far | Near}</LineAlignment> <!-- default value = null -->

      </StringFormat>

      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- default value = null-->

   </GraphicsQualityOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <MetafileRenderingOptions><!-- always present -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = Bitmap -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

      <EmulateRasterOperations>{true/false}</EmulateRasterOperations> <!-- Gets or sets a value determining whether or not the raster operations should be emulated. -->     

   </MetafileRenderingOptions>

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <PaperColor>{color}</PaperColor><!-- default value = WHITE -->

   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- default value = Format32BppArgb -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <Resolution>{float_number}</Resolution><!-- default value = 96 -->

   <HorizontalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <VerticalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <Scale>{float_number}</Scale><!-- default value = 1.0 -->

</BmpSaveOptions>

```

- **Request for saving** **a document (DOC, DOT):**

**DocSaveOptions**

```html

<DocSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <Password>{string}</Password><!-- default value = "" -->

   <SaveRoutingSlip>{true/false}</SaveRoutingSlip><!-- default value = true -->

</DocSaveOptions>

```

- **Request for saving OOXML (DOCX, DOCM, DOTX, DOTM, FLATOPC):**

**OoxmlSaveOptions**

```html

<OoxmlSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <PrettyFormat>{true/false}</PrettyFormat><!-- default value = false -->

   <Compliance>{Ecma376_2006/Iso29500_2008_Transitional}</Compliance><!-- default value = Ecma376_2006 -->

   <Password>{string}</Password><!-- default value = "" -->

</OoxmlSaveOptions>

```

- **Request for saving EMF:**

**EmfSaveOptions**

```html

<EmfSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <ImageBrightness>{float_number}</ImageBrightness><!-- default value = 0.5 -->

   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- default value = None -->

   <ImageContrast>{float_number}</ImageContrast><!-- default value = 0.5 -->

   <GraphicsQualityOptions>

      <CompositingMode>{SourceOver | SourceOver}</CompositingMode> <!-- default value = null-->

      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality> <!-- default value = null-->

      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- default value = null-->

      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- default value = null-->

      <StringFormat>

        <Alignment>{Center | Far | Near} </Alignment> <!-- default value = null -->

        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags> <!-- default value = null -->

        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix> <!-- default value = null -->

        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming> <!-- default value = null -->

        <LineAlignment>{Center | Far | Near}</LineAlignment> <!-- default value = null -->

      </StringFormat>

      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- default value = null-->

   </GraphicsQualityOptions>

   <MetafileRenderingOptions><!-- always present -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = Bitmap -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <PaperColor>{color}</PaperColor><!-- default value = WHITE -->

   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- default value = Format32BppArgb -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <Resolution>{float_number}</Resolution><!-- default value = 96 -->

   <HorizontalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <VerticalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <Scale>{float_number}</Scale><!-- defaulHtmlSaveOptionst value = 1.0 -->

   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- default value = true-->

</EmfSaveOptions>

```

- **Request for saving EPUB:**

**EpubSaveOptions**

```html

<EpubSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <PrettyFormat>{true/false}</PrettyFormat><!-- default value = false -->

   <AllowNegativeIndent>{true/false}</AllowNegativeIndent><!-- default value = false -->

   <CssStyleSheetType>{Embedded/External/Inline}</CssStyleSheetType><!-- default value = External -->

   <DocumentSplitCriteria>{ColumnBreak/HeadingParagraph/None/PageBreak/SectionBreak}</DocumentSplitCriteria><!-- default value = HeadingParagraph -->

   <DocumentSplitHeadingLevel>{number}</DocumentSplitHeadingLevel><!-- default value = 2 -->

   <Encoding>{string}</Encoding><!-- default value = "UTF-8" -->

   <EpubNavigationMapLevel>{number}</EpubNavigationMapLevel><!-- default value = 3 -->

   <ExportDocumentProperties>{true/false}</ExportDocumentProperties><!-- default value = false -->

   <ExportFontsAsBase64>{true/false}</ExportFontsAsBase64><!-- default value = false -->

   <ExportFontResources>{true/false}</ExportFontResources><!-- default value = false -->

   <ExportHeadersFootersMode>{FirstSectionHeaderLastSectionFooter/None/PerSection}</ExportHeadersFootersMode><!-- default value = None -->

   <ExportImagesAsBase64>{true/false}</ExportImagesAsBase64><!-- default value = false -->

   <ExportLanguageInformation>{true/false}</ExportLanguageInformation><!-- default value = false -->

   <ExportListLabels>{Auto/AsInlineText/ByHtmlTags}</ExportListLabels><!-- default value = Auto -->

   <ExportMetafileAsRaster>{true/false}</ExportMetafileAsRaster><!-- default value = true -->

   <ExportOriginalUrlForLinkedImages>{true/false}</ExportOriginalUrlForLinkedImages><!-- default value = false-->

   <ExportPageSetup>{true/false}</ExportPageSetup><!-- default value = false -->

   <ExportRelativeFontSize>{true/false}</ExportRelativeFontSize><!-- default value = false -->

   <ExportRoundtripInformation>{true/false}</ExportRoundtripInformation><!-- default value = true -->

   <ExportTextBoxAsSvg>{true/false}</ExportTextBoxAsSvg><!-- default value = false -->

   <ExportTextInputFormFieldAsText>{true/false}</ExportTextInputFormFieldAsText><!-- default value = false -->

   <ExportTocPageNumbers>{true/false}</ExportTocPageNumbers><!-- default value = false -->

   <FontResourcesSubsettingSizeThreshold>{number}</FontResourcesSubsettingSizeThreshold><!-- default value = 0 -->

   <HtmlVersion>{Xhtml| Html5}</HtmlVersion><!-- default value = "Xhtml" -->

   <ImageResolution>{number}</ImageResolution><!-- default value = 96 -->

   <OfficeMathOutputMode>{Image/MathML/Text}</OfficeMathOutputMode><!-- default value = Image -->

   <ResourceFolder>{string}</ResourceFolder><!-- default is an empty string -->

   <ResourceFolderAlias>{string}</ResourceFolderAlias><!-- default is an empty string -->

   <ScaleImageToShapeSize>{true/false}</ScaleImageToShapeSize><!-- default value = true -->

   <TableWidthOutputMode>{All/None/RelativeOnly}</TableWidthOutputMode><!-- default value = All -->

</EpubSaveOptions>

```

- **Request for saving GIF:**

**GifSaveOptions**

```html

<GifSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <ColorMode>{Normal | Grayscale }</ColorMode><!-- default value = Normal -->

   <!-- specific part -->

   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- default value = false -->

   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- default value = false -->

   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- default value = true-->

   <ImageBrightness>{float_number}</ImageBrightness><!-- default value = 0.5 -->

   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- default value = None -->

   <ImageContrast>{float_number}</ImageContrast><!-- default value = 0.5 -->

   <GraphicsQualityOptions>

      <CompositingMode>{SourceOver | SourceOver}</CompositingMode> <!-- default value = null-->

      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality> <!-- default value = null-->

      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- default value = null-->

      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- default value = null-->

      <StringFormat>

        <Alignment>{Center | Far | Near} </Alignment> <!-- default value = null -->

        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags> <!-- default value = null -->

        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix> <!-- default value = null -->

        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming> <!-- default value = null -->

        <LineAlignment>{Center | Far | Near}</LineAlignment> <!-- default value = null -->

      </StringFormat>

      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- default value = null-->

   </GraphicsQualityOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <MetafileRenderingOptions><!-- always present -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = Bitmap -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

      <ScaleWmfFontsToMetafileSize>{true/false}</ScaleWmfFontsToMetafileSize> <!-- Gets or sets a value determining whether or not to scale fonts in WMF metafile according to metafile size on the page. -->

   </MetafileRenderingOptions>

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <PaperColor>{color}</PaperColor><!-- default value = WHITE -->

   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- default value = Format32BppArgb -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <Resolution>{float_number}</Resolution><!-- default value = 96 -->

   <HorizontalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <VerticalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <Scale>{float_number}</Scale><!-- default value = 1.0 -->

</GifSaveOptions>

```

- **Request for saving HTML:**

**HtmlSaveOptions**

```html

<HtmlSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <PrettyFormat>{true/false}</PrettyFormat><!-- default value = false -->

   <AllowNegativeIndent>{true/false}</AllowNegativeIndent><!-- default value = false -->

   <CssStyleSheetFileName>{string}</CssStyleSheetFileName><!-- default value = "" -->

   <CssStyleSheetType>{Embedded/External/Inline}</CssStyleSheetType><!-- default value = Inline -->

   <DocumentSplitCriteria>{ColumnBreak/HeadingParagraph/None/PageBreak/SectionBreak}</DocumentSplitCriteria><!-- default value = None -->

   <DocumentSplitHeadingLevel>{number}</DocumentSplitHeadingLevel><!-- default value = 2 -->

   <Encoding>{string}</Encoding><!-- default value = "UTF-8" -->

   <ExportDocumentProperties>{true/false}</ExportDocumentProperties><!-- default value = false -->

   <ExportFontsAsBase64>{true/false}</ExportFontsAsBase64><!-- default value = false -->

   <ExportFontResources>{true/false}</ExportFontResources><!-- default value = false -->

   <ExportHeadersFootersMode>{FirstSectionHeaderLastSectionFooter/None/PerSection}</ExportHeadersFootersMode><!-- default value = PerSection -->

   <ExportImagesAsBase64>{true/false}</ExportImagesAsBase64><!-- default value = false -->

   <ExportLanguageInformation>{true/false}</ExportLanguageInformation><!-- default value = false -->

   <ExportListLabels>{Auto/AsInlineText/ByHtmlTags}</ExportListLabels><!-- default value = Auto -->

   <ExportMetafileAsRaster>{true/false}</ExportMetafileAsRaster><!-- default value = true -->

   <ExportOriginalUrlForLinkedImages>{true/false}</ExportOriginalUrlForLinkedImages><!-- default value = false-->

   <ExportPageSetup>{true/false}</ExportPageSetup><!-- default value = false -->

   <ExportPageMargins>{true/false}</ExportPageMargins><!-- default value = false -->

   <ExportRelativeFontSize>{true/false}</ExportRelativeFontSize><!-- default value = false -->

   <ExportRoundtripInformation>{true/false}</ExportRoundtripInformation><!-- default value = true -->

   <ExportTextBoxAsSvg>{true/false}</ExportTextBoxAsSvg><!-- default value = false -->

   <ExportTextInputFormFieldAsText>{true/false}</ExportTextInputFormFieldAsText><!-- default value = false -->

   <ExportTocPageNumbers>{true/false}</ExportTocPageNumbers><!-- default value = false -->

   <ExportXhtmlTransitional>{true/false}</ExportXhtmlTransitional><!-- default value = false -->

   <FontResourcesSubsettingSizeThreshold>{number}</FontResourcesSubsettingSizeThreshold><!-- default value = 0 -->

   <FontsFolder>{string}</FontsFolder><!-- default value = "" -->

   <FontsFolderAlias>{string}</FontsFolderAlias><!-- default value = "" -->

   <HtmlVersion>{Xhtml| Html5}</HtmlVersion><!-- default value = "Xhtml" -->

   <ImageResolution>{number}</ImageResolution><!-- default value = 96 -->

   <ImagesFolder>{string}</ImagesFolder><!-- default value = "" -->

   <ImagesFolderAlias>{string}</ImagesFolderAlias><!-- default value = "" -->

   <OfficeMathOutputMode>{Image/MathML/Text}</OfficeMathOutputMode><!-- default value = Image -->

   <ResourceFolder>{string}</ResourceFolder><!-- default is an empty string -->

   <ResourceFolderAlias>{string}</ResourceFolderAlias><!-- default is an empty string -->

   <ScaleImageToShapeSize>{true/false}</ScaleImageToShapeSize><!-- default value = true -->

   <TableWidthOutputMode>{All/None/RelativeOnly}</TableWidthOutputMode><!-- default value = All -->

   <ExportDropDownFormFieldAsText>{true/false}</ExportDropDownFormFieldAsText><!-- default value = false -->

   <ResolveFontNames>{true/false}</ResolveFontNames> <!-- Specifies whether font family names used in the document are resolved and substituted according to FontSettings when being written into HTML-based formats. -->

</HtmlSaveOptions>

```

- **Request for saving fixed HTML:**

**HtmlFixedSaveOptions**

```html

<HtmlFixedSaveOptions>

   <!-- common part -->

   <CssClassNamesPrefix>{string}</CssClassNamesPrefix><!-- default value = aw -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <ExportEmbeddedCss>{true/false}</ExportEmbeddedCss><!-- default value = false -->

   <ExportEmbeddedFonts>{true/false}</ExportEmbeddedFonts><!-- default value = false -->

   <ExportEmbeddedImages>{true/false}</ExportEmbeddedImages><!-- default value = false -->

   <ExportFormFields>{true/false}</ExportFormFields><!-- default value = false -->

   <Encoding>ASCII</Encoding><!-- default value = UTF8 -->

   <FontFormat>{Tft/Woff}</FontFormat><!-- default value = Woff -->

   <JpegQuality>{number}</JpegQuality><!-- default value = 95 -->

   <MetafileRenderingOptions><!-- always present -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = VectorWithFallback -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageCount>{number}</PageCount><!-- default value = Int32.MaxValue -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <PageHorizontalAlignment>{Left/Center/Right}</PageHorizontalAlignment><!-- default value = "Center" -->

   <PageMargins>{double}</PageMargins><!-- default value = 10 -->

   <ResourcesFolder>{string}</ResourcesFolder><!-- default value = "" -->

   <ResourcesFolderAlias>{string}</ResourcesFolderAlias><!-- default value = "" -->

   <ShowPageBorder>{true/false}</ShowPageBorder><!-- default value = true -->

</HtmlFixedSaveOptions>

```

- **Request for saving images JPEG:**

**JpegSaveOptions**

```html

<JpegSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- default value = false -->

   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- default value = false -->

   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- default value = true-->

   <ImageBrightness>{float_number}</ImageBrightness><!-- default value = 0.5 -->

   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- default value = None -->

   <ImageContrast>{float_number}</ImageContrast><!-- default value = 0.5 -->

   <GraphicsQualityOptions>

      <CompositingMode>{SourceOver | SourceOver}</CompositingMode> <!-- default value = null-->

      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality> <!-- default value = null-->

      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- default value = null-->

      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- default value = null-->

      <StringFormat>

        <Alignment>{Center | Far | Near} </Alignment> <!-- default value = null -->

        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags> <!-- default value = null -->

        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix> <!-- default value = null -->

        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming> <!-- default value = null -->

        <LineAlignment>{Center | Far | Near}</LineAlignment> <!-- default value = null -->

      </StringFormat>

      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- default value = null-->

   </GraphicsQualityOptions>

   <JpegQuality>{number}</JpegQuality><!-- default value = 95 -->

   <MetafileRenderingOptions><!-- always present -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = Bitmap -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <PaperColor>{color}</PaperColor><!-- default value = WHITE -->

   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- default value = Format32BppArgb -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <Resolution>{float_number}</Resolution><!-- default value = 96 -->

   <HorizontalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <VerticalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <Scale>{float_number}</Scale><!-- default value = 1.0 -->

</JpegSaveOptions>

```

- **Request for saving MHTML:**

**MhtmlSaveOptions**

```html

<MhtmlSaveOptions>

 <!-- common part -->

 <SaveFormat>{string}</SaveFormat>

 <FileName>{string}</FileName>

 <!-- specific part -->

 <PrettyFormat>{true/false}</PrettyFormat><!-- default value = false -->

 <AllowNegativeIndent>{true/false}</AllowNegativeIndent><!-- default value = false -->

 <CssStyleSheetType>{Embedded/External/Inline}</CssStyleSheetType><!-- default value = Inline -->

 <Encoding>{string}</Encoding><!-- default value = "UTF-8" -->

 <ExportDocumentProperties>{true/false}</ExportDocumentProperties><!-- default value = false -->

 <ExportFontsAsBase64>{true/false}</ExportFontsAsBase64><!-- default value = false -->

 <ExportFontResources>{true/false}</ExportFontResources><!-- default value = false -->

 <ExportHeadersFootersMode>{FirstSectionHeaderLastSectionFooter/None/PerSection}</ExportHeadersFootersMode><!-- default value = PerSection -->

 <ExportImagesAsBase64>{true/false}</ExportImagesAsBase64><!-- default value = false -->

 <ExportLanguageInformation>{true/false}</ExportLanguageInformation><!-- default value = false -->

 <ExportListLabels>{Auto/AsInlineText/ByHtmlTags}</ExportListLabels><!-- default value = Auto -->

 <ExportMetafileAsRaster>{true/false}</ExportMetafileAsRaster><!-- default value = true -->

 <ExportOriginalUrlForLinkedImages>{true/false}</ExportOriginalUrlForLinkedImages><!-- default value = false-->

 <ExportPageSetup>{true/false}</ExportPageSetup><!-- default value = false -->

 <ExportRelativeFontSize>{true/false}</ExportRelativeFontSize><!-- default value = false -->

 <ExportRoundtripInformation>{true/false}</ExportRoundtripInformation><!-- default value = true -->

 <ExportTextBoxAsSvg>{true/false}</ExportTextBoxAsSvg><!-- default value = false -->

 <ExportTextInputFormFieldAsText>{true/false}</ExportTextInputFormFieldAsText><!-- default value = false -->

 <ExportTocPageNumbers>{true/false}</ExportTocPageNumbers><!-- default value = false -->

 <ExportXhtmlTransitional>{true/false}</ExportXhtmlTransitional><!-- default value = false -->

 <FontResourcesSubsettingSizeThreshold>{number}</FontResourcesSubsettingSizeThreshold><!-- default value = 0 -->

 <HtmlVersion>{Xhtml| Html5}</HtmlVersion><!-- default value = "Xhtml" -->

 <ImageResolution>{number}</ImageResolution><!-- default value = 96 -->

 <OfficeMathOutputMode>{Image/MathML/Text}</OfficeMathOutputMode><!-- default value = Image -->

 <ResourceFolder>{string}</ResourceFolder><!-- default is an empty string -->

 <ResourceFolderAlias>{string}</ResourceFolderAlias><!-- default is an empty string -->

 <ScaleImageToShapeSize>{true/false}</ScaleImageToShapeSize><!-- default value = true -->

 <TableWidthOutputMode>{All/None/RelativeOnly}</TableWidthOutputMode><!-- default value = All -->

</MhtmlSaveOptions>

```

- **Request for saving ODT, OTT:**

**OdtSaveOptions**

```html

<OdtSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <PrettyFormat>{true/false}</PrettyFormat><!-- default value = false -->

   <IsStrictSchema11>{true/false}</IsStrictSchema11><!-- default value = false -->

</OdtSaveOptions>

```

- **Request for saving PCL:**

**PclSaveOptions**

```html

<PclSaveOptions>

   <SaveFormat>pcl</SaveFormat>

   <FileName>{string}</FileName>

   <JpegQuality>{number}</JpegQuality><!-- default value = 100 -->

   <MetafileRenderingOptions><!-- always present -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = VectorWithFallback -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

  <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

  <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

  <PageCount>{number}</PageCount><!-- default value = Int32.MaxValue -->

  <PageIndex>{number}</PageIndex><!-- default value = 0 -->

  <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

  <FalllbackFontName>{string}</FalllbackFontName>

  <RasterizeTransformedElements>{true/false}</RasterizeTransformedElements><!-- default value = true -->

</PclSaveOptions>

```

- **Request for saving PDF:**

**PdfSaveOptions**

```html

<PdfSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <Compliance>{Pdf15/PdfA1b}</Compliance><!-- default value = Pdf15 -->

   <CreateNoteHyperlinks>{true/false}</CreateNoteHyperlinks><!-- default value = false -->

   <CustomPropertiesExport>{None|Standart|Metadata}</CustomPropertiesExport><!-- default value = None-->

   <DigitalSignatureDetails><!-- default value = null -->

      <Certificate>{certificate_filename}</Certificate><!-- default value = null -->

      <HashAlgorithm>{Md5/Sha1/Sha256/Sha384/Sha512}</HashAlgorithm><!-- default value = Sha512 -->

      <Location>{string}</Location><!-- default value = null -->

      <Reason>{string}</Reason><!-- default value = null -->

      <SignatureDate>{date_string}</SignatureDate><!-- default value = current time -->

   </DigitalSignatureDetails>

   <DisplayDocTitle>{true/false}</DisplayDocTitle> <!-- default value = false. -->

   <DownsampleOptions>

      <DownsampleImages>{true/false}</DownsampleImages><!-- default value = true -->

 	  <Resolution>{number}</Resolution><!-- default value is 220  -->

      <ResolutionThreshold>{number}</ResolutionThreshold><!-- default value is 0 -->

   </DownsampleOptions>

   <EmbedFullFonts>{true/false}</EmbedFullFonts><!-- default value = false -->

   <FontEmbeddingMode>{true/false}</FontEmbeddingMode><!-- default value = true -->

   <EncryptionDetails><!-- default value = null -->

      <EncryptionAlgorithm>{RC4_128/RC4_40}</EncryptionAlgorithm><!-- default value = RC4_40 -->

      <OwnerPassword>{string}</OwnerPassword><!-- default value = null -->

      <Permissions>{AllowAll/ContentCopy/ContentCopyForAccessibility/DisallowAll/DocumentAssembly/FillIn/HighResolutionPrinting/ModifyAnnotations/ModifyContents/Printing}</Permissions><!-- default value = DisallowAll -->

      <UserPassword>{string}</UserPassword><!-- default value = null -->

   </EncryptionDetails>

   <CustomPropertiesExport>{true/false}</CustomPropertiesExport><!-- default value = false -->

   <ExportDocumentStructure>{true/false}</ExportDocumentStructure><!-- default value = false -->

   <ImageCompression>{Auto/Jpeg}</ImageCompression> <!-- default value = Auto -->

   <JpegQuality>{number}</JpegQuality><!-- default value = 100 -->

   <MetafileRenderingOptions><!-- always present -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = VectorWithFallback -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OpenHyperlinksInNewWindow>{true/false}<OpenHyperlinksInNewWindow><!-- default value = false -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <OutlineOptions><!-- always present -->

      <BookmarksOutlineLevels><!-- default value = empty  list, i.e. <BookmarksOutlineLevels/> -->

         <BookmarksOutlineLevel name="{string}">{number}</BookmarksOutlineLevel>

         ...

      </BookmarksOutlineLevels>

      <DefaultBookmarksOutlineLevel>{number}</DefaultBookmarksOutlineLevel><!-- default value = 0 -->

      <ExpandedOutlineLevels>{number}</ExpandedOutlineLevels><!-- default value = 0 -->

      <HeadingsOutlineLevels>{number}</HeadingsOutlineLevels><!-- default value = 0 -->

   </OutlineOptions>

   <PageCount>{number}</PageCount><!-- default value = Int32.MaxValue -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <PageMode>{UseNone/UseOutlines/UseThumbs/FullScreen/UseOC}</PageMode><!-- default value = UseOutlines -->

   <PreserveFormFields>{true/false}</PreserveFormFields><!-- default value = false -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <TextCompression>{Flate/None}</TextCompression><!-- default value = Flate -->

   <UseBookFoldPrintingSettings>{true/false}</UseBookFoldPrintingSettings><!-- default value = false -->

   <UseCoreFonts>{true/false}</UseCoreFonts><!-- default value = false -->

   <ZoomBehavior>{None/ZoomFactor/FitPage/FitWidth/FitHeight/FitBox}<ZoomBehavior><!-- default value = None -->

   <ZoomFactor>{number}</ZoomFactor><!-- default value = 0 -->

   <ImageColorSpaceExportMode>{Auto | SimpleCmyk}</ImageColorSpaceExportMode><!-- default value = Auto -->

   <EscapeUri>{true/false}</EscapeUri> <!-- A flag specifying whether URI should be escaped before writing. The default value is true. -->

</PdfSaveOptions>

```

- **Request for saving images PNG:**

**PngSaveOptions**

```html

 <PngSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- default value = false -->

   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- default value = false -->

   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- default value = true-->

   <ImageBrightness>{float_number}</ImageBrightness><!-- default value = 0.5 -->

   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- default value = None -->

   <ImageContrast>{float_number}</ImageContrast><!-- default value = 0.5 -->

   <GraphicsQualityOptions>

      <CompositingMode>{SourceOver | SourceOver}</CompositingMode> <!-- default value = null-->

      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality> <!-- default value = null-->

      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- default value = null-->

      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- default value = null-->

      <StringFormat>

        <Alignment>{Center | Far | Near} </Alignment> <!-- default value = null -->

        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags> <!-- default value = null -->

        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix> <!-- default value = null -->

        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming> <!-- default value = null -->

        <LineAlignment>{Center | Far | Near}</LineAlignment> <!-- default value = null -->

      </StringFormat>

      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- default value = null-->

   </GraphicsQualityOptions>

   <MetafileRenderingOptions><!-- always present -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = Bitmap -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <PaperColor>{color}</PaperColor><!-- default value = WHITE -->

   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- default value = Format32BppArgb -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <Resolution>{float_number}</Resolution><!-- default value = 96 -->

   <HorizontalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <VerticalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <Scale>{float_number}</Scale><!-- default value = 1.0 -->

</PngSaveOptions>

```

- **Request for saving PS:**

**PsSaveOptions**

```html

 <PsSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <JpegQuality>{number}</JpegQuality><!-- default value = 95 -->

   <MetafileRenderingOptions><!-- always present -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = VectorWithFallback -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageCount>{number}</PageCount><!-- default value = Int32.MaxValue -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <UseBookFoldPrintingSettings>{true/false}</UseBookFoldPrintingSettings><!-- default value = false -->

</PsSaveOptions>

```

- **Request for saving RTF:**

**RtfSaveOptions**

```html

<RtfSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <PrettyFormat>{true/false}</PrettyFormat><!-- default value = false -->

   <ExportCompactSize>{true/false}</ExportCompactSize><!-- default value = false -->

   <ExportImagesForOldReaders>{true/false}</ExportImagesForOldReaders><!-- default value = true -->

</RtfSaveOptions> 

```

- **Request for saving SVG:**

**SvgSaveOptions**

```html

 <SvgSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <ExportEmbeddedImages>{true/false}</ExportEmbeddedImages><!-- default value = false -->

   <FitToViewPort>{true/false}</FitToViewPort><!-- default value = false -->

   <JpegQuality>{number}</JpegQuality><!-- default value = 95 -->

   <MetafileRenderingOptions><!-- always present -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = VectorWithFallback -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageCount>{number}</PageCount><!-- default value = Int32.MaxValue -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <ResourcesFolder>{string}</ResourcesFolder><!-- default value = "" -->

   <ResourcesFolderAlias>{string}</ResourcesFolderAlias><!-- default value = "" -->

   <ShowPageBorder>{true/false}</ShowPageBorder><!-- default value = true -->

   <TextOutputMode>{UsePlacedGlyphs/UseSvgFonts/UseTargetMachineFonts}</TextOutputMode><!-- default value = UseTargetMachineFonts -->

</SvgSaveOptions>

```

- **Request for saving TIFF:**

**TiffSaveOptions**

```html

 <TiffSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <UseAntiAliasing>{true/false}</UseAntiAliasing><!-- default value = false -->

   <UseHighQualityRendering>{true/false}</UseHighQualityRendering><!-- default value = false -->

   <UseGdiEmfRenderer>{true/false}</UseGdiEmfRenderer><!-- default value = true-->

   <ImageBrightness>{float_number}</ImageBrightness><!-- default value = 0.5 -->

   <ImageColorMode>{BlackAndWhite/Grayscale/None}</ImageColorMode><!-- default value = None -->

   <ImageContrast>{float_number}</ImageContrast><!-- default value = 0.5 -->

   <GraphicsQualityOptions>

      <CompositingMode>{SourceOver | SourceOver}</CompositingMode> <!-- default value = null-->

      <CompositingQuality>{Default | HighSpeed | HighQuality | GammaCorrected | AssumeLinear}</CompositingQuality> <!-- default value = null-->

      <InterpolationMode>{Default | Low | High | Bilinear | Bicubic | NearestNeighbor | HighQualityBilinear | HighQualityBicubic }</InterpolationMode><!-- default value = null-->

      <SmoothingMode>{Default | HighSpeed | HighQuality | None | AntiAlias }</SmoothingMode><!-- default value = null-->

      <StringFormat>

        <Alignment>{Center | Far | Near} </Alignment> <!-- default value = null -->

        <FormatFlags>{DirectionRightToLeft | DirectionVertical | DisplayFormatControl | FitBlackBox | LineLimit | MeasureTrailingSpaces | NoClip | NoFontFallback | NoWrap}</FormatFlags> <!-- default value = null -->

        <HotkeyPrefix>{ Hide | None | Show } </HotkeyPrefix> <!-- default value = null -->

        <Trimming>{ Character | EllipsisCharacter | EllipsisPath | EllipsisWord | None | Word }</Trimming> <!-- default value = null -->

        <LineAlignment>{Center | Far | Near}</LineAlignment> <!-- default value = null -->

      </StringFormat>

      <TextRenderingHint>{SystemDefault | SingleBitPerPixelGridFit | SingleBitPerPixel | AntiAliasGridFit | AntiAlias |ClearTypeGridFit}</TextRenderingHint><!-- default value = null-->

   </GraphicsQualityOptions>

   <MetafileRenderingOptions><!-- always present -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = Bitmap -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageCount>{number}</PageCount><!-- default value = Int32.MaxValue -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <PaperColor>{color}</PaperColor><!-- default value = WHITE -->

   <PixelFormat>{Format16BppArgb1555/Format16BppRgb555/Format16BppRgb565/Format24BppRgb/Format32BppArgb/Format32BppPArgb/Format32BppRgb/Format48BppRgb/Format64BppArgb/Format64BppPArgb}</PixelFormat><!-- default value = Format32BppArgb -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <Resolution>{float_number}</Resolution><!-- default value = 96 -->

   <HorizontalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <VerticalResolution>{float_number}</Resolution><!-- default value = 96 -->

   <Scale>{float_number}</Scale><!-- default value = 1.0 -->

   <TiffBinarizationMethod>{FloydSteinbergDithering/Threshold}</TiffBinarizationMethod><!-- default value = Threshold -->

   <TiffCompression>{Ccitt3/Ccitt4/Lzw/None/Rle}</TiffCompression><!-- default value = Lzw -->

</TiffSaveOptions>

```

- **Request for saving TXT:**

**TextSaveOptions**

```html

<TextSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <Encoding>{string}</Encoding><!-- default value = "UTF-8" -->

   <ForcePageBreaks>{true/false}</ForcePageBreaks"><!-- default value = false -->

   <ParagraphBreak>{string}</ParagraphBreak><!-- default value = "\r\n" -->

   <PreserveTableLayout>{true/false}</PreserveTableLayout><!-- default value = false -->

   <SimplifyListLabels>{true/false}</SimplifyListLabels><!-- default value = false -->

</TextSaveOptions>

```

- **Request for saving WORDML:**

**WordMLSaveOptions**

```html

<WordMLSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <PrettyFormat>{true/false}</PrettyFormat><!-- default value = false -->

</WordMLSaveOptions>

```

- **Request for saving XAMLFIXED:**

**XamlFixedSaveOptions**

```html

<XamlFixedSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <JpegQuality>{number}</JpegQuality><!-- default value = 95 -->

   <!-- specific part -->

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <PageCount>{number}</PageCount><!-- default value = Int32.MaxValue -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <ResourcesFolder>string</ResourcesFolder>

   <ResourcesFolderAlias>string</ResourcesFolderAlias>

</XamlFixedSaveOptions>

```

- **Request for saving XAMLFLOW:**

**XamlFlowSaveOptions**

```html

<XamlFlowSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <ImagesFolder>{string}</ImagesFolder><!-- default value = "" -->

   <ImagesFolderAlias>{string}</ImagesFolderAlias><!-- default value = "" -->

</XamlFlowSaveOptions>

```

- **Request for saving XPS (OpenXPS, XPS):**

**XpsSaveOptions**

```html

<XpsSaveOptions>

   <!-- common part -->

   <SaveFormat>{string}</SaveFormat>

   <FileName>{string}</FileName>

   <!-- specific part -->

   <BookmarksOutlineLevel>{number}</BookmarksOutlineLevel><!-- default value = 0 -->

   <HeadingsOutlineLevels>{number}</HeadingsOutlineLevels><!-- default value = 0 -->

   <JpegQuality>{number}</JpegQuality><!-- default value = 95 -->

   <MetafileRenderingOptions><!-- always present -->

      <RenderingMode>{VectorWithFallback/Vector/Bitmap}<RenderingMode><!-- default value = VectorWithFallback -->

      <EmfPlusDualRenderingMode>{EmfPlusWithFallback/EmfPlus/Emf}<EmfPlusDualRenderingMode><!-- default value = EmfPlusWithFallback -->

      <UseEmfEmbeddedToWmf>{true/false}</UseEmfEmbeddedToWmf><!-- default value = true -->

   </MetafileRenderingOptions>

   <NumeralFormat>{European/ArabicIndic/EasternArabicIndic/Context/System}</NumeralFormat><!-- default value = European -->

   <OptimizeOutput>{true/false}</OptimizeOutput><!-- default value = false -->

   <OutlineOptions><!-- always present -->

      <BookmarksOutlineLevels><!-- default value = empty  list, i.e. <BookmarksOutlineLevels/> -->

         <BookmarksOutlineLevel name="{string}">{number}</BookmarksOutlineLevel>

         ...

      </BookmarksOutlineLevels>

      <DefaultBookmarksOutlineLevel>{number}</DefaultBookmarksOutlineLevel><!-- default value = 0 -->

      <ExpandedOutlineLevels>{number}</ExpandedOutlineLevels><!-- default value = 0 -->

      <HeadingsOutlineLevels>{number}</HeadingsOutlineLevels><!-- default value = 0 -->

      <CreateMissingOutlineLevels>{true/false}</CreateMissingOutlineLevels> <!-- Gets or sets a value determining whether or not to create missing outline levels when the document is exported. -->

   </OutlineOptions>

   <PageCount>{number}</PageCount><!-- default value = Int32.MaxValue -->

   <PageIndex>{number}</PageIndex><!-- default value = 0 -->

   <DmlRenderingMode>{Fallback | DrawingML}</DmlRenderingMode><!-- default value = Fallback -->

   <DmlEffectsRenderingMode>{Simplified | None | Fine}</DmlEffectsRenderingMode><!-- default value = Simplified -->

   <UseBookFoldPrintingSettings>{true/false}</UseBookFoldPrintingSettings><!-- default value = false -->

</XpsSaveOptions>

```

**Type definition:**

**Type definition**

```html

{color} = ColorName | (R,G,B)

{ColorName} = known color name, e.g. Black

R,G,B = 0..255

```

## Resource URI

[Swagger UI](https://apireference.aspose.cloud/words/#/Convert/SaveAs) lets you call this REST API directly from the browser. The description of the API and its parameters is also given there.

## cURL Example

{{< tabs tabTotal="2" tabID="25" tabName1="Request" tabName2="Response" >}}
{{< tab tabNum="1" >}}
```java
// Please get your App_Key and App_SID credentials from https://dashboard.aspose.cloud/#/apps.
// Place App_Key in "client_secret" and App_SID in "client_id" argument.

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

// cURL example to convert MS Word Document to PDF using PDFSaveOptions

curl -v "https://api.aspose.cloud/v4.0/words/test_multi_pages.docx/saveAs" \
-X PUT \
-d "{'SaveFormat':'pdf', 'FileName': 'test_multi_pages.pdf'}" \
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
## SDKs

Using an SDK is the best way to speed up the development. An SDK takes care of low-level details and lets you focus on your project tasks. Check out our [GitHub repository](https://github.com/aspose-words-cloud) for a complete list of Aspose.Words SDKs with code examples.

## SDK Examples

Code examples for various SDKs are presented below:
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
