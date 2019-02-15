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