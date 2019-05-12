v2.012 (2019/5/12)
==========
- Updated the design of 90 glyphs.
- U+540D 名 now using the TW glyph in Source Han Sans 1.004. 
- Mapped the glyph of Suzhou Numeral Nine U+3029 to ㄆ (Bopomofo Letter P, U+3106). I believe such form is more frequently seen in Hong Kong. 

v2.011 (2019/4/18)
==========
- **BC BREAK**: Removed numeric font weight naming because of issues on Windows.
- 46 modified glyphs has been added.
- The design of U+7B75 筵 has been updated.

v2.010 (2019/4/11)
==========
- Based on Source Han Sans 2.001.
- **BC BREAK**: Retracted the decision to incorporate a specialized version of Noto Sans into the font to simply the build process. The font is still available at https://github.com/tamcy/chiron-sans-hk-companion.
- About 400 codepoints are added, mainly for @ktshek aka @jyutnet. They are included in this build to not over complicate the build process, and to hope that they will be useful to someone else.

v2.003 (2019/2/15)
==========
- **BC BREAK**: Alphanumeric characters of the typeface are now derived from Noto Sans.
- Added 23 modified glyphs.
- Added experimental webfont.

v2.002 (2019/2/7)
==========
- A number of glyphs were found to be inadvertently removed in previous versions due to a bug in the non-local glyphs removal process. This is now fixed. As a result, previous versions are no longer considered production ready and should be avoided. 
- Fixed abnormal spacing in certain modified glyphs.
- **BC BREAK**: Font weight *ExtraLight* is now *Thin* to keep the full name of the TrueType flavour under 31 characters for better Windows (especially MS Office) compatibility.
- Added 38 modified glyphs.

~~v2.001 (2019/1/28)~~
==========
- Uses JP version of characters with 步 component.
- The glyph for U+96FB 電 is adjusted.
- Removed 'palt'/'vpal' GPOS features for full-width punctuations.
- Following codepoints are mapped to their corresponding proportional version: U+2018(‘), U+2019(’), U+201C(“) and U+201D(”).

~~v2.000 (2019/1/17, unstable)~~
==========
- Initial release.