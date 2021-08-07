v2.043 (2021/08/07)
====
- Fixed the glyph width of 簝 (U+7C1D).
- Updated and added some glyphs.

v2.042 (2021/06/29)
====
- Maintenance release (updated and added some glyphs).

v2.041 (2021/05/27)
====
- Added single quotes characters (U+2018 ‘, U+2019 ’) to the webfont build.
- Remapped the following characters in the Kangxi Radicals block (U+2F00 - U+2FDF) to the font's preferred form: U+2F10 ⼐, U+2F50 ⽐, U+2F78 ⽸, U+2FAC ⾬, U+2FBF ⾿, U+2FC5 ⿅, U+2FC9 ⿉, U+2FD2 ⿒.
- All daily used characters should now adhere to the font's preferred form. Starting from v2.040, redesigned characters that are not frequently used will not be explicitly mentioned in the changelog (this file). Please consult `meta.json` for the redesigned character count of each release.

v2.040 (2021/04/29)
====
- Upstream version updated to Source Han Sans 2.004. Fixed instance names not showing correctly in variable OTF.
- Restored the design fix of 瓊 (U+74CA). The fix was inadvertently reverted in the previous version.

v2.035 (2021/04/15)
====
- Upstream version updated to Source Han Sans 2.003. Notice: the scale of glyphs in the intermediate weights (Light, Normal, Regular, Medium, Bold) has been adjusted slightly because of the building pipeline change in Source Han Sans to support the new variable font format.
- Added a new variable font (VF) configuration. The font name for this configuration is **Chiron Sans HK VF**.
- The web font configuration is now in variable font format. All weights are contained in a single file. It is now possible for designers to specify arbitrary font weight values. The font weight numbers have been adjusted to match Source Han Sans VF. Finally, the CSS files which local installed font resources take precedence are now removed.
- Redesigned the following 20 characters: 㔆㚬㶴㷇䓎䖅奿娛媁嫾岺撍栾焲熩爤豅𢲷𨥉𪊲.

Remarks: There are a few known issues in the VF version of Source Han Sans v2.003 which also affects Chiron Sans HK VF. I decided to roll a new release that includes the VF variant because I believe the webfont VF configuration is a worthy update. It feels strange when a release only contains a WOFF2 VF but no desktop version, so a desktop OpenType/CFF2 variable font is also included anyway.


v2.034 (2021/03/17)
====
- Fixed the design of 瓊 (U+74CA), it is now mapped to the alternate JP glyph.
- Redesigned the following 7 characters: 幠菕鑗鑶龲𨰣𩸽.
- The following 38 characters are now using the design in Source Han Sans V1: 吙嗧埮悐晱栺梑瀱炋烒烳焟焨焺焻煂煔煰熁熂熼燆燨爅爏爧竼笁笚笝龦𠐔𠴲𢅺𤅗𧅥𩡗𩸭.
- As most browsers now support the latest `font-weight` syntax which allows arbitrary numeric `font-weight` value between 1 and 1000, the `font-weight` value for Normal in the webfont build is changed to 370.  

v2.033 (2021/02/28)
====
- Tweaked the design of 譽.
- Fixed the design of 糀.
- Redesigned the following 4 characters: 㴆㸒婬霪.

v2.032 (2021/01/30)
====
- Corrected the mapping of 鵳.
- Corrected the shape of 𥹉.
- Redesigned the following 10 characters: 釨釮釴鉘銆鏍鏎鏔鏕鐉.
- Set the em-box aligned version of the following characters to be the default: U+2E3A (⸺), U+2E3B (⸻), U+203C (‼), U+2047 (⁇), U+2048 (⁈), and U+2049 (⁉).

v2.031 (2020/11/30)
====
- Redesigned the following 102 characters: 剼參墋嵾幓慘摻槮毿滲磣穇篸糝縿蔘襂贂鏒驂鬖鰺黲窑窰繇罄罋颻懩攁瀁癢養䚗姹𠵈𡡅毼煐熥熸燵爉筶篚膍䴇蕶虂惀睔蜦彾昤朎狑秢駖魿梌溆蒢鵌睮羭腧褕貐蚙鯩祄菳鈖鈗鉖鉡鉾鋑錂錆鍄鍈鍏鍗鎄鎕鏧鏱㸆巆烻焢煄煼熳爞磱𤎌𤒹峠糀.

v2.030 (2020/11/16)
====
- Fix: upstream of TTF version not correctly updated to Source Han Sans 2.002 in v2.029.
- Fix: enhanced design of 徹轍底 mistakenly removed in v2.029.
- Redesigned the following 10 characters: 凼密岙峊窋蔤𩓥𪘁𪘲𪙛.

v2.029 (2020/11/15)
====
- Upstream version updated to Source Han Sans 2.002.
- Removed the redesign glyph of 準 - the upstream version can now be used.
- Remapped the following 18 characters to J source: 齒齓齕齗齘齚齞齟齠齣齧齪齫齬齮齯齰齺.
- Redesigned the following 25 characters: 㟻冚函喦岔峹嶞嶨巒幽菡齔齖齙齛齜齝齡齦齩齱齲齵齶齷.

v2.028 (2020/10/13)
====
- Enhanced the design of the following 4 characters: 準徹轍底.

v2.027 (2020/8/1)
====
- Redesigned 驟. This character has been incorrectly remapped to C source, and the correct T/H source is of subpar quality.
- Remapped the following 11 characters to J source: 劚囑墀屬斸樨爥犀矚穉钃.
- Redesigned the following 26 characters: 䙱䠱噑孎徲摨曍橰欘灟獋獔翶翺蠾遲𡲬㜳壞懷櫰瀤瓌蘹蘾褱.

v2.026 (2020/7/13)
====
- Redesigned the following 38 characters: 棜爗癟篲簆籑膰膴臕芘芮苶蕧薿藇藨談閼馤鬠鷋麌齘龤䤬䥇䥈䬪䬳䬴䭅䭣鋵飤飿餁餄餏.
- Added U+301DB 𰇛 (⿰口伏).

v2.025 (2020/5/10)
====
- Redesigned the following 38 characters: 㖸㗘㘛㜮㤉㧁㨑㪐㽎䁯䃗䇶䖙䠡䢍䢢䯋吂塠揬桊炣烌眡砛肨胮胿膁膎膭𠹷𡢃𤉙𤌍𥔱𦻐𨃩.

v2.024 (2020/3/23)
====
- Redesigned the following 105 characters: 㜲㟷㯓侌傛僇剳剹勠唂嘐噙容岒岭峪崐崘嵊嵱嵺帢廕廥怜憀搿摎柃榕樛歙渰溚溶漻潝灜熔瑢璆瓴疁瘳癊磟祫禴穋竛紒紾綌翏胣腳艅芃葊蓉蓼袗袷裕褡襘詅谹谼谾谿豁豂蹘蹹郤鄝酴醩醼醽鍳鐪闟鞈鞥鞳韐飂餦餴饆饠駗驘髎鰫鴒鷚𠸐𠹸𠹹𡆇𦖿𨀣.
- Remapped the following 5 characters to the TW version: 羸臝蠃贏鸁.

v2.023 (2020/3/13)
====
- Redesigned the following 78 characters: 㝎䍇偝僗匳妎姙姼媕媖媮媱嫛嫳嬐孏寥崟嶮廖戮扲揄梣檎瀏烴焌煒煺爁爟爣爦爨牏獳礝繆膝膠臙薟藜蘞蘦蟉襝謬踰轇醪鉠鉧銎鎏鏊鏖鑌钁隁隃霒霡霫霮霿靀骽麂黐鼹齌𢫏𤃬𩁹𩃬𩅰.
- Unicode 13.0 was released in 2020/3/10. As the status of the upstream is undetermined, I decided to encode the following CJK Unified Ideographs Extension G characters in Chiron Sans HK: U+3106C 𱁬 (CID+61861), U+30729 𰜩 (CID+61858), U+30EDD 𰻝 (CID+61859) and U+30EDE 𰻞 (CID+61857).

v2.022 (2020/2/24)
==========
- Added U+210AB 𡂫 (⿰口蓬).
- Adjusted the position of U+6C0F 氏.
- Redesigned the following 4 characters: 蓬縫釯銻.
- Redesigned the following 24 characters: 㩋嘯奫婣橚櫹歗淵潚瀟熽璛簫繡肅蕭蠨鏽驌鱐鷫鼘𤄙𤑳.

v2.021 (2020/1/27)
==========
- Redesigned the following 9 characters: 劉擀芩蠄覦鈶鏗飡𤏲.
- Added U+2BB37 𫬷 (⿰口騎). 
- The webfont build now follows Google Font Noto Sans HK's latest (v5) Unicode-range subsetting strategy.

v2.020 (2020/1/22)
==========
- Redesigned the following 262 characters: 䤼䥥䬬凎姸娽峇崙崯廞烚焓煍煏燏燐燠爌箜箠箬篋篱篳篴篼簉簙簨簻籈籊籙籝籩蝓衿郪釢釫釺釾鈃鈆鈑鈒鈚鈜鉌鉔鉥鉫銋銍銨銱銾鋄鋊鋐鋘鋝鋣鋩鋬鋮鋶錁錄錈錛錞錥錧錴錵鍁鍃鍇鍐鍔鍖鍟鍤鍦鍧鍭鍮鍰鎉鎒鎛鎡鎪鎯鎲鎷鎸鏂鏇鏏鏐鏓鏚鏠鏬鏮鏰鏵鏺鐀鐋鐎鐏鐓鐕鐖鐝鐥鐩鐭鐯鐻鑊鑐鑒鑔鑞鑢鑤鑨鑮鑱鑴鑵鑹鑾鑿钀钂钃顉飈飥飦飫飵飶飺餂餈餎餐餑餔餕餗餙餜餟餩餪餫餭餱餲餳餷餹餺餻餼饀饁饃饇饊饍饎饐饔饗饘饙饛饜饝饟饡饢𠸎𡅈𢴈𤆣𤏸𤗈𤸻𤺥𥮉𥰡𥲤𥶙𦸅𨧜𨫼𨭌𨯩𨰉㵦㷭㺖䃮䆃䆳䇷䈥䉷䊚䌥䎭䗬䘵䚢䚦䢜䢩䩮䭔䭤䯌䯞䯢䱚䲎䵍䵎旤曃櫎莂觵过还迩迯选逎逓逥逩逫逬逰遀遅遟遱邌餶饏鬇鱑.

v2.019 (2019/12/29)
==========
- Updated the design of the following 27 characters: 呤唥囹搇泠舲蛉衾鈪錭鎞鎩鎬鎰鏙鏞鏹鏻鏾鐫鐶陰飣餖餮饕𡃶.
- Redesigned U+25C4A 𥱊.
- Added U+2D25D 𭉝 (⿰口殊).
- Added >6,000 characters in CJK Ext-A and Ext-B to the webfont build.

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
- **BC BREAK**: Retracted the decision to incorporate a specialized version of Noto Sans into the font to simplify the build process. The font is still available at https://github.com/tamcy/chiron-sans-hk-companion.
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
