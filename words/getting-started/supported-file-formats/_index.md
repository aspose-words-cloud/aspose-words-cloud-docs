---
title: "Supported File Formats"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /getting-started/supported-file-formats/
aliases: [/supported-file-formats/]
description: "A complete list of file formats supported by Aspose Words Cloud API"
weight: 30
---

The Aspose.Words Cloud API provides extensive I/O support for a variety of formats, including Word, PDF, Web, and eBook document formats. With read (import) and write (export) capabilities, developers can efficiently manage and customize content in these formats. This flexibility ensures that the Cloud API can satisfy a wide range of requirements and use cases.

Certain file formats, such as fixed page layout formats and image formats, are only supported for writing. They are primarily intended for storing static content in binary form, making it difficult to modify such files after they have been created. Therefore, our API offers export capabilities for these file formats only.

Below is the complete list of formats along with their import/export options.

## Microsoft Word formats

  | Format                                                              | Description                                                                        | Import                 | Export                 |
  |---------------------------------------------------------------------|------------------------------------------------------------------------------------|------------------------|------------------------|
  | [DOC](https://docs.fileformat.com/word-processing/doc/)             | Microsoft Word 97 – 2007 Document                                                  | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | DocPreWord60                                                        | Word 6 or Word 95 Document                                                         | {{< emoticons/tick >}} |                        |
  | [DOT](https://docs.fileformat.com/word-processing/dot/)             | Microsoft Word 97 – 2007 Template                                                  | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | WordML                                                              | Microsoft Word 2003 WordprocessingML                                               | {{< emoticons/tick >}} | {{< emoticons/tick >}} |


## Office Open XML formats

  | Format                                                              | Description                                                                                                 | Import                 | Export                 |
  |---------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|------------------------|------------------------|
  | [DOCM](https://docs.fileformat.com/word-processing/docm/)           | Office Open XML WordprocessingML Macro-Enabled Document                                                     | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [DOCX](https://docs.fileformat.com/word-processing/docx/)           | Office Open XML WordprocessingML Macro-Free Document                                                        | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [DOTM](https://docs.fileformat.com/word-processing/dotm/)           | Office Open XML WordprocessingML Macro-Enabled Template                                                     | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [DOTX](https://docs.fileformat.com/word-processing/dotx/)           | Office Open XML WordprocessingML Macro-Free Template                                                        | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | FlatOpc                                                             | Office Open XML WordprocessingML stored in a flat XML file instead of a ZIP package                         | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | FlatOpcMacroEnabled                                                 | Office Open XML WordprocessingML Macro-Enabled Document stored in a flat XML file instead of a ZIP package  | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | FlatOpcTemplate                                                     | Office Open XML WordprocessingML Template (macro-free) stored in a flat XML file instead of a ZIP package   | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | FlatOpcTemplateMacroEnabled                                         | Office Open XML WordprocessingML Macro-Enabled Template stored in a flat XML file instead of a ZIP package  | {{< emoticons/tick >}} | {{< emoticons/tick >}} |

## OpenDocument formats

  | Format                                                              | Description                                                                        | Import                 | Export                 |
  |---------------------------------------------------------------------|------------------------------------------------------------------------------------|------------------------|------------------------|
  | [ODT](https://docs.fileformat.com/word-processing/odt/)             | OpenDocument Text Document                                                         | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [OTT](https://docs.fileformat.com/word-processing/ott/)             | OpenDocument Text Template                                                         | {{< emoticons/tick >}} | {{< emoticons/tick >}} |

## PDF

  | Format                                                              | Description                                                                        | Import                 | Export                 |
  |---------------------------------------------------------------------|------------------------------------------------------------------------------------|------------------------|------------------------|
  | [PDF](https://docs.fileformat.com/pdf/)                             | Adobe Portable Document                                                            | {{< emoticons/tick >}} | {{< emoticons/tick >}} |


## Text and markup formats

  | Format                                                              | Description                                                                        | Import                 | Export                 |
  |---------------------------------------------------------------------|------------------------------------------------------------------------------------|------------------------|------------------------|
  | [HTML](https://docs.fileformat.com/web/html/)                       | Hyper Text Markup Language document                                                | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [MD](https://docs.fileformat.com/word-processing/md/)               | Markdown document                                                                  | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [MHTML](https://docs.fileformat.com/web/mhtml/)                     | Web archive that is MIME encapsulation of HTML documents                           | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [RTF](https://docs.fileformat.com/word-processing/rtf/)             | Rich Text Format document                                                          | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [TXT](https://docs.fileformat.com/word-processing/txt/)             | Plain Text                                                                         | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [XamlFlow](https://docs.fileformat.com/web/xaml/)                   | Extensible Application Markup Language (XAML) format as a flow document            |                        | {{< emoticons/tick >}} |
  | [XamlFlowPack](https://docs.fileformat.com/web/xaml/)               | Extensible Application Markup Language (XAML) package format as a flow document    |                        | {{< emoticons/tick >}} |
  | [XML](https://docs.fileformat.com/web/xml/)                         | eXtensible Markup Language document                                                | {{< emoticons/tick >}} |                        |

## eBook formats

  | Format                                                              | Description                                                                        | Import                 |    Export              |
  |---------------------------------------------------------------------|------------------------------------------------------------------------------------|------------------------|------------------------|
  | [AZW3](https://docs.fileformat.com/ebook/azw3/)                     | eBook format used by Amazon Kindle readers                                         | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [CHM](https://docs.fileformat.com/web/chm/)                         | Compiled HTML Help format                                                          | {{< emoticons/tick >}} |                        |
  | [EPUB](https://docs.fileformat.com/ebook/epub/)                     | IDPF EPUB format                                                                   | {{< emoticons/tick >}} | {{< emoticons/tick >}} |
  | [MOBI](https://docs.fileformat.com/ebook/mobi/)                     | eBook format used by the MobiPocket Reader and Amazon Kindle readers               | {{< emoticons/tick >}} | {{< emoticons/tick >}} |


## Fixed page layout formats

  | Format                                                              | Description                                                                        | Export                 |
  |---------------------------------------------------------------------|------------------------------------------------------------------------------------|------------------------|
  | [HtmlFixed](https://docs.fileformat.com/web/html/)                  | HTML format using absolutely positioned elements                                   | {{< emoticons/tick >}} |
  | [OpenXPS](https://docs.fileformat.com/page-description-language/xps/) | OpenXPS (ECMA-388) format                                                        | {{< emoticons/tick >}} |
  | [PCL](https://docs.fileformat.com/page-description-language/pcl/)   | Printer Control Language format                                                    | {{< emoticons/tick >}} |
  | [PS](https://docs.fileformat.com/page-description-language/ps/)     | PostScript format                                                                  | {{< emoticons/tick >}} |
  | [XamlFixed](https://docs.fileformat.com/web/xaml/)                  | Extensible Application Markup Language (XAML) format as a fixed document           | {{< emoticons/tick >}} |
  | [XPS](https://docs.fileformat.com/page-description-language/xps/)   | XML Paper Specification document                                                   | {{< emoticons/tick >}} |

## Image formats

  | Format                                                              | Description                                                                        | Export                 |
  |---------------------------------------------------------------------|------------------------------------------------------------------------------------|------------------------|
  | [BMP](https://docs.fileformat.com/image/bmp/)                       | Bitmap image format                                                                | {{< emoticons/tick >}} |
  | [EMF](https://docs.fileformat.com/image/emf/)                       | Vector Enhanced Metafile image format                                              | {{< emoticons/tick >}} |
  | [GIF](https://docs.fileformat.com/image/gif/)                       | Graphic Interchange image format                                                   | {{< emoticons/tick >}} |
  | [JPEG](https://docs.fileformat.com/image/jpeg/)                     | Joint Photographic Experts Group image format                                      | {{< emoticons/tick >}} |
  | [PNG](https://docs.fileformat.com/image/png/)                       | Portable Network Graphic format                                                    | {{< emoticons/tick >}} |
  | [SVG](https://docs.fileformat.com/page-description-language/svg/)   | Scalar Vector Graphics format                                                      | {{< emoticons/tick >}} |
  | [TIFF](https://docs.fileformat.com/image/tiff/)                     | Single or multipage Tagged Image file format                                       | {{< emoticons/tick >}} |

