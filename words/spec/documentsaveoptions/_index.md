---
title: "DocumentSaveOptions"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /spec/documentsaveoptions/
description: "DocumentSaveOptions"
notoc: true
weight: 200
---


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
  </tbody>
</table>


## BmpSaveOptionsData

Represents a container class for bmp save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| HorizontalResolution | <span style="color:SteelBlue;">double</span>  | Gets or sets the horizontal resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| ImageBrightness      | <span style="color:SteelBlue;">double</span>  | Gets or sets the brightness level of the image. |
| ImageColorMode       | [ImageColorModeEnum](#imagesaveoptionsdata.imagecolormodeenum) | Gets or sets the color mode of the image. |
| ImageContrast        | <span style="color:SteelBlue;">double</span>  | Gets or sets the contrast level of the image. |
| PaperColor           | <span style="color:SteelBlue;">string</span>  | Gets or sets the background (paper) color of the image. |
| PixelFormat          | [PixelFormatEnum](#imagesaveoptionsdata.pixelformatenum) | Gets or sets the pixel format of the image. |
| Resolution           | <span style="color:SteelBlue;">double</span>  | Gets or sets both horizontal and vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| Scale                | <span style="color:SteelBlue;">double</span>  | Gets or sets the zoom factor of the image. |
| UseAntiAliasing      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use anti-aliasing for rendering. |
| UseGdiEmfRenderer    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF. |
| UseHighQualityRendering | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms. |
| VerticalResolution   | <span style="color:SteelBlue;">double</span>  | Gets or sets the vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |


## DocmSaveOptionsData

Represents a container class for docm save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the oOXML version for the output document. |
| CompressionLevel     | [CompressionLevelEnum](#ooxmlsaveoptionsdata.compressionlevelenum) | Gets or sets the compression level. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document using ECMA376 Standard encryption algorithm. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## DocSaveOptionsData

Represents a container class for doc/dot save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| AlwaysCompressMetafiles | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating when False, that small metafiles are not compressed for performance reason. The default value is true, all metafiles are compressed regardless of its size. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password. |
| SavePictureBullet    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating when False, that PictureBullet data is not saved to the output document. The default value is true. |
| SaveRoutingSlip      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to save RoutingSlip data to output document. |


## DocxSaveOptionsData

Represents a container class for docx save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the oOXML version for the output document. |
| CompressionLevel     | [CompressionLevelEnum](#ooxmlsaveoptionsdata.compressionlevelenum) | Gets or sets the compression level. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document using ECMA376 Standard encryption algorithm. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## DotmSaveOptionsData

Represents a container class for dotm save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the oOXML version for the output document. |
| CompressionLevel     | [CompressionLevelEnum](#ooxmlsaveoptionsdata.compressionlevelenum) | Gets or sets the compression level. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document using ECMA376 Standard encryption algorithm. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## DotSaveOptionsData

Represents a container class for dot save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| AlwaysCompressMetafiles | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating when False, that small metafiles are not compressed for performance reason. The default value is true, all metafiles are compressed regardless of its size. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password. |
| SavePictureBullet    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating when False, that PictureBullet data is not saved to the output document. The default value is true. |
| SaveRoutingSlip      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to save RoutingSlip data to output document. |


## DotxSaveOptionsData

Represents a container class for dotx save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the oOXML version for the output document. |
| CompressionLevel     | [CompressionLevelEnum](#ooxmlsaveoptionsdata.compressionlevelenum) | Gets or sets the compression level. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document using ECMA376 Standard encryption algorithm. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## EmfSaveOptionsData

Represents a container class for emf save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| HorizontalResolution | <span style="color:SteelBlue;">double</span>  | Gets or sets the horizontal resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| ImageBrightness      | <span style="color:SteelBlue;">double</span>  | Gets or sets the brightness level of the image. |
| ImageColorMode       | [ImageColorModeEnum](#imagesaveoptionsdata.imagecolormodeenum) | Gets or sets the color mode of the image. |
| ImageContrast        | <span style="color:SteelBlue;">double</span>  | Gets or sets the contrast level of the image. |
| PaperColor           | <span style="color:SteelBlue;">string</span>  | Gets or sets the background (paper) color of the image. |
| PixelFormat          | [PixelFormatEnum](#imagesaveoptionsdata.pixelformatenum) | Gets or sets the pixel format of the image. |
| Resolution           | <span style="color:SteelBlue;">double</span>  | Gets or sets both horizontal and vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| Scale                | <span style="color:SteelBlue;">double</span>  | Gets or sets the zoom factor of the image. |
| UseAntiAliasing      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use anti-aliasing for rendering. |
| UseGdiEmfRenderer    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF. |
| UseHighQualityRendering | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms. |
| VerticalResolution   | <span style="color:SteelBlue;">double</span>  | Gets or sets the vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |


## EpubSaveOptionsData

Represents a container class for epub save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| AllowNegativeIndent  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether negative left and right indents of paragraphs are allowed (not normalized) . |
| CssClassNamePrefix   | <span style="color:SteelBlue;">string</span>  | Gets or sets the prefix which is added to all CSS class names. The default value is an empty string and generated CSS class names have no common prefix. If this value is not empty, all CSS classes generated by Aspose.Words will start with the specified prefix.This might be useful, for example, if you add custom CSS to generated documents and want to prevent class name conflicts. If the value is not null or empty, it must be a valid CSS identifier. |
| CssStyleSheetFileName | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the CSS file written when the document is exported to HTML. |
| CssStyleSheetType    | [CssStyleSheetTypeEnum](/words/spec/style#htmlsaveoptionsdata.cssstylesheettypeenum) | Gets or sets the option that controls how the CSS styles are exported. |
| DocumentSplitCriteria | [DocumentSplitCriteriaEnum](#htmlsaveoptionsdata.documentsplitcriteriaenum) | Gets or sets the option that controls how the document should be split when saving. |
| DocumentSplitHeadingLevel | <span style="color:SteelBlue;">int</span>     | Gets or sets the maximum level of headings at which to split the document. |
| Encoding             | <span style="color:SteelBlue;">string</span>  | Gets or sets the character encoding to use when exporting. |
| ExportDocumentProperties | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to export built-in and custom document properties. |
| ExportDropDownFormFieldAsText | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how drop-down form fields are saved to HTML. The default value is false. |
| ExportFontResources  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether font resources should be exported. |
| ExportFontsAsBase64  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fonts resources should be embedded to HTML in Base64 encoding. The default value is false. |
| ExportHeadersFootersMode | [ExportHeadersFootersModeEnum](#htmlsaveoptionsdata.exportheadersfootersmodeenum) | Gets or sets the option that controls how headers and footers are exported. |
| ExportImagesAsBase64 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether images are saved in Base64 format. |
| ExportLanguageInformation | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether language information is exported. |
| ExportListLabels     | [ExportListLabelsEnum](#htmlsaveoptionsdata.exportlistlabelsenum) | Gets or sets the option that controls how list labels are exported. |
| ExportOriginalUrlForLinkedImages | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the original URL should be used as the URL of the linked images. The default value is false. |
| ExportPageMargins    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether page margins are exported to HTML, MHTML or EPUB. The default value is false. |
| ExportPageSetup      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether page setup is exported. |
| ExportRelativeFontSize | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether font sizes should be output in relative units when saving. |
| ExportRoundtripInformation | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to write the roundtrip information when saving to HTML. The default value is true. |
| ExportTextBoxAsSvg   | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how textboxes represented by Aspose.Words.Drawing.Shape are saved to HTML, MHTML or EPUB. The default value is false. When set to true, exports textboxes as inline "svg" elements. When false, exports as "image" elements. |
| ExportTextInputFormFieldAsText | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how text input form fields are saved. |
| ExportTocPageNumbers | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to write page numbers to table of contents when saving. |
| ExportXhtmlTransitional | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to write the DOCTYPE declaration when saving. |
| FontResourcesSubsettingSizeThreshold | <span style="color:SteelBlue;">int</span>     | Gets or sets the option that controls which font resources need subsetting when saving. |
| FontsFolder          | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where fonts are saved when exporting a document. |
| FontsFolderAlias     | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct font URIs. |
| HtmlVersion          | [HtmlVersionEnum](#htmlsaveoptionsdata.htmlversionenum) | Gets or sets the version of HTML standard, that should be used when saving the document to HTML or MHTML. Default value is Aspose.Words.Saving.HtmlVersion.Xhtml. |
| ImageResolution      | <span style="color:SteelBlue;">int</span>     | Gets or sets the output resolution for images when exporting. |
| ImagesFolder         | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where images are saved when exporting a document. |
| ImagesFolderAlias    | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct image URIs. |
| MetafileFormat       | [MetafileFormatEnum](#htmlsaveoptionsdata.metafileformatenum) | Gets or sets the options, that controls in what format metafiles are saved when exporting to HTML, MHTML, or EPUB. The default value is Aspose.Words.Saving.HtmlMetafileFormat.Png, meaning that metafiles are rendered to raster PNG images. Metafiles are not natively displayed by HTML browsers. By default, Aspose.Words converts WMF and EMF images into PNG files when exporting to HTML.Other options are to convert metafiles to SVG images or to export them as is without conversion. Some image transforms, in particular image cropping, will not be applied to metafile images if they are exported to HTML without conversion. |
| OfficeMathOutputMode | [OfficeMathOutputModeEnum](#htmlsaveoptionsdata.officemathoutputmodeenum) | Gets or sets the option that controls how OfficeMath objects are exported to HTML, MHTML or EPUB. The default value is HtmlOfficeMathOutputMode.Image. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |
| ResolveFontNames     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether font family names used in the document are resolved and substituted according to FontSettings when being written into HTML-based formats. The default value is false. |
| ResourceFolder       | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where all resources like images, fonts, and external CSS are saved when a document is exported to HTML. The default value is an empty string. |
| ResourceFolderAlias  | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct URIs of all resources written into HTML document. The default value is an empty string. |
| ScaleImageToShapeSize | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether images are scaled by Aspose.Words to the bounding shape size when exporting. |
| TableWidthOutputMode | [TableWidthOutputModeEnum](#htmlsaveoptionsdata.tablewidthoutputmodeenum) | Gets or sets the option that controls how table, row and cell widths are exported. |
| EpubNavigationMapLevel | <span style="color:SteelBlue;">int</span>     | Gets or sets the maximum level of headings populated to the navigation map when exporting. |


## FixedPageSaveOptionsData

Represents a contains common options that can be specified when saving a document into fixed page formats (PDF, XPS, images etc) .

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |


## FlatOpcMacroSaveOptionsData

Represents a container class for fopc_macro save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the oOXML version for the output document. |
| CompressionLevel     | [CompressionLevelEnum](#ooxmlsaveoptionsdata.compressionlevelenum) | Gets or sets the compression level. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document using ECMA376 Standard encryption algorithm. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## FlatOpcSaveOptionsData

Represents a container class for fopc save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the oOXML version for the output document. |
| CompressionLevel     | [CompressionLevelEnum](#ooxmlsaveoptionsdata.compressionlevelenum) | Gets or sets the compression level. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document using ECMA376 Standard encryption algorithm. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## FlatOpcTemplateMacroSaveOptionsData

Represents a container class for fopc_template_macro save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the oOXML version for the output document. |
| CompressionLevel     | [CompressionLevelEnum](#ooxmlsaveoptionsdata.compressionlevelenum) | Gets or sets the compression level. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document using ECMA376 Standard encryption algorithm. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## FlatOpcTemplateSaveOptionsData

Represents a container class for fopc_template save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the oOXML version for the output document. |
| CompressionLevel     | [CompressionLevelEnum](#ooxmlsaveoptionsdata.compressionlevelenum) | Gets or sets the compression level. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document using ECMA376 Standard encryption algorithm. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## GifSaveOptionsData

Represents a container class for gif save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| HorizontalResolution | <span style="color:SteelBlue;">double</span>  | Gets or sets the horizontal resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| ImageBrightness      | <span style="color:SteelBlue;">double</span>  | Gets or sets the brightness level of the image. |
| ImageColorMode       | [ImageColorModeEnum](#imagesaveoptionsdata.imagecolormodeenum) | Gets or sets the color mode of the image. |
| ImageContrast        | <span style="color:SteelBlue;">double</span>  | Gets or sets the contrast level of the image. |
| PaperColor           | <span style="color:SteelBlue;">string</span>  | Gets or sets the background (paper) color of the image. |
| PixelFormat          | [PixelFormatEnum](#imagesaveoptionsdata.pixelformatenum) | Gets or sets the pixel format of the image. |
| Resolution           | <span style="color:SteelBlue;">double</span>  | Gets or sets both horizontal and vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| Scale                | <span style="color:SteelBlue;">double</span>  | Gets or sets the zoom factor of the image. |
| UseAntiAliasing      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use anti-aliasing for rendering. |
| UseGdiEmfRenderer    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF. |
| UseHighQualityRendering | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms. |
| VerticalResolution   | <span style="color:SteelBlue;">double</span>  | Gets or sets the vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |


## HtmlFixedSaveOptionsData

Represents a container class for fixed html save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| CssClassNamesPrefix  | <span style="color:SteelBlue;">string</span>  | Gets or sets the prefix which is added to all class names in style.css file. Default value is "aw". |
| Encoding             | <span style="color:SteelBlue;">string</span>  | Gets or sets the character encoding. |
| ExportEmbeddedCss    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the CSS (Cascading Style Sheet) should be embedded into the Html document. |
| ExportEmbeddedFonts  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fonts should be embedded into the Html document in Base64 format. |
| ExportEmbeddedImages | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether images should be embedded into the Html document in Base64 format. |
| ExportFormFields     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether form fields are exported as interactive items (as 'input' tag) rather than converted to text or graphics. |
| FontFormat           | [FontFormatEnum](#htmlfixedsaveoptionsdata.fontformatenum) | Gets or sets the export format of fonts. |
| PageHorizontalAlignment | [PageHorizontalAlignmentEnum](#htmlfixedsaveoptionsdata.pagehorizontalalignmentenum) | Gets or sets the horizontal alignment of pages in the HTML document. The default value is HtmlFixedHorizontalPageAlignment.Center. |
| PageMargins          | <span style="color:SteelBlue;">double</span>  | Gets or sets the margin around pages in HTML document. The margins value is measured in points and should be equal to or greater than 0. Default value is 10 points. |
| ResourcesFolder      | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where resources are saved when exporting the document. |
| ResourcesFolderAlias | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct resource URIs. |
| SaveFontFaceCssSeparately | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether "@font-face" CSS rules should be placed into a separate file "fontFaces.css" when a document is being saved with external stylesheet (that is, when Aspose.Words.Saving.HtmlFixedSaveOptions.ExportEmbeddedCss is false) . The default value is false, all CSS rules are written into single file "styles.css". |
| ShowPageBorder       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to show border around pages. |
| UseTargetMachineFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fonts from target machine must be used to display the document. If this flag is set to true, Aspose.Words.Saving.HtmlFixedSaveOptions.FontFormat and Aspose.Words.Saving.HtmlFixedSaveOptions.ExportEmbeddedFonts properties do not have effect, also Aspose.Words.Saving.HtmlFixedSaveOptions.ResourceSavingCallback is not fired for fonts. The default value is false. |


## HtmlSaveOptionsData

Represents a container class for html save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| AllowNegativeIndent  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether negative left and right indents of paragraphs are allowed (not normalized) . |
| CssClassNamePrefix   | <span style="color:SteelBlue;">string</span>  | Gets or sets the prefix which is added to all CSS class names. The default value is an empty string and generated CSS class names have no common prefix. If this value is not empty, all CSS classes generated by Aspose.Words will start with the specified prefix.This might be useful, for example, if you add custom CSS to generated documents and want to prevent class name conflicts. If the value is not null or empty, it must be a valid CSS identifier. |
| CssStyleSheetFileName | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the CSS file written when the document is exported to HTML. |
| CssStyleSheetType    | [CssStyleSheetTypeEnum](/words/spec/style#htmlsaveoptionsdata.cssstylesheettypeenum) | Gets or sets the option that controls how the CSS styles are exported. |
| DocumentSplitCriteria | [DocumentSplitCriteriaEnum](#htmlsaveoptionsdata.documentsplitcriteriaenum) | Gets or sets the option that controls how the document should be split when saving. |
| DocumentSplitHeadingLevel | <span style="color:SteelBlue;">int</span>     | Gets or sets the maximum level of headings at which to split the document. |
| Encoding             | <span style="color:SteelBlue;">string</span>  | Gets or sets the character encoding to use when exporting. |
| ExportDocumentProperties | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to export built-in and custom document properties. |
| ExportDropDownFormFieldAsText | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how drop-down form fields are saved to HTML. The default value is false. |
| ExportFontResources  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether font resources should be exported. |
| ExportFontsAsBase64  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fonts resources should be embedded to HTML in Base64 encoding. The default value is false. |
| ExportHeadersFootersMode | [ExportHeadersFootersModeEnum](#htmlsaveoptionsdata.exportheadersfootersmodeenum) | Gets or sets the option that controls how headers and footers are exported. |
| ExportImagesAsBase64 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether images are saved in Base64 format. |
| ExportLanguageInformation | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether language information is exported. |
| ExportListLabels     | [ExportListLabelsEnum](#htmlsaveoptionsdata.exportlistlabelsenum) | Gets or sets the option that controls how list labels are exported. |
| ExportOriginalUrlForLinkedImages | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the original URL should be used as the URL of the linked images. The default value is false. |
| ExportPageMargins    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether page margins are exported to HTML, MHTML or EPUB. The default value is false. |
| ExportPageSetup      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether page setup is exported. |
| ExportRelativeFontSize | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether font sizes should be output in relative units when saving. |
| ExportRoundtripInformation | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to write the roundtrip information when saving to HTML. The default value is true. |
| ExportTextBoxAsSvg   | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how textboxes represented by Aspose.Words.Drawing.Shape are saved to HTML, MHTML or EPUB. The default value is false. When set to true, exports textboxes as inline "svg" elements. When false, exports as "image" elements. |
| ExportTextInputFormFieldAsText | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how text input form fields are saved. |
| ExportTocPageNumbers | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to write page numbers to table of contents when saving. |
| ExportXhtmlTransitional | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to write the DOCTYPE declaration when saving. |
| FontResourcesSubsettingSizeThreshold | <span style="color:SteelBlue;">int</span>     | Gets or sets the option that controls which font resources need subsetting when saving. |
| FontsFolder          | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where fonts are saved when exporting a document. |
| FontsFolderAlias     | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct font URIs. |
| HtmlVersion          | [HtmlVersionEnum](#htmlsaveoptionsdata.htmlversionenum) | Gets or sets the version of HTML standard, that should be used when saving the document to HTML or MHTML. Default value is Aspose.Words.Saving.HtmlVersion.Xhtml. |
| ImageResolution      | <span style="color:SteelBlue;">int</span>     | Gets or sets the output resolution for images when exporting. |
| ImagesFolder         | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where images are saved when exporting a document. |
| ImagesFolderAlias    | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct image URIs. |
| MetafileFormat       | [MetafileFormatEnum](#htmlsaveoptionsdata.metafileformatenum) | Gets or sets the options, that controls in what format metafiles are saved when exporting to HTML, MHTML, or EPUB. The default value is Aspose.Words.Saving.HtmlMetafileFormat.Png, meaning that metafiles are rendered to raster PNG images. Metafiles are not natively displayed by HTML browsers. By default, Aspose.Words converts WMF and EMF images into PNG files when exporting to HTML.Other options are to convert metafiles to SVG images or to export them as is without conversion. Some image transforms, in particular image cropping, will not be applied to metafile images if they are exported to HTML without conversion. |
| OfficeMathOutputMode | [OfficeMathOutputModeEnum](#htmlsaveoptionsdata.officemathoutputmodeenum) | Gets or sets the option that controls how OfficeMath objects are exported to HTML, MHTML or EPUB. The default value is HtmlOfficeMathOutputMode.Image. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |
| ResolveFontNames     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether font family names used in the document are resolved and substituted according to FontSettings when being written into HTML-based formats. The default value is false. |
| ResourceFolder       | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where all resources like images, fonts, and external CSS are saved when a document is exported to HTML. The default value is an empty string. |
| ResourceFolderAlias  | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct URIs of all resources written into HTML document. The default value is an empty string. |
| ScaleImageToShapeSize | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether images are scaled by Aspose.Words to the bounding shape size when exporting. |
| TableWidthOutputMode | [TableWidthOutputModeEnum](#htmlsaveoptionsdata.tablewidthoutputmodeenum) | Gets or sets the option that controls how table, row and cell widths are exported. |


## ImageSaveOptionsData

Represents a container abstract class for image save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| HorizontalResolution | <span style="color:SteelBlue;">double</span>  | Gets or sets the horizontal resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| ImageBrightness      | <span style="color:SteelBlue;">double</span>  | Gets or sets the brightness level of the image. |
| ImageColorMode       | [ImageColorModeEnum](#imagesaveoptionsdata.imagecolormodeenum) | Gets or sets the color mode of the image. |
| ImageContrast        | <span style="color:SteelBlue;">double</span>  | Gets or sets the contrast level of the image. |
| PaperColor           | <span style="color:SteelBlue;">string</span>  | Gets or sets the background (paper) color of the image. |
| PixelFormat          | [PixelFormatEnum](#imagesaveoptionsdata.pixelformatenum) | Gets or sets the pixel format of the image. |
| Resolution           | <span style="color:SteelBlue;">double</span>  | Gets or sets both horizontal and vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| Scale                | <span style="color:SteelBlue;">double</span>  | Gets or sets the zoom factor of the image. |
| UseAntiAliasing      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use anti-aliasing for rendering. |
| UseGdiEmfRenderer    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF. |
| UseHighQualityRendering | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms. |
| VerticalResolution   | <span style="color:SteelBlue;">double</span>  | Gets or sets the vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |


## JpegSaveOptionsData

Represents a container class for jpeg save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| HorizontalResolution | <span style="color:SteelBlue;">double</span>  | Gets or sets the horizontal resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| ImageBrightness      | <span style="color:SteelBlue;">double</span>  | Gets or sets the brightness level of the image. |
| ImageColorMode       | [ImageColorModeEnum](#imagesaveoptionsdata.imagecolormodeenum) | Gets or sets the color mode of the image. |
| ImageContrast        | <span style="color:SteelBlue;">double</span>  | Gets or sets the contrast level of the image. |
| PaperColor           | <span style="color:SteelBlue;">string</span>  | Gets or sets the background (paper) color of the image. |
| PixelFormat          | [PixelFormatEnum](#imagesaveoptionsdata.pixelformatenum) | Gets or sets the pixel format of the image. |
| Resolution           | <span style="color:SteelBlue;">double</span>  | Gets or sets both horizontal and vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| Scale                | <span style="color:SteelBlue;">double</span>  | Gets or sets the zoom factor of the image. |
| UseAntiAliasing      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use anti-aliasing for rendering. |
| UseGdiEmfRenderer    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF. |
| UseHighQualityRendering | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms. |
| VerticalResolution   | <span style="color:SteelBlue;">double</span>  | Gets or sets the vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |


## MarkdownSaveOptionsData

Represents a container class for markdown save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Encoding             | <span style="color:SteelBlue;">string</span>  | Gets or sets the character encoding to use when exporting in plain text format. |
| ExportHeadersFootersMode | [ExportHeadersFootersModeEnum](#htmlsaveoptionsdata.exportheadersfootersmodeenum) | Gets or sets the option that controls whether to output headers and footers when exporting in plain text format. default value is TxtExportHeadersFootersMode.PrimaryOnly. |
| ForcePageBreaks      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the page breaks should be preserved during export. The default value is false. |
| ParagraphBreak       | <span style="color:SteelBlue;">string</span>  | Gets or sets the string to use as a paragraph break when exporting in plain text format. |
| TableContentAlignment | [TableContentAlignmentEnum](#markdownsaveoptionsdata.tablecontentalignmentenum) | Gets or sets the value, that specifies how to align contents in tables when exporting into the Markdown format. The default value is Auto. |


## MhtmlSaveOptionsData

Represents a container class for mhtml save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| AllowNegativeIndent  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether negative left and right indents of paragraphs are allowed (not normalized) . |
| CssClassNamePrefix   | <span style="color:SteelBlue;">string</span>  | Gets or sets the prefix which is added to all CSS class names. The default value is an empty string and generated CSS class names have no common prefix. If this value is not empty, all CSS classes generated by Aspose.Words will start with the specified prefix.This might be useful, for example, if you add custom CSS to generated documents and want to prevent class name conflicts. If the value is not null or empty, it must be a valid CSS identifier. |
| CssStyleSheetFileName | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the CSS file written when the document is exported to HTML. |
| CssStyleSheetType    | [CssStyleSheetTypeEnum](/words/spec/style#htmlsaveoptionsdata.cssstylesheettypeenum) | Gets or sets the option that controls how the CSS styles are exported. |
| DocumentSplitCriteria | [DocumentSplitCriteriaEnum](#htmlsaveoptionsdata.documentsplitcriteriaenum) | Gets or sets the option that controls how the document should be split when saving. |
| DocumentSplitHeadingLevel | <span style="color:SteelBlue;">int</span>     | Gets or sets the maximum level of headings at which to split the document. |
| Encoding             | <span style="color:SteelBlue;">string</span>  | Gets or sets the character encoding to use when exporting. |
| ExportDocumentProperties | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to export built-in and custom document properties. |
| ExportDropDownFormFieldAsText | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how drop-down form fields are saved to HTML. The default value is false. |
| ExportFontResources  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether font resources should be exported. |
| ExportFontsAsBase64  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fonts resources should be embedded to HTML in Base64 encoding. The default value is false. |
| ExportHeadersFootersMode | [ExportHeadersFootersModeEnum](#htmlsaveoptionsdata.exportheadersfootersmodeenum) | Gets or sets the option that controls how headers and footers are exported. |
| ExportImagesAsBase64 | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether images are saved in Base64 format. |
| ExportLanguageInformation | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether language information is exported. |
| ExportListLabels     | [ExportListLabelsEnum](#htmlsaveoptionsdata.exportlistlabelsenum) | Gets or sets the option that controls how list labels are exported. |
| ExportOriginalUrlForLinkedImages | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the original URL should be used as the URL of the linked images. The default value is false. |
| ExportPageMargins    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether page margins are exported to HTML, MHTML or EPUB. The default value is false. |
| ExportPageSetup      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether page setup is exported. |
| ExportRelativeFontSize | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether font sizes should be output in relative units when saving. |
| ExportRoundtripInformation | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to write the roundtrip information when saving to HTML. The default value is true. |
| ExportTextBoxAsSvg   | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how textboxes represented by Aspose.Words.Drawing.Shape are saved to HTML, MHTML or EPUB. The default value is false. When set to true, exports textboxes as inline "svg" elements. When false, exports as "image" elements. |
| ExportTextInputFormFieldAsText | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how text input form fields are saved. |
| ExportTocPageNumbers | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to write page numbers to table of contents when saving. |
| ExportXhtmlTransitional | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to write the DOCTYPE declaration when saving. |
| FontResourcesSubsettingSizeThreshold | <span style="color:SteelBlue;">int</span>     | Gets or sets the option that controls which font resources need subsetting when saving. |
| FontsFolder          | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where fonts are saved when exporting a document. |
| FontsFolderAlias     | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct font URIs. |
| HtmlVersion          | [HtmlVersionEnum](#htmlsaveoptionsdata.htmlversionenum) | Gets or sets the version of HTML standard, that should be used when saving the document to HTML or MHTML. Default value is Aspose.Words.Saving.HtmlVersion.Xhtml. |
| ImageResolution      | <span style="color:SteelBlue;">int</span>     | Gets or sets the output resolution for images when exporting. |
| ImagesFolder         | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where images are saved when exporting a document. |
| ImagesFolderAlias    | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct image URIs. |
| MetafileFormat       | [MetafileFormatEnum](#htmlsaveoptionsdata.metafileformatenum) | Gets or sets the options, that controls in what format metafiles are saved when exporting to HTML, MHTML, or EPUB. The default value is Aspose.Words.Saving.HtmlMetafileFormat.Png, meaning that metafiles are rendered to raster PNG images. Metafiles are not natively displayed by HTML browsers. By default, Aspose.Words converts WMF and EMF images into PNG files when exporting to HTML.Other options are to convert metafiles to SVG images or to export them as is without conversion. Some image transforms, in particular image cropping, will not be applied to metafile images if they are exported to HTML without conversion. |
| OfficeMathOutputMode | [OfficeMathOutputModeEnum](#htmlsaveoptionsdata.officemathoutputmodeenum) | Gets or sets the option that controls how OfficeMath objects are exported to HTML, MHTML or EPUB. The default value is HtmlOfficeMathOutputMode.Image. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |
| ResolveFontNames     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether font family names used in the document are resolved and substituted according to FontSettings when being written into HTML-based formats. The default value is false. |
| ResourceFolder       | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where all resources like images, fonts, and external CSS are saved when a document is exported to HTML. The default value is an empty string. |
| ResourceFolderAlias  | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct URIs of all resources written into HTML document. The default value is an empty string. |
| ScaleImageToShapeSize | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether images are scaled by Aspose.Words to the bounding shape size when exporting. |
| TableWidthOutputMode | [TableWidthOutputModeEnum](#htmlsaveoptionsdata.tablewidthoutputmodeenum) | Gets or sets the option that controls how table, row and cell widths are exported. |
| ExportCidUrlsForMhtmlResources | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use CID (Content-ID) URLs to reference resources (images, fonts, CSS) included in MHTML documents. The default value is false. |


## OdtSaveOptionsData

Represents a container class for odt/ott save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| IsStrictSchema11     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether export should correspond to ODT specification 1.1 strictly. |
| MeasureUnit          | [MeasureUnitEnum](#odtsaveoptionsdata.measureunitenum) | Gets or sets the units of measure to apply to document content. The default value is Aspose.Words.Saving.OdtSaveMeasureUnit.Centimeters. Open Office uses centimeters when specifying lengths, widths and other measurable formatting and content properties in documents whereas MS Office uses inches. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## OoxmlSaveOptionsData

Represents a container class for docx/docm/dotx/dotm/flatopc save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the oOXML version for the output document. |
| CompressionLevel     | [CompressionLevelEnum](#ooxmlsaveoptionsdata.compressionlevelenum) | Gets or sets the compression level. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document using ECMA376 Standard encryption algorithm. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## OpenXpsSaveOptionsData

Represents a container class for xps save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| BookmarksOutlineLevel | <span style="color:SteelBlue;">int</span>     | Gets or sets the level in the XPS document outline at which to display Word bookmarks. |
| HeadingsOutlineLevels | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of heading levels (paragraphs formatted with the Heading styles) to include in the XPS document outline. |
| OutlineOptions       | [OutlineOptionsData](#outlineoptionsdata)     | Gets or sets the outline options. |
| UseBookFoldPrintingSettings | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the document should be saved using a booklet printing layout. |


## OttSaveOptionsData

Represents a container class for ott save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| IsStrictSchema11     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether export should correspond to ODT specification 1.1 strictly. |
| MeasureUnit          | [MeasureUnitEnum](#odtsaveoptionsdata.measureunitenum) | Gets or sets the units of measure to apply to document content. The default value is Aspose.Words.Saving.OdtSaveMeasureUnit.Centimeters. Open Office uses centimeters when specifying lengths, widths and other measurable formatting and content properties in documents whereas MS Office uses inches. |
| Password             | <span style="color:SteelBlue;">string</span>  | Gets or sets the password to encrypt document. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## PclSaveOptionsData

Represents a container class for pcl save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| FalllbackFontName    | <span style="color:SteelBlue;">string</span>  | Gets or sets the font name, that will be used if no expected font is found in printer and built-in fonts collections. |
| RasterizeTransformedElements | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether complex transformed elements should be rasterized before saving to PCL document.. The default value is true. |


## PdfSaveOptionsData

Represents a container class for pdf save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| Compliance           | [ComplianceEnum](#ooxmlsaveoptionsdata.complianceenum) | Gets or sets the PDF standards compliance level for output documents. |
| CreateNoteHyperlinks | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to convert footnote/endnote references in main text story into active hyperlinks. When clicked the hyperlink will lead to the corresponding footnote/endnote. The default value is false. |
| CustomPropertiesExport | [CustomPropertiesExportEnum](#pdfsaveoptionsdata.custompropertiesexportenum) | Gets or sets the option that controls the way CustomDocumentProperties are exported to PDF file. The default value is None. |
| DigitalSignatureDetails | [PdfDigitalSignatureDetailsData](#pdfdigitalsignaturedetailsdata) | Gets or sets the details for signing the output PDF document. |
| DisplayDocTitle      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the window’s title bar should display the document title taken from the Title entry of the document information dictionary. |
| DownsampleOptions    | [DownsampleOptionsData](#downsampleoptionsdata) | Gets or sets the downsample options. |
| EmbedFullFonts       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fonts are embedded into the resulting PDF documents. |
| EncryptionDetails    | [PdfEncryptionDetailsData](#pdfencryptiondetailsdata) | Gets or sets the details for encrypting the output PDF document. |
| ExportDocumentStructure | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to export document structure. |
| ExportLanguageToSpanTag | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether or not to create a "Span" tag in the document structure to export the text language. |
| FontEmbeddingMode    | [FontEmbeddingModeEnum](#pdfsaveoptionsdata.fontembeddingmodeenum) | Gets or sets the font embedding mode. |
| HeaderFooterBookmarksExportMode | [HeaderFooterBookmarksExportModeEnum](#pdfsaveoptionsdata.headerfooterbookmarksexportmodeenum) | Gets or sets the option that controls how bookmarks in headers/footers are exported. The default value is Aspose.Words.Saving.HeaderFooterBookmarksExportMode.All. |
| ImageColorSpaceExportMode | [ImageColorSpaceExportModeEnum](#pdfsaveoptionsdata.imagecolorspaceexportmodeenum) | Gets or sets the option that controls how the color space will be selected for the images in PDF document. |
| ImageCompression     | <span style="color:SteelBlue;">string</span>  | Gets or sets the compression type to be used for all images in the document. |
| InterpolateImages    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether image interpolation shall be performed by a conforming reader. When false is specified, the flag is not written to the output document and the default behavior of reader is used instead. |
| OpenHyperlinksInNewWindow | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether hyperlinks in the output Pdf document are forced to be opened in a new window (or tab) of a browser. |
| OutlineOptions       | [OutlineOptionsData](#outlineoptionsdata)     | Gets or sets the outline options. |
| PageMode             | [PageModeEnum](#pdfsaveoptionsdata.pagemodeenum) | Gets or sets the option that controls how the PDF document should be displayed when opened in the PDF reader. |
| PreblendImages       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to preblend transparent images with black background color. |
| PreserveFormFields   | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to preserve Microsoft Word form fields as form fields in PDF or convert them to text. |
| TextCompression      | [TextCompressionEnum](#pdfsaveoptionsdata.textcompressionenum) | Gets or sets the compression type to be used for all textual content in the document. |
| UseBookFoldPrintingSettings | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the document should be saved using a booklet printing layout. |
| UseCoreFonts         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to substitute TrueType fonts Arial, Times New Roman, Courier New and Symbol with core PDF Type 1 fonts. |
| ZoomBehavior         | [ZoomBehaviorEnum](#pdfsaveoptionsdata.zoombehaviorenum) | Gets or sets the option that controls what type of zoom should be applied when a document is opened with a PDF viewer. |
| ZoomFactor           | <span style="color:SteelBlue;">int</span>     | Gets or sets the zoom factor (in percentages) for a document. |


## PngSaveOptionsData

Represents a container class for png save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| HorizontalResolution | <span style="color:SteelBlue;">double</span>  | Gets or sets the horizontal resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| ImageBrightness      | <span style="color:SteelBlue;">double</span>  | Gets or sets the brightness level of the image. |
| ImageColorMode       | [ImageColorModeEnum](#imagesaveoptionsdata.imagecolormodeenum) | Gets or sets the color mode of the image. |
| ImageContrast        | <span style="color:SteelBlue;">double</span>  | Gets or sets the contrast level of the image. |
| PaperColor           | <span style="color:SteelBlue;">string</span>  | Gets or sets the background (paper) color of the image. |
| PixelFormat          | [PixelFormatEnum](#imagesaveoptionsdata.pixelformatenum) | Gets or sets the pixel format of the image. |
| Resolution           | <span style="color:SteelBlue;">double</span>  | Gets or sets both horizontal and vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |
| Scale                | <span style="color:SteelBlue;">double</span>  | Gets or sets the zoom factor of the image. |
| UseAntiAliasing      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use anti-aliasing for rendering. |
| UseGdiEmfRenderer    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF. |
| UseHighQualityRendering | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms. |
| VerticalResolution   | <span style="color:SteelBlue;">double</span>  | Gets or sets the vertical resolution in dots per inch for the generated images. This property has effect only when saving to raster image formats. The default value is 96. |


## PsSaveOptionsData

Represents a container class for ps save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| UseBookFoldPrintingSettings | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the document should be saved using a booklet printing layout. |


## RtfSaveOptionsData

Represents a container class for rtf save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ExportCompactSize    | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to make output RTF documents smaller in size, but if they contain RTL (right-to-left) text, it will not be displayed correctly. |
| ExportImagesForOldReaders | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the keywords for "old readers" are written to RTF or not. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |
| SaveImagesAsWmf      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether when true all images will be saved as WMF. This option might help to avoid WordPad warning messages. |


## SvgSaveOptionsData

Represents a container class for svg save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| ExportEmbeddedImages | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether images should be embedded into SVG document as base64. |
| FitToViewPort        | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the output SVG should fill the available viewport area (browser window or container) . When set to true width and height of output SVG are set to 100%. |
| ResourcesFolder      | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where resources (images) are saved when exporting. |
| ResourcesFolderAlias | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct image URIs. |
| ShowPageBorder       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to show or hide page stepper. |
| TextOutputMode       | [TextOutputModeEnum](#svgsaveoptionsdata.textoutputmodeenum) | Gets or sets the option that controls how text should be rendered. |


## TextSaveOptionsData

Represents a container class for text save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Encoding             | <span style="color:SteelBlue;">string</span>  | Gets or sets the character encoding to use when exporting in plain text format. |
| ExportHeadersFootersMode | [ExportHeadersFootersModeEnum](#htmlsaveoptionsdata.exportheadersfootersmodeenum) | Gets or sets the option that controls whether to output headers and footers when exporting in plain text format. default value is TxtExportHeadersFootersMode.PrimaryOnly. |
| ForcePageBreaks      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the page breaks should be preserved during export. The default value is false. |
| ParagraphBreak       | <span style="color:SteelBlue;">string</span>  | Gets or sets the string to use as a paragraph break when exporting in plain text format. |
| AddBidiMarks         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to add bi-directional marks before each BiDi run when exporting in plain text format. The default value is true. |
| MaxCharactersPerLine | <span style="color:SteelBlue;">int</span>     | Gets or sets an integer value that specifies the maximum number of characters per one line. The default value is 0, that means no limit. |
| PreserveTableLayout  | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the program should attempt to preserve layout of tables when saving in the plain text format. |
| SimplifyListLabels   | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the program should simplify list labels in case of complex label formatting not being adequately represented by plain text. |


## TxtSaveOptionsBaseData

Represents a base class for save options of text formats.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| Encoding             | <span style="color:SteelBlue;">string</span>  | Gets or sets the character encoding to use when exporting in plain text format. |
| ExportHeadersFootersMode | [ExportHeadersFootersModeEnum](#htmlsaveoptionsdata.exportheadersfootersmodeenum) | Gets or sets the option that controls whether to output headers and footers when exporting in plain text format. default value is TxtExportHeadersFootersMode.PrimaryOnly. |
| ForcePageBreaks      | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the page breaks should be preserved during export. The default value is false. |
| ParagraphBreak       | <span style="color:SteelBlue;">string</span>  | Gets or sets the string to use as a paragraph break when exporting in plain text format. |


## WordMLSaveOptionsData

Represents a container class for wml save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| PrettyFormat         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to use pretty formats output. |


## XamlFixedSaveOptionsData

Represents a container class for xaml fixed save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| ResourcesFolder      | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where resources (images and fonts) are saved when exporting a document to fixed page Xaml format. The default value is null. |
| ResourcesFolderAlias | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct image URIs written into an fixed page Xaml document. The default value is null. |


## XamlFlowPackSaveOptionsData

Represents a container class for xamlflow_pack save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ImagesFolder         | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where images are saved when exporting. |
| ImagesFolderAlias    | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct image URIs. |


## XamlFlowSaveOptionsData

Represents a container class for xaml flow save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ImagesFolder         | <span style="color:SteelBlue;">string</span>  | Gets or sets the physical folder where images are saved when exporting. |
| ImagesFolderAlias    | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of the folder used to construct image URIs. |


## XpsSaveOptionsData

Represents a container class for xps save options.

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| AllowEmbeddingPostScriptFonts | <span style="color:SteelBlue;">bool</span>    | Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false.. |
| CustomTimeZoneInfoData | [TimeZoneInfoData](/words/spec/document#timezoneinfodata) | Gets or sets CustomTimeZoneInfo. |
| Dml3DEffectsRenderingMode | [Dml3DEffectsRenderingModeEnum](#saveoptionsdata.dml3deffectsrenderingmodeenum) | Gets or sets the value determining how 3D effects are rendered. |
| DmlEffectsRenderingMode | [DmlEffectsRenderingModeEnum](#saveoptionsdata.dmleffectsrenderingmodeenum) | Gets or sets the value determining how DrawingML effects are rendered. { Simplified | None | Fine }. |
| DmlRenderingMode     | [DmlRenderingModeEnum](#saveoptionsdata.dmlrenderingmodeenum) | Gets or sets the option that controls how DrawingML shapes are rendered. |
| FileName             | <span style="color:SteelBlue;">string</span>  | Gets or sets the name of destination file. |
| FlatOpcXmlMappingOnly | <span style="color:SteelBlue;">bool</span>    | Gets or sets value determining which document formats are allowed to be mapped by Aspose.Words.Markup.StructuredDocumentTag.XmlMapping. By default only Aspose.Words.LoadFormat.FlatOpc document format is allowed to be mapped. |
| ImlRenderingMode     | [ImlRenderingModeEnum](#saveoptionsdata.imlrenderingmodeenum) | Gets or sets the value determining how ink (InkML) objects are rendered. |
| SaveFormat           | <span style="color:SteelBlue;">string</span>  | Gets the format of save. |
| UpdateCreatedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value determining whether the Aspose.Words.Properties.BuiltInDocumentProperties.CreatedTime property is updated before saving. Default value is false. |
| UpdateFields         | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether fields should be updated before saving the document to a fixed page format. The default value is true. |
| UpdateLastPrintedProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastPrinted property is updated before saving. |
| UpdateLastSavedTimeProperty | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the Aspose.Words.Properties.BuiltInDocumentProperties.LastSavedTime property is updated before saving. |
| UpdateSdtContent     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether content of StructuredDocumentTag is updated before saving. |
| ZipOutput            | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to zip output or not. The default value is false. |
| ColorMode            | [ColorModeEnum](#fixedpagesaveoptionsdata.colormodeenum) | Gets or sets the value determining how colors are rendered. { Normal | Grayscale}. |
| JpegQuality          | <span style="color:SteelBlue;">int</span>     | Gets or sets the quality of the JPEG images inside PDF document. |
| MetafileRenderingOptions | [MetafileRenderingOptionsData](#metafilerenderingoptionsdata) | Gets or sets the metafile rendering options. |
| NumeralFormat        | [NumeralFormatEnum](#fixedpagesaveoptionsdata.numeralformatenum) | Gets or sets the symbol set, that is used to represent numbers while rendering to fixed page formats. |
| OptimizeOutput       | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether it is required to optimize output of XPS. If this flag is set redundant nested canvases and empty canvases are removed, also neighbor glyphs with the same formatting are concatenated. Note: The accuracy of the content display may be affected if this property is set to true.. The default value is false. |
| PageCount            | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of pages to render. |
| PageIndex            | <span style="color:SteelBlue;">int</span>     | Gets or sets the 0-based index of the first page to render. |
| BookmarksOutlineLevel | <span style="color:SteelBlue;">int</span>     | Gets or sets the level in the XPS document outline at which to display Word bookmarks. |
| HeadingsOutlineLevels | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of heading levels (paragraphs formatted with the Heading styles) to include in the XPS document outline. |
| OutlineOptions       | [OutlineOptionsData](#outlineoptionsdata)     | Gets or sets the outline options. |
| UseBookFoldPrintingSettings | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the document should be saved using a booklet printing layout. |


## PdfPermissions

This class is used in [PdfEncryptionDetailsData](#pdfencryptiondetailsdata).


## BookmarksOutlineLevelData

Represents a container class for individual bookmarks outline level.

This class is used in [OutlineOptionsData](#outlineoptionsdata).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| BookmarksOutlineLevel | <span style="color:SteelBlue;">int</span>     | Gets or sets the bookmark's level. |
| Name                 | <span style="color:SteelBlue;">string</span>  | Gets or sets the bookmark's name. |


## DownsampleOptionsData

Represents a container class for Downsample options.

This class is used in [PdfSaveOptionsData](#pdfsaveoptionsdata).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| DownsampleImages     | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether images should be downsampled. |
| Resolution           | <span style="color:SteelBlue;">int</span>     | Gets or sets the resolution in pixels per inch which the images should be downsampled to. |
| ResolutionThreshold  | <span style="color:SteelBlue;">int</span>     | Gets or sets the threshold resolution in pixels per inch. If resolution of an image in the document is less than threshold value, the downsampling algorithm will not be applied. A value of 0 means the threshold check is not used and all images that can be reduced in size are downsampled. |


## MetafileRenderingOptionsData

Represents a container class for options of metafile rendering.

This class is used in [BmpSaveOptionsData](#bmpsaveoptionsdata), [EmfSaveOptionsData](#emfsaveoptionsdata), [FixedPageSaveOptionsData](#fixedpagesaveoptionsdata), [GifSaveOptionsData](#gifsaveoptionsdata), [HtmlFixedSaveOptionsData](#htmlfixedsaveoptionsdata), [ImageSaveOptionsData](#imagesaveoptionsdata), [JpegSaveOptionsData](#jpegsaveoptionsdata), [PclSaveOptionsData](#pclsaveoptionsdata), [PdfSaveOptionsData](#pdfsaveoptionsdata), [PngSaveOptionsData](#pngsaveoptionsdata), [PsSaveOptionsData](#pssaveoptionsdata), [SvgSaveOptionsData](#svgsaveoptionsdata), [TiffSaveOptionsData](/words/spec/document#tiffsaveoptionsdata), [XamlFixedSaveOptionsData](#xamlfixedsaveoptionsdata), [XpsSaveOptionsData](#xpssaveoptionsdata).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| EmfPlusDualRenderingMode | [EmfPlusDualRenderingModeEnum](#metafilerenderingoptionsdata.emfplusdualrenderingmodeenum) | Gets or sets the option that controls how EMF+ Dual metafiles should be rendered. |
| EmulateRasterOperations | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether the raster operations should be emulated. |
| RenderingMode        | [RenderingModeEnum](#metafilerenderingoptionsdata.emfplusdualrenderingmodeenum) | Gets or sets the option that controls how metafile images should be rendered. |
| ScaleWmfFontsToMetafileSize | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to scale fonts in WMF metafile according to metafile size on the page. The default value is true. |
| UseEmfEmbeddedToWmf  | <span style="color:SteelBlue;">bool</span>    | Gets or sets the flag, that controls how WMF metafiles with embedded EMF metafiles should be rendered. |


## OutlineOptionsData

Represents a container class for outline options.

This class is used in [PdfSaveOptionsData](#pdfsaveoptionsdata), [XpsSaveOptionsData](#xpssaveoptionsdata).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| BookmarksOutlineLevels | List&lt;[BookmarksOutlineLevelData](#bookmarksoutlineleveldata)&gt; | Gets or sets the individual bookmarks outline level. |
| CreateMissingOutlineLevels | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to create missing outline levels when the document is exported. The default value is false. |
| CreateOutlinesForHeadingsInTables | <span style="color:SteelBlue;">bool</span>    | Gets or sets a value indicating whether to create outlines for headings (paragraphs formatted with the Heading styles) inside tables. |
| DefaultBookmarksOutlineLevel | <span style="color:SteelBlue;">int</span>     | Gets or sets the default level in the document outline at which to display Word bookmarks. |
| ExpandedOutlineLevels | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of levels in the document outline to show expanded when the file is viewed. |
| HeadingsOutlineLevels | <span style="color:SteelBlue;">int</span>     | Gets or sets the number of levels of headings (paragraphs formatted with the Heading styles) to include in the document outline. |


## PdfDigitalSignatureDetailsData

Represents a container class for details of digital signature.

This class is used in [PdfSaveOptionsData](#pdfsaveoptionsdata).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| CertificateFilename  | <span style="color:SteelBlue;">string</span>  | Gets or sets the certificate's filename using for signing. |
| HashAlgorithm        | [HashAlgorithmEnum](/words/spec/other#pdfdigitalsignaturedetailsdata.hashalgorithmenum) | Gets or sets the hash algorithm. |
| Location             | <span style="color:SteelBlue;">string</span>  | Gets or sets the location of the signing. |
| Reason               | <span style="color:SteelBlue;">string</span>  | Gets or sets the reason for the signing. |
| SignatureDate        | <span style="color:SteelBlue;">DateTime</span> | Gets or sets the date of the signing. |


## PdfEncryptionDetailsData

Represents a container class for details of encryption.

This class is used in [PdfSaveOptionsData](#pdfsaveoptionsdata).

The following properties are defined:

| Property             | Type                                          | Description |
|----------------------|-----------------------------------------------|-------------|
| OwnerPassword        | <span style="color:SteelBlue;">string</span>  | Gets or sets the owner password for the encrypted PDF document. |
| Permissions          | List&lt;[PdfPermissions](#pdfpermissions)&gt; | Gets or sets the operations that are allowed to a user on the encrypted PDF document. |
| UserPassword         | <span style="color:SteelBlue;">string</span>  | Gets or sets the user password required for opening the encrypted PDF document. |


## FixedPageSaveOptionsData.ColorModeEnum

The following values are defined: Normal, Grayscale.


## FixedPageSaveOptionsData.NumeralFormatEnum

The following values are defined: European, ArabicIndic, EasternArabicIndic, Context, System.


## HtmlFixedSaveOptionsData.FontFormatEnum

The following values are defined: Woff, Ttf.


## HtmlFixedSaveOptionsData.PageHorizontalAlignmentEnum

The following values are defined: Left, Center, Right.


## HtmlSaveOptionsData.DocumentSplitCriteriaEnum

The following values are defined: None, PageBreak, ColumnBreak, SectionBreak, HeadingParagraph.


## HtmlSaveOptionsData.ExportHeadersFootersModeEnum

The following values are defined: None, PerSection, FirstSectionHeaderLastSectionFooter, FirstPageHeaderFooterPerSection.


## HtmlSaveOptionsData.ExportListLabelsEnum

The following values are defined: Auto, AsInlineText, ByHtmlTags.


## HtmlSaveOptionsData.HtmlVersionEnum

The following values are defined: Xhtml, Html5.


## HtmlSaveOptionsData.MetafileFormatEnum

The following values are defined: Png, Svg, EmfOrWmf.


## HtmlSaveOptionsData.OfficeMathOutputModeEnum

The following values are defined: Image, MathML, Text.


## HtmlSaveOptionsData.TableWidthOutputModeEnum

The following values are defined: All, RelativeOnly, None.


## ImageSaveOptionsData.ImageColorModeEnum

The following values are defined: None, Grayscale, BlackAndWhite.


## ImageSaveOptionsData.PixelFormatEnum

The following values are defined: Format16BppRgb555, Format16BppRgb565, Format16BppArgb1555, Format24BppRgb, Format32BppRgb, Format32BppArgb, Format32BppPArgb, Format48BppRgb, Format64BppArgb, Format64BppPArgb, Format1bppIndexed.


## MarkdownSaveOptionsData.TableContentAlignmentEnum

The following values are defined: Auto, Left, Center, Right.


## MetafileRenderingOptionsData.EmfPlusDualRenderingModeEnum

The following values are defined: EmfPlusWithFallback, EmfPlus, Emf.


## MetafileRenderingOptionsData.RenderingModeEnum

The following values are defined: VectorWithFallback, Vector, Bitmap.


## OdtSaveOptionsData.MeasureUnitEnum

The following values are defined: Centimeters, Inches.


## OoxmlSaveOptionsData.ComplianceEnum

The following values are defined: Ecma376_2006, Iso29500_2008_Transitional, Iso29500_2008_Strict.


## OoxmlSaveOptionsData.CompressionLevelEnum

The following values are defined: Normal, Maximum, Fast, SuperFast.


## PdfSaveOptionsData.ComplianceEnum

The following values are defined: Pdf17, Pdf20, PdfA1a, PdfA1b, PdfA2a, PdfA2u, PdfUa1.


## PdfSaveOptionsData.CustomPropertiesExportEnum

The following values are defined: None, Standard, Metadata.


## PdfSaveOptionsData.FontEmbeddingModeEnum

The following values are defined: EmbedAll, EmbedNonstandard, EmbedNone.


## PdfSaveOptionsData.HeaderFooterBookmarksExportModeEnum

The following values are defined: None, First, All.


## PdfSaveOptionsData.ImageColorSpaceExportModeEnum

The following values are defined: Auto, SimpleCmyk.


## PdfSaveOptionsData.PageModeEnum

The following values are defined: UseNone, UseOutlines, UseThumbs, FullScreen, UseOC, UseAttachments.


## PdfSaveOptionsData.TextCompressionEnum

The following values are defined: None, Flate.


## PdfSaveOptionsData.ZoomBehaviorEnum

The following values are defined: None, ZoomFactor, FitPage, FitWidth, FitHeight, FitBox.


## SaveOptionsData.Dml3DEffectsRenderingModeEnum

The following values are defined: Basic, Advanced.


## SaveOptionsData.DmlEffectsRenderingModeEnum

The following values are defined: Simplified, None, Fine.


## SaveOptionsData.DmlRenderingModeEnum

The following values are defined: Fallback, DrawingML.


## SaveOptionsData.ImlRenderingModeEnum

The following values are defined: Fallback, InkML.


## SvgSaveOptionsData.TextOutputModeEnum

The following values are defined: UseSvgFonts, UseTargetMachineFonts, UsePlacedGlyphs.


## TiffSaveOptionsData.TiffBinarizationMethodEnum

The following values are defined: Threshold, FloydSteinbergDithering.


## TiffSaveOptionsData.TiffCompressionEnum

The following values are defined: None, Rle, Lzw, Ccitt3, Ccitt4.


## TxtSaveOptionsBaseData.ExportHeadersFootersModeEnum

The following values are defined: None, PrimaryOnly, AllAtEnd.

