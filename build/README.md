Installable font resources and webfont files can be found under their corresponding directories.

本目錄包含可安裝的桌面字型和網頁字型。

otf
===

This directory contains the OpenType/CFF (OTF) font resources in 7 weights.

This is the recommended configuration.

本目錄包含七個字重的 OpenType/CFF (OTF) 格式字型。

建議一般使用。

ttf
===

This directory contains the TrueType (TTF) font resources in 7 weights.

The TTF version is provided mainly for compatibility reasons. For instance, some PDF generators are unable to handle Opentype CFF font properly which result in garbled text in the generated document. Besides, 4 exceptionally tall glyphs (U+2E3A, U+2E3B, U+3031 and U+3032) have been removed. The tall glyphs leads to a large FontBBox value which can cause issues in certain applications (ref. [https://github.com/googlei18n/noto-cjk/issues/66](https://github.com/googlei18n/noto-cjk/issues/66)).

Note that TTF fonts are meant to be an interim solution to the aforementioned compatibility issues. It isn't a drop-in replacement of the OTF version. The font family name has been changed to **Chiron Sans HK TT** so that they can be installed alongside the OTF version.

本目錄包含七個字重的 TrueType (TTF) 格式字型。

主要是為遇到兼容性問題的使用者而設。例如有些 PDF 製作軟件因無法支援 Opentype CFF 格式字型導致產生出亂碼的 PDF 文件。另外，TTF 版本移除了 4 個思源黑體原有、高度超出正常中文字的字圖（兩個給U+2E3A、U+2E3B的豎排用的長破折號和兩個日語假名疊字符號U+3031及U+3032）。這些字圖令字型有較高的 FontBBox 值，某些軟件會因而出現問題 (參看 [https://github.com/googlei18n/noto-cjk/issues/66](https://github.com/googlei18n/noto-cjk/issues/66))。

留意 TTF 字型只作為遇到上述問題時的臨時解決方案，並非 OTF 版的替代品。為使 TTF 版可與 OTF 版同時安裝，TTF 版的字體名稱改為「Chiron Sans HK TT」。

webfont
=======

The `webfont` directory contains the webfont build (in `WOFF2` format) of Chiron Sans HK. Its name is **Chiron Sans HK WS**.

The webfont build includes 28,850 codepoints. All characters in the Big5 and HKSCS character sets are covered, in addition to those found in the KangXi dictionary and characters that are exclusive to written Cantonese. As the webfont targets Traditional Chinese usages, Simplified Chinese characters, Hangul etc. are NOT included.

[Unicode-range subsetting](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization#unicode-range_subsetting) is employed to improve performance. Instead of serving one single and large WOFF2 file, the font is broken into smaller pieces, resulting in around 140 tiny subset files per weight (most of them are less than 50KB). The codepoints covered by each file are defined using the `unicode-range` CSS descriptor to instruct supported browsers to only download the subset files containing codepoints that are actually used in a page. The result is a much smaller download size in general.

The subsetting strategy mostly follows Google Font’s [Noto Sans HK](https://fonts.google.com/specimen/Noto+Sans+HK), with Simplified Chinese characters excluded.

Two sets of CSS files are available, namely `[font_weight].css` and `[font_weight]_fb.css`. The one with `_fb` suffix tries to use the locally installed *Chiron Sans HK* first, with the webfont version acted as a fallback. This means no webfont downloading if the OTF version of the font is already installed on user's device. The webfont version will always be served when `[font_weight].css` is used.

For usage example, please check the HTML files named after each font weight in the `webfont` directory which prints all supported characters on a single page.

Due to the limitations of CSS support in existing browsers, the same font weight value 400 is used for both **Normal** and **Regular**. You cannot use both weights in the same page.

`webfont` 目錄內載有昭源黑體的網頁字型版 **Chiron Sans HK WS**，以 `WOFF2` 格式封裝。

網頁字型是 OTF 檔的子集版，包含 28,850 個字元，涵蓋整個 Big5/HKSCS 字集，其餘為《康熙字典》字頭、粵語專用字等。網頁字型針對繁體中文用途，沒有收錄簡體中文、諺文等文字。

為改善效能，字型採用了 [Unicode-range subsetting](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization#unicode-range_subsetting) 技術，將每個字重的單一字型檔拆分成大約 140 個細小檔案（多數檔案小於 50KB，非常用字子集小於 150KB），並在 CSS 指明該檔案所涵蓋的字碼。瀏覽器只會在網頁有用到該字碼時才會載入相關字型檔。這樣做的好處是大大減低須下載字型檔案的大小。收字方式如下：

1. 先以 Google Fonts 服務中 [Noto Sans HK](https://fonts.google.com/specimen/Noto+Sans+HK) 的拆分方式為基礎。據知 Google Fonts 在日、韓兩種語言利用了 machine learning 產生 subset，務求在最小下載檔案數之下得到最多的常用字元。雖然未知繁體中文是否也是如此，但最終應該也會用上，所以決定先跟隨 Google Fonts 的 subsetting 方法。不過，Google Fonts 的繁體子集會包含一些不在 Big5/HKSCS 的簡化字，處理時會予以過濾。
2. 本網頁字型會補上一些香港常用字符。
3. 最後，補充 Big5/HKSCS 字集和字集外、本字體有收的非常用漢字（多屬《康熙字典》字頭，也有一些粵語用字）。雖然為數不少，但由於採用了 Unicode-range subsetting，加入這些字符對一般使用者相信影響不大。

目錄內提供的 CSS 檔可分為兩種，分別是`[字重].css` 和 `[字重]_fb.css`。有 `_fb` 的版本會優先使用使用者系統中安裝的昭源黑體，假如使用者安裝了昭源黑體，就不會再下載網頁字型檔。`[字重].css` 則只會使用網頁字型。

目錄內另包含以字重命名的 HTML 檔案，會印出所有網頁字型的覆蓋字元，作為應用示範。

注意：由於目前瀏覽器的 CSS 支援所限，**Normal** 和 **Regular** 的字重數字均設定為 400，同一頁面不能同時使用這兩種字重。
