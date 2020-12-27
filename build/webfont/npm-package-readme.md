Chiron Sans HK Webfont
======================

## About

This package contains only the webfont version of [Chiron Sans HK (昭源黑體)](https://github.com/chiron-fonts/chiron-sans-hk) for adding to the web pages.

Chiron Sans HK is a CJK typeface derived from the Source Han Sans / Noto Sans CJK font family. It aims to provide a modern, region-agnostic glyph set adopting the “written” style that is similar to the prevailing, usually commercial, typefaces such that it is suitable for use in a Traditional Chinese environment.

Chiron Sans HK is available in three configurations: OpenType/CFF (OTF) version, TrueType (TTF) version, and the webfont version in WOFF File Format 2.0 (WOFF2) format.

The webfont version utilizes Unicode-range subsetting technology to reduce download size and improve loading performance. For usage example, check out the [official website (Chinese only)](https://chiron-fonts.github.io/chiron-sans-hk/).

## Usage

First, install this package:

```bash
npm install chiron-sans-hk-webfont 
```

To use this font in your web pages, import the CSS file of the desired font weights in the `css/` directory. For instance, if you use [webpack](https://webpack.js.org/), you would import the font's CSS files with the following statements (just import the weights you want to use): 

```css
@import '~chiron-sans-hk-webfont/css/ExtraLight.css';
@import '~chiron-sans-hk-webfont/css/Light.css';
@import '~chiron-sans-hk-webfont/css/Normal.css';
@import '~chiron-sans-hk-webfont/css/Regular.css';
@import '~chiron-sans-hk-webfont/css/Medium.css';
@import '~chiron-sans-hk-webfont/css/Bold.css';
@import '~chiron-sans-hk-webfont/css/Heavy.css';
```

Now you can access this font by specifying the `Chiron Sans HK WS` font family in your stylesheet. For instance:

```css
body {
    font-family: "Chiron Sans HK WS", sans-serif;
}
```

Please refer to the following table for the CSS `font-weight` values of different font weights:

| Font Weight | CSS font-weight Value |
|---|---|
| ExtraLight | 100 |
| Light | 300 |
| Normal | 400 |
| Regular | 400 |
| Medium | 500 |
| Bold | 700 |
| Heavy | 900 |

Note that the CSS font weight value of _Normal_ and _Regular_ are identical, so you can only use either one on a webpage.

## License

Chiron Sans HK is licensed under the SIL Open Font License, Version 1.1. The full text of the license is available at [https://scripts.sil.org/OFL_web](https://scripts.sil.org/OFL_web).
