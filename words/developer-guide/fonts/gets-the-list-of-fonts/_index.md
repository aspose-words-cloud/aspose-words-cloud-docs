---
title: "Gets the List of Fonts"
second_title: "Aspose Words Cloud Docs"
type: docs
url: /fonts/gets-the-list-of-fonts/
aliases: [/gets-the-list-of-fonts/]
description: "Get a list of fonts from a Word document"
weight: 10
---

This REST API retrieves a collection of `Font` items, which consists of three groups:

- SystemFonts - Represents all TrueType fonts installed on the server.
- AdditionalFonts - Set of fonts, which have been added by the aspose team to the server additionally.
- CustomFonts - User's fonts from "fontsLocation" folder in file storage.

The API request parameters are:

|Parameter Name|HTTP Method(s)|Type|Query String/HTTPBody|Description|
| :- | :- | :- | :- | :- |
|fontsLocation|GET|string|Query String: fontsLocation=CustomFonts|A folder in file storage with custom fonts.|

and **FontInfo** properties are:

|Name|Description)|
| :- | :- |
|FontFamilyName|The family name of the font.|
|FullFontName|Full name of the font.|
|Version|Version string of the font.|
|FilePath|Path to the font file if any. It does not exist for "CustomFonts" collection.|

## Usage examples with cURL and Postman

The following URI is used to address the REST resource:

```HTML
~/fonts/available
```

You can carry out REST API interactions using `cURL` and `Postman`. Please read these <a href="/words/getting-started/quickstart/">instructions</a> to receive a personal `JWT_TOKEN` for authorization.

{{< nosnippet >}}
{{< tabs tabTotal="3" tabID="2" tabName1="cURL Request" tabName2="Postman Request" tabName3="Server Response" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "8a52e648cd36d3e0a7402727561073b6" "GetAvailableFonts.curl" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "894866974db18d27af2a7f67dd929b6f" "GetAvailableFonts.json" >}}

<p style="margin-top:-32px;font-size:80%;font-style:italic">To get a JWT token use this <a href="/words/getting-started/quickstart/">instruction</a></p>

{{< /tab >}}
{{< tab tabNum="3" >}}
```json
{
  "SystemFonts": [
    {
      "FontFamilyName": "Century Gothic",
      "FullFontName": "Century Gothic",
      "Version": "Version 2.35",
      "FilePath": "C:\\Windows\\Fonts\\11528.ttf"
    },
    {
      "FontFamilyName": "Arial Narrow",
      "FullFontName": "Arial Narrow Italic",
      "Version": "Version 2.30",
      "FilePath": "C:\\Windows\\Fonts\\Arial Narrow.ttf"
    },
    {
      "FontFamilyName": "Arial",
      "FullFontName": "Arial",
      "Version": "Version 6.90",
      "FilePath": "C:\\Windows\\Fonts\\arial.ttf"
    },
    {
      "FontFamilyName": "Arial",
      "FullFontName": "Arial Bold",
      "Version": "Version 6.90",
      "FilePath": "C:\\Windows\\Fonts\\arialbd.ttf"
    },
    {
      "FontFamilyName": "Arial",
      "FullFontName": "Arial Bold Italic",
      "Version": "Version 6.90",
      "FilePath": "C:\\Windows\\Fonts\\arialbi.ttf"
    },
    {
      "FontFamilyName": "Arial",
      "FullFontName": "Arial Italic",
      "Version": "Version 6.90",
      "FilePath": "C:\\Windows\\Fonts\\ariali.ttf"
    },
    {
      "FontFamilyName": "Arial Narrow",
      "FullFontName": "Arial Narrow",
      "Version": "Version 2.37",
      "FilePath": "C:\\Windows\\Fonts\\Arialn.ttf"
    },
    {
      "FontFamilyName": "Arial Narrow",
      "FullFontName": "Arial Narrow",
      "Version": "Version 2.30",
      "FilePath": "C:\\Windows\\Fonts\\ArialNarrow2.ttf"
    },
    {
      "FontFamilyName": "Arial Narrow",
      "FullFontName": "Arial Narrow Bold",
      "Version": "Version 1.01",
      "FilePath": "C:\\Windows\\Fonts\\ARIALNB.TTF"
    },
    {
      "FontFamilyName": "Arial Narrow",
      "FullFontName": "Arial Narrow Bold Italic",
      "Version": "Version 1.01",
      "FilePath": "C:\\Windows\\Fonts\\ARIALNBI.TTF"
    },
    {
      "FontFamilyName": "Arial Narrow",
      "FullFontName": "Arial Narrow Italic",
      "Version": "Version 2.37",
      "FilePath": "C:\\Windows\\Fonts\\ARIALNI.TTF"
    },
    {
      "FontFamilyName": "Arial Unicode MS",
      "FullFontName": "Arial Unicode MS",
      "Version": "Version 1.01",
      "FilePath": "C:\\Windows\\Fonts\\ARIALUNI.TTF"
    },
    {
      "FontFamilyName": "Arial Black",
      "FullFontName": "Arial Black",
      "Version": "Version 5.22",
      "FilePath": "C:\\Windows\\Fonts\\ariblk.ttf"
    },
    {
      "FontFamilyName": "Batang",
      "FullFontName": "Batang",
      "Version": "Version 5.00",
      "FilePath": "C:\\Windows\\Fonts\\batang.ttc"
    },
    {
      "FontFamilyName": "BatangChe",
      "FullFontName": "BatangChe",
      "Version": "Version 5.00",
      "FilePath": "C:\\Windows\\Fonts\\batang.ttc"
    },
    {
      "FontFamilyName": "Gungsuh",
      "FullFontName": "Gungsuh",
      "Version": "Version 5.00",
      "FilePath": "C:\\Windows\\Fonts\\batang.ttc"
    },
    {
      "FontFamilyName": "GungsuhChe",
      "FullFontName": "GungsuhChe",
      "Version": "Version 5.00",
      "FilePath": "C:\\Windows\\Fonts\\batang.ttc"
    },
    {
      "FontFamilyName": "Calibri",
      "FullFontName": "Calibri",
      "Version": "Version 6.18",
      "FilePath": "C:\\Windows\\Fonts\\calibri.ttf"
    },
    {
      "FontFamilyName": "Calibri",
      "FullFontName": "Calibri Bold",
      "Version": "Version 6.18",
      "FilePath": "C:\\Windows\\Fonts\\calibrib.ttf"
    },
    {
      "FontFamilyName": "Calibri",
      "FullFontName": "Calibri Italic",
      "Version": "Version 6.18",
      "FilePath": "C:\\Windows\\Fonts\\calibrii.ttf"
    },
    {
      "FontFamilyName": "Calibri Light",
      "FullFontName": "Calibri Light",
      "Version": "Version 6.18",
      "FilePath": "C:\\Windows\\Fonts\\calibril.ttf"
    },
    {
      "FontFamilyName": "Calibri Light",
      "FullFontName": "Calibri Light Italic",
      "Version": "Version 6.18",
      "FilePath": "C:\\Windows\\Fonts\\calibrili.ttf"
    },
    {
      "FontFamilyName": "Calibri",
      "FullFontName": "Calibri Bold Italic",
      "Version": "Version 6.18",
      "FilePath": "C:\\Windows\\Fonts\\calibriz.ttf"
    },
    {
      "FontFamilyName": "Cambria",
      "FullFontName": "Cambria",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\cambria.ttc"
    },
    {
      "FontFamilyName": "Cambria Math",
      "FullFontName": "Cambria Math",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\cambria.ttc"
    },
    {
      "FontFamilyName": "Comic Sans MS",
      "FullFontName": "Comic Sans MS",
      "Version": "Version 5.12",
      "FilePath": "C:\\Windows\\Fonts\\comic.ttf"
    },
    {
      "FontFamilyName": "Comic Sans MS",
      "FullFontName": "Comic Sans MS Bold",
      "Version": "Version 5.12",
      "FilePath": "C:\\Windows\\Fonts\\comicbd.ttf"
    },
    {
      "FontFamilyName": "Comic Sans MS",
      "FullFontName": "Comic Sans MS Italic",
      "Version": "Version 5.12",
      "FilePath": "C:\\Windows\\Fonts\\comici.ttf"
    },
    {
      "FontFamilyName": "Comic Sans MS",
      "FullFontName": "Comic Sans MS Bold Italic",
      "Version": "Version 5.12",
      "FilePath": "C:\\Windows\\Fonts\\comicz.ttf"
    },
    {
      "FontFamilyName": "Consolas",
      "FullFontName": "Consolas",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\consola.ttf"
    },
    {
      "FontFamilyName": "Consolas",
      "FullFontName": "Consolas Bold",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\consolab.ttf"
    },
    {
      "FontFamilyName": "Consolas",
      "FullFontName": "Consolas Italic",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\consolai.ttf"
    },
    {
      "FontFamilyName": "Consolas",
      "FullFontName": "Consolas Bold Italic",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\consolaz.ttf"
    },
    {
      "FontFamilyName": "Courier New",
      "FullFontName": "Courier New",
      "Version": "Version 6.90",
      "FilePath": "C:\\Windows\\Fonts\\cour.ttf"
    },
    {
      "FontFamilyName": "Courier New",
      "FullFontName": "Courier New Bold",
      "Version": "Version 6.90",
      "FilePath": "C:\\Windows\\Fonts\\courbd.ttf"
    },
    {
      "FontFamilyName": "Courier New",
      "FullFontName": "Courier New Bold Italic",
      "Version": "Version 6.90",
      "FilePath": "C:\\Windows\\Fonts\\courbi.ttf"
    },
    {
      "FontFamilyName": "Courier New",
      "FullFontName": "Courier New Italic",
      "Version": "Version 6.90",
      "FilePath": "C:\\Windows\\Fonts\\couri.ttf"
    },
    {
      "FontFamilyName": "Ebrima",
      "FullFontName": "Ebrima",
      "Version": "Version 5.11",
      "FilePath": "C:\\Windows\\Fonts\\ebrima.ttf"
    },
    {
      "FontFamilyName": "Ebrima",
      "FullFontName": "Ebrima Bold",
      "Version": "Version 5.11",
      "FilePath": "C:\\Windows\\Fonts\\ebrimabd.ttf"
    },
    {
      "FontFamilyName": "Freestyle Script",
      "FullFontName": "Freestyle Script",
      "Version": "Version 1.05",
      "FilePath": "C:\\Windows\\Fonts\\FREESCPT.TTF"
    },
    {
      "FontFamilyName": "Gadugi",
      "FullFontName": "Gadugi",
      "Version": "Version 1.10",
      "FilePath": "C:\\Windows\\Fonts\\gadugi.ttf"
    },
    {
      "FontFamilyName": "Garamond",
      "FullFontName": "Garamond",
      "Version": "Version 2.20",
      "FilePath": "C:\\Windows\\Fonts\\Garamond.ttf"
    },
    {
      "FontFamilyName": "Georgia",
      "FullFontName": "Georgia",
      "Version": "Version 5.58",
      "FilePath": "C:\\Windows\\Fonts\\georgia.ttf"
    },
    {
      "FontFamilyName": "Georgia",
      "FullFontName": "Georgia Bold",
      "Version": "Version 5.58",
      "FilePath": "C:\\Windows\\Fonts\\georgiab.ttf"
    },
    {
      "FontFamilyName": "Georgia",
      "FullFontName": "Georgia Italic",
      "Version": "Version 5.58",
      "FilePath": "C:\\Windows\\Fonts\\georgiai.ttf"
    },
    {
      "FontFamilyName": "Georgia",
      "FullFontName": "Georgia Bold Italic",
      "Version": "Version 5.58",
      "FilePath": "C:\\Windows\\Fonts\\georgiaz.ttf"
    },
    {
      "FontFamilyName": "Gulim",
      "FullFontName": "Gulim",
      "Version": "Version 5.02",
      "FilePath": "C:\\Windows\\Fonts\\gulim.ttc"
    },
    {
      "FontFamilyName": "GulimChe",
      "FullFontName": "GulimChe",
      "Version": "Version 5.02",
      "FilePath": "C:\\Windows\\Fonts\\gulim.ttc"
    },
    {
      "FontFamilyName": "Dotum",
      "FullFontName": "Dotum",
      "Version": "Version 5.02",
      "FilePath": "C:\\Windows\\Fonts\\gulim.ttc"
    },
    {
      "FontFamilyName": "DotumChe",
      "FullFontName": "DotumChe",
      "Version": "Version 5.02",
      "FilePath": "C:\\Windows\\Fonts\\gulim.ttc"
    },
    {
      "FontFamilyName": "Microsoft Himalaya",
      "FullFontName": "Microsoft Himalaya",
      "Version": "Version 5.22",
      "FilePath": "C:\\Windows\\Fonts\\himalaya.ttf"
    },
    {
      "FontFamilyName": "Edwardian Script ITC",
      "FullFontName": "Edwardian Script ITC",
      "Version": "Version 1.05",
      "FilePath": "C:\\Windows\\Fonts\\ITCEDSCR.TTF"
    },
    {
      "FontFamilyName": "Javanese Text",
      "FullFontName": "Javanese Text",
      "Version": "Version 1.07",
      "FilePath": "C:\\Windows\\Fonts\\javatext.ttf"
    },
    {
      "FontFamilyName": "Leelawadee UI",
      "FullFontName": "Leelawadee UI Bold",
      "Version": "Version 5.05",
      "FilePath": "C:\\Windows\\Fonts\\LeelaUIb.ttf"
    },
    {
      "FontFamilyName": "Leelawadee UI",
      "FullFontName": "Leelawadee UI",
      "Version": "Version 5.05",
      "FilePath": "C:\\Windows\\Fonts\\LeelawUI.ttf"
    },
    {
      "FontFamilyName": "Leelawadee UI Semilight",
      "FullFontName": "Leelawadee UI Semilight",
      "Version": "Version 5.05",
      "FilePath": "C:\\Windows\\Fonts\\LeelUIsl.ttf"
    },
    {
      "FontFamilyName": "Lucida Console",
      "FullFontName": "Lucida Console",
      "Version": "Version 5.00",
      "FilePath": "C:\\Windows\\Fonts\\lucon.ttf"
    },
    {
      "FontFamilyName": "Malgun Gothic",
      "FullFontName": "Malgun Gothic",
      "Version": "Version 6.67",
      "FilePath": "C:\\Windows\\Fonts\\malgun.ttf"
    },
    {
      "FontFamilyName": "Myanmar Text",
      "FullFontName": "Myanmar Text",
      "Version": "Version 1.15",
      "FilePath": "C:\\Windows\\Fonts\\mmrtext.ttf"
    },
    {
      "FontFamilyName": "Mongolian Baiti",
      "FullFontName": "Mongolian Baiti",
      "Version": "Version 5.52",
      "FilePath": "C:\\Windows\\Fonts\\monbaiti.ttf"
    },
    {
      "FontFamilyName": "Microsoft JhengHei",
      "FullFontName": "Microsoft JhengHei",
      "Version": "Version 6.13",
      "FilePath": "C:\\Windows\\Fonts\\msjh.ttc"
    },
    {
      "FontFamilyName": "Microsoft JhengHei UI",
      "FullFontName": "Microsoft JhengHei UI",
      "Version": "Version 6.13",
      "FilePath": "C:\\Windows\\Fonts\\msjh.ttc"
    },
    {
      "FontFamilyName": "Microsoft YaHei",
      "FullFontName": "Microsoft YaHei",
      "Version": "Version 6.22",
      "FilePath": "C:\\Windows\\Fonts\\msyh.ttc"
    },
    {
      "FontFamilyName": "Microsoft YaHei UI",
      "FullFontName": "Microsoft YaHei UI",
      "Version": "Version 6.22",
      "FilePath": "C:\\Windows\\Fonts\\msyh.ttc"
    },
    {
      "FontFamilyName": "Microsoft Yi Baiti",
      "FullFontName": "Microsoft Yi Baiti",
      "Version": "Version 5.99",
      "FilePath": "C:\\Windows\\Fonts\\msyi.ttf"
    },
    {
      "FontFamilyName": "MV Boli",
      "FullFontName": "MV Boli",
      "Version": "Version 6.84",
      "FilePath": "C:\\Windows\\Fonts\\mvboli.ttf"
    },
    {
      "FontFamilyName": "Nirmala UI",
      "FullFontName": "Nirmala UI",
      "Version": "Version 1.34",
      "FilePath": "C:\\Windows\\Fonts\\Nirmala.ttf"
    },
    {
      "FontFamilyName": "Nirmala UI",
      "FullFontName": "Nirmala UI Bold",
      "Version": "Version 1.34",
      "FilePath": "C:\\Windows\\Fonts\\NirmalaB.ttf"
    },
    {
      "FontFamilyName": "Nirmala UI Semilight",
      "FullFontName": "Nirmala UI Semilight",
      "Version": "Version 1.34",
      "FilePath": "C:\\Windows\\Fonts\\NirmalaS.ttf"
    },
    {
      "FontFamilyName": "Microsoft New Tai Lue",
      "FullFontName": "Microsoft New Tai Lue",
      "Version": "Version 5.98",
      "FilePath": "C:\\Windows\\Fonts\\ntailu.ttf"
    },
    {
      "FontFamilyName": "Microsoft PhagsPa",
      "FullFontName": "Microsoft PhagsPa",
      "Version": "Version 5.99",
      "FilePath": "C:\\Windows\\Fonts\\phagspa.ttf"
    },
    {
      "FontFamilyName": "Segoe MDL2 Assets",
      "FullFontName": "Segoe MDL2 Assets",
      "Version": "Version 1.55",
      "FilePath": "C:\\Windows\\Fonts\\segmdl2.ttf"
    },
    {
      "FontFamilyName": "Segoe Print",
      "FullFontName": "Segoe Print",
      "Version": "Version 5.02",
      "FilePath": "C:\\Windows\\Fonts\\segoepr.ttf"
    },
    {
      "FontFamilyName": "Segoe UI",
      "FullFontName": "Segoe UI",
      "Version": "Version 5.53",
      "FilePath": "C:\\Windows\\Fonts\\segoeui.ttf"
    },
    {
      "FontFamilyName": "Segoe UI",
      "FullFontName": "Segoe UI Bold",
      "Version": "Version 5.53",
      "FilePath": "C:\\Windows\\Fonts\\segoeuib.ttf"
    },
    {
      "FontFamilyName": "Segoe UI",
      "FullFontName": "Segoe UI Italic",
      "Version": "Version 5.29",
      "FilePath": "C:\\Windows\\Fonts\\segoeuii.ttf"
    },
    {
      "FontFamilyName": "Segoe UI Light",
      "FullFontName": "Segoe UI Light",
      "Version": "Version 5.53",
      "FilePath": "C:\\Windows\\Fonts\\segoeuil.ttf"
    },
    {
      "FontFamilyName": "Segoe UI Semilight",
      "FullFontName": "Segoe UI Semilight",
      "Version": "Version 5.53",
      "FilePath": "C:\\Windows\\Fonts\\segoeuisl.ttf"
    },
    {
      "FontFamilyName": "Segoe UI",
      "FullFontName": "Segoe UI Bold Italic",
      "Version": "Version 5.29",
      "FilePath": "C:\\Windows\\Fonts\\segoeuiz.ttf"
    },
    {
      "FontFamilyName": "Segoe UI Black",
      "FullFontName": "Segoe UI Black",
      "Version": "Version 2.00",
      "FilePath": "C:\\Windows\\Fonts\\seguibl.ttf"
    },
    {
      "FontFamilyName": "Segoe UI Emoji",
      "FullFontName": "Segoe UI Emoji",
      "Version": "Version 1.11",
      "FilePath": "C:\\Windows\\Fonts\\seguiemj.ttf"
    },
    {
      "FontFamilyName": "Segoe UI Historic",
      "FullFontName": "Segoe UI Historic",
      "Version": "Version 1.01",
      "FilePath": "C:\\Windows\\Fonts\\seguihis.ttf"
    },
    {
      "FontFamilyName": "Segoe UI Semibold",
      "FullFontName": "Segoe UI Semibold",
      "Version": "Version 5.53",
      "FilePath": "C:\\Windows\\Fonts\\seguisb.ttf"
    },
    {
      "FontFamilyName": "Segoe UI Symbol",
      "FullFontName": "Segoe UI Symbol",
      "Version": "Version 6.22",
      "FilePath": "C:\\Windows\\Fonts\\seguisym.ttf"
    },
    {
      "FontFamilyName": "SimSun",
      "FullFontName": "SimSun",
      "Version": "Version 5.15",
      "FilePath": "C:\\Windows\\Fonts\\simsun.ttc"
    },
    {
      "FontFamilyName": "NSimSun",
      "FullFontName": "NSimSun",
      "Version": "Version 5.15",
      "FilePath": "C:\\Windows\\Fonts\\simsun.ttc"
    },
    {
      "FontFamilyName": "Source Code Pro Black",
      "FullFontName": "Source Code Pro Black",
      "Version": "Version 2.010;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-Black.otf"
    },
    {
      "FontFamilyName": "Source Code Pro Black",
      "FullFontName": "Source Code Pro Black Italic",
      "Version": "Version 1.030;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-BlackIt.otf"
    },
    {
      "FontFamilyName": "Source Code Pro",
      "FullFontName": "Source Code Pro Bold",
      "Version": "Version 2.010;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-Bold.otf"
    },
    {
      "FontFamilyName": "Source Code Pro",
      "FullFontName": "Source Code Pro Bold Italic",
      "Version": "Version 1.030;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-BoldIt.otf"
    },
    {
      "FontFamilyName": "Source Code Pro ExtraLight",
      "FullFontName": "Source Code Pro ExtraLight",
      "Version": "Version 2.010;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-ExtraLight.otf"
    },
    {
      "FontFamilyName": "Source Code Pro ExtraLight",
      "FullFontName": "Source Code Pro ExtraLight Italic",
      "Version": "Version 1.030;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-ExtraLightIt.otf"
    },
    {
      "FontFamilyName": "Source Code Pro",
      "FullFontName": "Source Code Pro Italic",
      "Version": "Version 1.030;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-It.otf"
    },
    {
      "FontFamilyName": "Source Code Pro Light",
      "FullFontName": "Source Code Pro Light",
      "Version": "Version 2.010;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-Light.otf"
    },
    {
      "FontFamilyName": "Source Code Pro Light",
      "FullFontName": "Source Code Pro Light Italic",
      "Version": "Version 1.030;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-LightIt.otf"
    },
    {
      "FontFamilyName": "Source Code Pro Medium",
      "FullFontName": "Source Code Pro Medium",
      "Version": "Version 2.010;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-Medium.otf"
    },
    {
      "FontFamilyName": "Source Code Pro Medium",
      "FullFontName": "Source Code Pro Medium Italic",
      "Version": "Version 1.030;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-MediumIt.otf"
    },
    {
      "FontFamilyName": "Source Code Pro",
      "FullFontName": "Source Code Pro",
      "Version": "Version 2.010;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-Regular.otf"
    },
    {
      "FontFamilyName": "Source Code Pro Semibold",
      "FullFontName": "Source Code Pro Semibold",
      "Version": "Version 2.010;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-Semibold.otf"
    },
    {
      "FontFamilyName": "Source Code Pro Semibold",
      "FullFontName": "Source Code Pro Semibold Italic",
      "Version": "Version 1.030;PS 1.0;hotconv 1.0.84;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceCodePro-SemiboldIt.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro Black",
      "FullFontName": "Source Sans Pro Black",
      "Version": "Version 2.020;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-Black.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro Black",
      "FullFontName": "Source Sans Pro Black Italic",
      "Version": "Version 1.075;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-BlackIt.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro",
      "FullFontName": "Source Sans Pro Bold",
      "Version": "Version 2.020;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-Bold.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro",
      "FullFontName": "Source Sans Pro Bold Italic",
      "Version": "Version 1.075;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-BoldIt.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro ExtraLight",
      "FullFontName": "Source Sans Pro ExtraLight",
      "Version": "Version 2.020;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-ExtraLight.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro ExtraLight",
      "FullFontName": "Source Sans Pro ExtraLight Italic",
      "Version": "Version 1.075;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-ExtraLightIt.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro",
      "FullFontName": "Source Sans Pro Italic",
      "Version": "Version 1.075;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-It.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro Light",
      "FullFontName": "Source Sans Pro Light",
      "Version": "Version 2.020;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-Light.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro Light",
      "FullFontName": "Source Sans Pro Light Italic",
      "Version": "Version 1.075;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-LightIt.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro",
      "FullFontName": "Source Sans Pro",
      "Version": "Version 2.020;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-Regular.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro Semibold",
      "FullFontName": "Source Sans Pro Semibold",
      "Version": "Version 2.020;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-Semibold.otf"
    },
    {
      "FontFamilyName": "Source Sans Pro Semibold",
      "FullFontName": "Source Sans Pro Semibold Italic",
      "Version": "Version 1.075;PS 2.0;hotconv 1.0.86;makeotf.lib2.5.63406",
      "FilePath": "C:\\Windows\\Fonts\\SourceSansPro-SemiboldIt.otf"
    },
    {
      "FontFamilyName": "Symbol",
      "FullFontName": "Symbol",
      "Version": "Version 5.01",
      "FilePath": "C:\\Windows\\Fonts\\symbol.ttf"
    },
    {
      "FontFamilyName": "Microsoft Tai Le",
      "FullFontName": "Microsoft Tai Le",
      "Version": "Version 5.98",
      "FilePath": "C:\\Windows\\Fonts\\taile.ttf"
    },
    {
      "FontFamilyName": "Times New Roman",
      "FullFontName": "Times New Roman",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\times.ttf"
    },
    {
      "FontFamilyName": "Times New Roman",
      "FullFontName": "Times New Roman Bold",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\timesbd.ttf"
    },
    {
      "FontFamilyName": "Times New Roman",
      "FullFontName": "Times New Roman Bold Italic",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\timesbi.ttf"
    },
    {
      "FontFamilyName": "Times New Roman",
      "FullFontName": "Times New Roman Italic",
      "Version": "Version 6.96",
      "FilePath": "C:\\Windows\\Fonts\\timesi.ttf"
    },
    {
      "FontFamilyName": "Trebuchet MS",
      "FullFontName": "Trebuchet MS",
      "Version": "Version 5.14",
      "FilePath": "C:\\Windows\\Fonts\\trebuc.ttf"
    },
    {
      "FontFamilyName": "Trebuchet MS",
      "FullFontName": "Trebuchet MS Bold",
      "Version": "Version 5.14",
      "FilePath": "C:\\Windows\\Fonts\\trebucbd.ttf"
    },
    {
      "FontFamilyName": "Trebuchet MS",
      "FullFontName": "Trebuchet MS Bold Italic",
      "Version": "Version 5.14",
      "FilePath": "C:\\Windows\\Fonts\\trebucbi.ttf"
    },
    {
      "FontFamilyName": "Trebuchet MS",
      "FullFontName": "Trebuchet MS Italic",
      "Version": "Version 5.14",
      "FilePath": "C:\\Windows\\Fonts\\trebucit.ttf"
    },
    {
      "FontFamilyName": "Verdana",
      "FullFontName": "Verdana",
      "Version": "Version 5.32",
      "FilePath": "C:\\Windows\\Fonts\\verdana.ttf"
    },
    {
      "FontFamilyName": "Verdana",
      "FullFontName": "Verdana Bold",
      "Version": "Version 5.32",
      "FilePath": "C:\\Windows\\Fonts\\verdanab.ttf"
    },
    {
      "FontFamilyName": "Verdana",
      "FullFontName": "Verdana Italic",
      "Version": "Version 5.32",
      "FilePath": "C:\\Windows\\Fonts\\verdanai.ttf"
    },
    {
      "FontFamilyName": "Verdana",
      "FullFontName": "Verdana Bold Italic",
      "Version": "Version 5.32",
      "FilePath": "C:\\Windows\\Fonts\\verdanaz.ttf"
    },
    {
      "FontFamilyName": "Webdings",
      "FullFontName": "Webdings",
      "Version": "Version 5.00",
      "FilePath": "C:\\Windows\\Fonts\\webdings.ttf"
    },
    {
      "FontFamilyName": "Wingdings",
      "FullFontName": "Wingdings",
      "Version": "Version 5.00",
      "FilePath": "C:\\Windows\\Fonts\\wingding.ttf"
    },
    {
      "FontFamilyName": "Wingdings 3",
      "FullFontName": "Wingdings 3",
      "Version": "Version 1.50",
      "FilePath": "C:\\Windows\\Fonts\\Wingdings3.ttf"
    },
    {
      "FontFamilyName": "Yu Gothic Medium",
      "FullFontName": "Yu Gothic Medium",
      "Version": "Version 1.73",
      "FilePath": "C:\\Windows\\Fonts\\YuGothM.ttc"
    },
    {
      "FontFamilyName": "Yu Gothic UI",
      "FullFontName": "Yu Gothic UI Regular",
      "Version": "Version 1.73",
      "FilePath": "C:\\Windows\\Fonts\\YuGothM.ttc"
    }
  ],
  "AdditionalFonts": null,
  "CustomFonts": null,
  "Code": 200,
  "Status": "OK"
}
```
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}

## Aspose.Words Cloud SDK Family

Using SDK is the best way to speed up the development. Please go to the [GitHub](https://github.com/aspose-words-cloud) repository to explore a wide family of our Cloud SDKs. These powerful libraries take care of all low-level programming details and let you focus on your primary tasks.

## Usage examples in Python, Java, C#, etc.

The following code samples show how to interact with REST API using almost any mainstream programming language. You can find a lot of other code examples in [Python](https://gist.github.com/aspose-words-cloud-gists/e26813ced70692c544820cd8011ee7e0), [Java](https://gist.github.com/aspose-words-cloud-gists/caede439bfd2e57c3010befe504faff4), [C#](https://gist.github.com/aspose-words-cloud-gists/374e1e3dd4bca8f696f29d913645f549), [JavaScript](https://gist.github.com/aspose-words-cloud-gists/a9510e4b51613f1138e7c1ec09634c4a), [PHP](https://gist.github.com/aspose-words-cloud-gists/e2a72445b96362dc0117f06ab54bb94a), [C++](https://gist.github.com/aspose-words-cloud-gists/49aa5151a094849179bae8672c887a0e), [Golang](https://gist.github.com/aspose-words-cloud-gists/625ca80adffd779e8f6e3611551e14d5), [Ruby](https://gist.github.com/aspose-words-cloud-gists/339f3835a4c0a536c81ec941de29baf7), [Swift](https://gist.github.com/aspose-words-cloud-gists/790dbd2edd5d36f170732366f52cac4c), [Dart](https://gist.github.com/aspose-words-cloud-gists/6aae628cf2b878b78fea177c3171c6bf) on GitHub. All codes are thoroughly tested and ready for production use.

{{< nosnippet >}}
{{< tabs tabTotal="11" tabID="5" tabName1="Python" tabName2="Java" tabName3="Node.js" tabName4="C#" tabName5="PHP" tabName6="C++" tabName7="Go" tabName8="Ruby" tabName9="Swift" tabName10="Dart" tabName11="Curl" >}}
{{< tab tabNum="1" >}}
{{< gist "aspose-words-cloud-gists" "e26813ced70692c544820cd8011ee7e0" "GetAvailableFonts.py" >}}
{{< /tab >}}
{{< tab tabNum="2" >}}
{{< gist "aspose-words-cloud-gists" "caede439bfd2e57c3010befe504faff4" "GetAvailableFonts.java" >}}
{{< /tab >}}
{{< tab tabNum="3" >}}
{{< gist "aspose-words-cloud-gists" "a9510e4b51613f1138e7c1ec09634c4a" "GetAvailableFonts.js" >}}
{{< /tab >}}
{{< tab tabNum="4" >}}
{{< gist "aspose-words-cloud-gists" "374e1e3dd4bca8f696f29d913645f549" "GetAvailableFonts.cs" >}}
{{< /tab >}}
{{< tab tabNum="5" >}}
{{< gist "aspose-words-cloud-gists" "e2a72445b96362dc0117f06ab54bb94a" "GetAvailableFonts.php" >}}
{{< /tab >}}
{{< tab tabNum="6" >}}
{{< gist "aspose-words-cloud-gists" "49aa5151a094849179bae8672c887a0e" "GetAvailableFonts.cpp" >}}
{{< /tab >}}
{{< tab tabNum="7" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "config.json" >}}
{{< gist "aspose-words-cloud-gists" "625ca80adffd779e8f6e3611551e14d5" "GetAvailableFonts.go" >}}
{{< /tab >}}
{{< tab tabNum="8" >}}
{{< gist "aspose-words-cloud-gists" "339f3835a4c0a536c81ec941de29baf7" "GetAvailableFonts.rb" >}}
{{< /tab >}}
{{< tab tabNum="9" >}}
{{< gist "aspose-words-cloud-gists" "790dbd2edd5d36f170732366f52cac4c" "GetAvailableFonts.swift" >}}
{{< /tab >}}
{{< tab tabNum="10" >}}
{{< gist "aspose-words-cloud-gists" "6aae628cf2b878b78fea177c3171c6bf" "GetAvailableFonts.dart" >}}
{{< /tab >}}
{{< /tabs >}}
{{< /nosnippet >}}
