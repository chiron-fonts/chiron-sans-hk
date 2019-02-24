Installable font resources and webfont files can be found here.

本目錄包含可安裝的桌面字型和網頁字型。

otf
===

Contains OpenType/CFF (OTF) font resources in 7 weights.

This is the recommended configuration.

包含七個字重的 OpenType/CFF (OTF) 格式字型。

建議一般使用。

ttf
===

Contains TrueType (TTF) font resources in 7 weights.

This is provided mainly for compatibility reasons. For instance, some PDF generators are unable to handle Opentype CFF font properly which result in garbled text in the generated document. In addition, 4 exceptionally tall glyphs (U+2E3A, U+2E3B, U+3031 and U+3032) from the original Source Han Sans font have been removed from this configuration. The tall glyphs leads to a large FontBBox value which are causing issues in certain applications (ref. [https://github.com/googlei18n/noto-cjk/issues/66](https://github.com/googlei18n/noto-cjk/issues/66)).

Note that TTF fonts are served as an interim solution to the aforementioned compatibility issues, but not a drop-in replacement of the OTF fonts. The font family name has been changed to **Chiron Sans HK TT** so that they can be installed alongside the OTF version.

包含七個字重的 TrueType (TTF) 格式字型。

主要是為遇到兼容性問題的使用者而設。例如有些 PDF 製作軟件因無法支援 Opentype CFF 格式字型導致產生出亂碼的 PDF 文件。另外，TTF 版本移除了 4 個思源黑體原有、高度超出正常中文字的字圖（兩個給U+2E3A、U+2E3B的豎排用的長破折號和兩個日語假名疊字符號U+3031及U+3032）。這些字圖令字型有較高的 FontBBox 值，某些軟件會因而出現問題 (參看 [https://github.com/googlei18n/noto-cjk/issues/66](https://github.com/googlei18n/noto-cjk/issues/66))。

留意 TTF 字型只作為遇到上述問題時的臨時解決方案，並非 OTF 版的替代品。為使 TTF 版可與 OTF 版同時安裝，TTF 版的字體名稱改為「Chiron Sans HK TT」。

webfont
=======


The `webfont` directory contains a *preview* of the webfont **Chiron Sans HK WS** packaged in `WOFF2` format.

The font is a subset of the OTF version which contains around 14,584 codepoints. The scope of the webfont version is limited to commonly-used characters in Big5 and HKSCS (although it isn't exactly the case for now due to the subsetting strategy, see below).

[Unicode-range subsetting](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization#unicode-range_subsetting) is used to improve performance. Instead of serving a single WOFF2 file, the font is further broken into smaller pieces, resulting in more than 100 tiny font files per weight (most of them are less than 50KB). Codepoints covered by each file are defined using the `unicode-range` CSS descriptor, and supported browsers are smart enough to only download the subset files containing codepoints that are actually used in a page. The benefit is a much smaller download size in general.

The subsetting strategy follows Google Font’s [Noto Sans TC](https://fonts.google.com/specimen/Noto+Sans+TC). This causes a number of Simplified Chinese characters being included, but are left as-is for now. Additional characters deemed useful for Hong Kong are also included.

Two sets of CSS files are available, namely `[font_weight].css` and `[font_weight]_fb.css`. The one with `_fb` suffix tries to use the locally installed *Chiron Sans HK* first, with the webfont version acted as a fallback. This means no webfont downloading if the OTF version of the font is already installed on user's device. On the other hand, `[font_weight].css` always serves the webfont version to the users.

For usage example, please check the HTML files named after each font weight which prints all supported characters on a single page in the directory.

`webfont` 目錄內的是網頁字型 **Chiron Sans HK WS** 的預覽版本，以 `WOFF2` 格式封裝。

網頁字型收錄 20,105 個字元，包含整個 Big5/HKSCS 字集。

為改善效能，字型採用了 Unicode-range subsetting 技術，將每個字重的單一字型檔拆分成超過 100 個細小檔案（大多數檔案小於 50KB，非常用字子集小於 150KB），並在 CSS 指明該檔案所涵蓋的字碼。瀏覽器只會在網頁有用到該字碼時，才會載入相關的字型檔。這樣做的好處是大大減低須下載字型檔案的大小。收字方式如下：

1. 先以 Google Fonts 服務中 [Noto Sans TC](https://fonts.google.com/specimen/Noto+Sans+TC) 的拆分方式為基礎。目前 Google Fonts 在日、韓兩種語言利用了 machine learning 產生 subset，務求在最小下載檔案數之下得到最多的常用字元。雖然未知繁體中文是否也是如此，但最終應該也會用上，所以決定先跟隨 Google Fonts 的 subsetting 方法。不過，Google Fonts 的繁體子集會包含一些不在 Big5/HKSCS 的簡化字，處理時會予以過濾。
2. Google Fonts 的子集缺少很多香港常用字（例如此issue：https://github.com/google/fonts/issues/396）。本 webfont 會補上香港常用字符。
3. 最後，補充 Big5/HKSCS 字集內的非常用字。既然已採用 unicode-range subsetting，加入這些字符對一般使用應無大影響。

目錄內提供兩組 CSS 檔，分別是`[字重].css` 和 `[字重]_fb.css`。有 `_fb` 的版本會優先使用使用者系統中安裝的昭源黑體，Webfont 則作為 fallback 使用。假如使用者安裝了昭源黑體，就不會再下載 Webfont 檔。`[字重].css` 則只會使用 webfont 版本。

目錄內另包含以字重命名的 HTML 檔案，會印出所有 Webfont 覆蓋字元，作為應用示範。
