Chiron Sans HK Webfont
======================

## About

This package contains the webfont version of [Chiron Sans HK (昭源黑體)](https://github.com/chiron-fonts/chiron-sans-hk) for using in websites.

Chiron Sans HK is a CJK typeface derived from the Source Han Sans / Noto Sans CJK font family. It aims to provide a modern, region-agnostic glyph set adopting the “written” style that is similar to the prevailing, usually commercial, typefaces such that it is suitable for use in a Traditional Chinese environment.

Chiron Sans HK is available in four configurations: OpenType/CFF (OTF), OpenType/CFF2 (OTF) Variable Font, TrueType (TTF), and the webfont version in WOFF File Format 2.0 (WOFF2) variable font format.

The webfont version utilizes Unicode-range subsetting technology to reduce download size and improve loading performance. For usage example, check out the [official website (Chinese only)](https://chiron-fonts.github.io/chiron-sans-hk/).

## Usage

First, install this package:

```bash
npm install chiron-sans-hk-webfont 
```

Include the `css/vf.css` file in your web pages to start using it. For instance, if you use [webpack](https://webpack.js.org/), you would import the font's CSS file with the following statement: 

```css
@import '~chiron-sans-hk-webfont/css/all.css';
```

Now you can access this font by specifying the `Chiron Sans HK WS` font family in your stylesheet. For instance:

```css
body {
    font-family: "Chiron Sans HK WS", sans-serif;
}
```

Refer to the following table for the corresponding CSS `font-weight` values of the default static font weights. As this is a variable font, you can also specify any value between 250 and 900 to the `font-weight` attribute.

| Font Weight | CSS font-weight Value |
|---|---|
| ExtraLight | 250 |
| Light | 300 |
| Normal | 350 |
| Regular | 400 |
| Medium | 500 |
| Bold | 700 |
| Heavy | 900 |

## License

Chiron Sans HK is licensed under the SIL Open Font License, Version 1.1. The full text of the license is available at [https://scripts.sil.org/OFL_web](https://scripts.sil.org/OFL_web).
