Installable font resources and webfont files can be found in their corresponding directories.

本目錄包含可安裝的桌面字型和網頁字型。

otf
===

This directory contains the OpenType/CFF (OTF) font resources in seven weights.

The font family name for this configuration is **Chiron Sans HK**. This is the recommended configuration.

本目錄包含七個字重的 OpenType/CFF (OTF) 格式字型。

安裝後的字型名稱是 **Chiron Sans HK**。建議一般使用。

variable
========

This directory contains the OpenType/CFF2 (OTF) variable font resource. Instead of choosing from seven static instances, users can now select a font weight at any point between the ExtraLight and Heavy instances in supported applications.

The font family name for this configuration is **Chiron Sans HK VF**. 

Note that this configuration requires a system and/or application that supports OpenType/CFF2 variable font format.

本目錄包含 OpenType/CFF2 (OTF) 可變式字型 (Variable Font)。跟 OTF 版本分成七個固定字重不同，可變字型將所有字重收入一個檔案，使用者可透過應用程式的字重軸任意揀選 ExtraLight 和 Heavy 之間的字重值。

安裝後的字體名稱是 **Chiron Sans HK VF**。

留意必須在支援可變式字型的作業系統或應用程式中使用。

ttf
===

This directory contains the TrueType (TTF) font resources in seven weights.

The TTF version is provided for applications with compatibility issues with the OTF format. Some PDF generators are unable to handle Opentype CFF font properly which result in garbled text in the generated document. Besides, four exceptionally tall glyphs (U+2E3A, U+2E3B, U+3031 and U+3032) have been removed in this build since they lead to a large FontBBox value which can cause problems in certain applications (ref. [https://github.com/googlei18n/noto-cjk/issues/66](https://github.com/googlei18n/noto-cjk/issues/66)).

Note that TTF fonts are meant to be an interim solution to the aforementioned compatibility issues. It is not a drop-in replacement of the OTF version. Its font family name has been changed to **Chiron Sans HK TT** so that they can be installed alongside the OTF version.

本目錄包含七個字重的 TrueType (TTF) 格式字型。

主要是為遇到兼容性問題的使用者而設。例如有些 PDF 製作軟件因無法支援 Opentype CFF 格式字型導致產生出亂碼的 PDF 文件。另外，TTF 版本移除了 4 個思源黑體原有、高度超出正常中文字的字圖（兩個給 U+2E3A、U+2E3B 的豎排用的長破折號和兩個日語假名疊字符號U+3031 及 U+3032）。這些字圖令字型有較高的 FontBBox 值，某些軟件會因而出現問題 (參看 [https://github.com/googlei18n/noto-cjk/issues/66](https://github.com/googlei18n/noto-cjk/issues/66))。

留意 TTF 字型只作為遇到上述問題時的臨時解決方案，並非 OTF 版的替代品。為使 TTF 版可與 OTF 版同時安裝，TTF 版的字體名稱改為「Chiron Sans HK TT」。

webfont
=======

The `webfont` directory contains the webfont build (in `WOFF2` format) of Chiron Sans HK VF. The family name of this configuration is **Chiron Sans HK WS**. To start using it, copy the `webfont/css` and `webfont/woff2` directories to your project location and include the corresponding CSS file. The webfont build is now available in variable font format, so you just need to include a single CSS file to access all possible font weights.

This webfont is a subsetted version of the original OTF configuration. It covers all characters in the Big5 and HKSCS character sets. In addition, characters that are found in the KangXi dictionary and exclusive to written Cantonese are included. As the webfont targets Traditional Chinese usages, Simplified Chinese characters, Hangul etc. are excluded from the build.

The webfont is optimized with [Unicode-range subsetting](https://web.dev/reduce-webfont-size/#unicode-range-subsetting). The font is broken into smaller pieces, resulting in around 140 tiny subset files per weight. Instead of downloading one single and large font file, the browser only needs to download the subset files that contain the glyphs required for rendering the text on a page.

The subsetting strategy mostly follows the one employed by Google Font's [Noto Sans HK](https://fonts.google.com/specimen/Noto+Sans+HK), with Simplified Chinese characters excluded.

For usage example, please check the HTML file in the `webfont/demo` directory which prints all supported characters on a single page.

`webfont` 目錄內載有昭源黑體的網頁字型版 **Chiron Sans HK WS**，以 `WOFF2` 格式封裝。將 `webfont/css` 和 `webfont/woff2` 目錄複裝到你的專案位置然後載入相關的 CSS 檔就即可使用。網頁字型以「可變式字型」格式提供，只須載入一個 CSS 檔案就可以用到全部字重。

網頁字型是 OTF 檔的子集版，涵蓋整個 Big5/HKSCS 字集，其餘為《康熙字典》字頭、粵語專用字等。網頁字型針對繁體中文用途，沒有收錄簡體中文、諺文等文字。

為改善效能，字型採用了 [Unicode-range subsetting](https://web.dev/reduce-webfont-size/#unicode-range-subsetting) 技術，將每個字重的單一字型檔拆分成大約 140 個細小檔案（多數檔案小於 50KB，非常用字子集小於 150KB），並在 CSS 指明該檔案所涵蓋的字碼。瀏覽器只會在網頁有用到該字碼時才會載入相關字型檔。這樣做的好處是大大減低須下載字型檔案的大小。收字方式如下：

1. 先以 Google Fonts 服務中 [Noto Sans HK](https://fonts.google.com/specimen/Noto+Sans+HK) 的拆分方式為基礎。據知 Google Fonts 在日、韓兩種語言利用了 machine learning 產生 subset，務求在最小下載檔案數之下得到最多的常用字元。雖然未知繁體中文是否也是如此，但最終應該也會用上，所以決定先跟隨 Google Fonts 的 subsetting 方法。不過，Google Fonts 的繁體子集會包含一些不在 Big5/HKSCS 的簡化字，處理時會予以過濾。
2. 本網頁字型會補上一些香港常用字符。
3. 最後，補充 Big5/HKSCS 字集和字集外、本字體有收的非常用漢字（多屬《康熙字典》字頭，也有一些粵語用字）。雖然為數不少，但由於採用了 Unicode-range subsetting，加入這些字符對一般使用者相信影響不大。

`webfont/demo` 目錄內包含一 HTML 檔，會印出所有網頁字型的覆蓋字元，作為應用示範。
