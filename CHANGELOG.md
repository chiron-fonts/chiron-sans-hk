v2.018 (2019/12/16)
==========
- Corrected the design of U+8102 脂 and U+8179 腹.
- Corrected the mapping of 纊 (JP → HK).

v2.017 (2019/8/2)
==========
- Updated the design of the following 9 characters: 鉚鉞銕銙鋂鋋鋌鍵鏤.
- Enhanced existing design of 諮.
- Fixed incorrect mapping of 翁.

v2.016 (2019/7/7)
==========
- Updated the design of the following 5 characters: 銹鋃鎚𩜠𩟔.
- Updated the design of the following 51 characters: 䥑釕釹鈁鈈鈧鈰鉕鉝鉬鉭鉲鉳鉺銣銥銦銩銪鋦鋯鋱錇錒錸錼鍀鍅鍆鍩鍺鎇鎝鎦鎵鎶鎿鏌鐒鐠鐦鐨鐽鐿鑀鑥鑪𨧀𨨏𨭆𨭎.
- Enhanced existing design of 芒 and 𤺧.

v2.015 (2019/6/26)
==========
- Updated the design of U+55B0 喰, U+923D 鈽, U+9248 鉈, U+9278 鉸, U+9283 銃, U+92F9 鋹, U+9398 鎘 and U+9427 鐧.
- Unicode-range subsetting strategy of Webfont build is now based on the latest version of Noto Sans TC. 

v2.014 (2019/6/15)
==========
- Modified the design of 64 additional glyphs.
- Updated the design of U+54CB 哋. 
- Fixed the design of U+92B3 銳.

v2.013 (2019/5/28)
==========
- Modified the design of 96 additional glyphs.

v2.012 (2019/5/12)
==========
- Modified the design of 90 additional glyphs.
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