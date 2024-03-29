v2.046 (2022/01/11)
====
- 重繪「辦」字字圖。
- 更新 palt/vpal 指令字元清單，以下字元（及其對應直書形式，如有的話）會被移除，使排版時不會出現壓縮全形標點符號所導致的半字寬情況：（）〔〕「」『』，。、！？．〈〉《》［］【】 (Fixes #24)。

v2.045 (2021/10/02)
====
- 部份字圖及對映更新。

v2.044 (2021/08/30)
====
- 修正以下字元之字圖：莂 (U+8382)，蟉 (U+87C9)，鍃 (U+9343)，鏠 (U+93E0)，鑱 (U+9471)，饝 (U+995D)，䘵 (U+4635)，䱚 (U+4C5A)，哵 (U+54F5)，寥 (U+5BE5)。
- 重繪及更改對映逾 100 字碼/字圖，主要屬含「大」或「禾」在底部（如莫、奐，包括央、矢、奏、癸、秦）而末筆讓作點的字，改從捺。

v2.043 (2021/08/07)
====
- 修正簝 (U+7C1D) 字字寬。
- 更新及新增字圖。

v2.042 (2021/06/29)
====
- 細微更新（修改及新增一些字圖）。

v2.041 (2021/05/27)
====
- 網頁字型 Webfont 補回英文單引號字元 (U+2018 ‘，U+2019 ’)。
- 將下列「康熙部首」區 (U+2F00-U+2FDF) 字元對映至本字體所屬意式樣：U+2F10 ⼐，U+2F50 ⽐，U+2F78 ⽸，U+2FAC ⾬，U+2FBF ⾿，U+2FC5 ⿅，U+2FC9 ⿉，U+2FD2 ⿒。
- 昭源黑體的常用字元已經符合本字體的設計方針，由 v2.040 版開始，更新紀錄檔（本檔案）不會再逐一列出非常用字元的字圖修改。欲知各版本的重繪字元數變更，請參考 `meta.json`。

v2.040 (2021/04/29)
====
- 上游版本更新至思源黑體 2.004 版。修正了可變式字型 OTF 字重名稱顯示不正確的問題。
- 上一版本錯誤移除了瓊 (U+74CA) 的字形修復變更，本版已改正。

v2.035 (2021/04/15)
====
- 上游版本更新至思源黑體 2.003 版。本版思源黑體由於新增可變式字型格式支援，製作流程有所更改，所以中間字重 (Light, Normal, Regular, Medium, Bold) 的字圖大小跟前版略有分別。
- 新增可變式字型 (Variable Font, VF)，字型名稱是 Chiron Sans HK VF。
- 網頁字型改用可變式字型格式，一個檔案有齊所有字重，並可任意指定字重值。字重值跟隨思源黑體作出調整。另外移除了優先使用系統字體的 CSS 檔案。
- 增加以下 20 字的修改字圖：㔆㚬㶴㷇䓎䖅奿娛媁嫾岺撍栾焲熩爤豅𢲷𨥉𪊲。

備註：思源黑體 v2.003 的 VF 格式有幾個已知問題，這些問題亦會出現在昭源黑體 VF。我最後仍決定推出配置 VF 格式的昭源黑體新版，因為我認為 VF 版網頁字型非常值得更新，假如只提供網頁用的可變式字型卻不提供桌面版本又會顯得奇怪，於是最後還是將桌面版 OpenType/CFF2 可變式字型收入。

v2.034 (2021/03/18)
====
- 將瓊 (U+74CA) 對映到 JP 源異體字以修正字形筆畫。
- 增加以下 7 字的修改字圖：幠菕鑗鑶龲𨰣𩸽。
- 以下 38 字改用思源第一版字圖：吙嗧埮悐晱栺梑瀱炋烒烳焟焨焺焻煂煔煰熁熂熼燆燨爅爏爧竼笁笚笝龦𠐔𠴲𢅺𤅗𧅥𩡗𩸭。
- 現時大部份瀏覽器已容許 `font-weight` 指定任何 1-1000 以內的數值，因此將網頁字型 Normal 字重的 `font-weight` 值改為 370，以避免跟 Regular 重疊。

v2.033 (2021/02/28)
====
- 調整「譽」字字形。
- 修正「糀」字字形。
- 增加以下 4 字的修改字圖：㴆㸒婬霪。

v2.032 (2021/01/30)
====
- 修正「鵳」字對映。
- 修正「𥹉」字字形。
- 增加以下 10 字的修改字圖：釨釮釴鉘銆鏍鏎鏔鏕鐉。
- 以下符號改為預設輸出與中文字（而非英文）對齊的版本：U+2E3A（⸺）、U+2E3B（⸻）、U+203C（‼）、U+2047（⁇）、U+2048（⁈）、U+2049（⁉）。

v2.031 (2020/11/30)
====
- 增加以下 102 字的修改字圖：
    - 23 個參部件字：剼參墋嵾幓慘摻槮毿滲磣穇篸糝縿蔘襂贂鏒驂鬖鰺黲。
    - 6 個缶部件字（底部改為齊腳）：窑窰繇罄罋颻。
    - 5 個養部件字：懩攁瀁癢養。
    - 其他，共 68 個：䚗姹𠵈𡡅毼煐熥熸燵爉筶篚膍䴇蕶虂惀睔蜦彾昤朎狑秢駖魿梌溆蒢鵌睮羭腧褕貐蚙鯩祄菳鈖鈗鉖鉡鉾鋑錂錆鍄鍈鍏鍗鎄鎕鏧鏱㸆巆烻焢煄煼熳爞磱𤎌𤒹峠糀。

v2.030 (2020/11/16)
====
- 修正：2.029 版 TTF 格式字型上游版本並未正確更新至思源黑體 2.002 版。
- 修正：2.029 版不慎錯誤移除「徹轍底」三字之修改字圖。
- 增加以下 10 字的修改字圖：凼密岙峊窋蔤𩓥𪘁𪘲𪙛（底部改為齊腳）。

v2.029 (2020/11/15)
====
- 上游版本更新至思源黑體 2.002 版。
- 移除「準」字修改字圖（上游版本已修正）。
- 以下 18 字改用 J 源：齒齓齕齗齘齚齞齟齠齣齧齪齫齬齮齯齰齺（改用底部齊腳字形）。
- 增加以下 25 字的修改字圖：㟻冚函喦岔峹嶞嶨巒幽菡齔齖齙齛齜齝齡齦齩齱齲齵齶齷（底部改為齊腳）。

v2.028 (2020/10/13)
====
- 改善以下 4 字造型：準徹轍底。本屬思源黑體更新範疇，由於原字體更新情況未明，暫於本字體先行處理。

v2.027 (2020/8/1)
====
- 修正「驟」字對映（之前錯誤對映至 C 源）。由於正確字圖（T 源）質素欠佳，因此改用修改版本。
- 以下 11 字改用 J 源：劚囑墀屬斸樨爥犀矚穉钃（中間「氺」形狀部件改用橫筆版本）。
- 增加以下 26 字的修改字圖：䙱䠱噑孎徲摨曍橰欘灟獋獔翶翺蠾遲𡲬㜳壞懷櫰瀤瓌蘹蘾褱（中間「氺」形狀部件改用橫筆版本）。

v2.026 (2020/7/13)
====
- 增加以下 38 字的修改字圖：棜爗癟篲簆籑膰膴臕芘芮苶蕧薿藇藨談閼馤鬠鷋麌齘龤䤬䥇䥈䬪䬳䬴䭅䭣鋵飤飿餁餄餏。
- 增收「U+301DB 𰇛 (⿰口伏)」字，位於中日韓統一表意文字擴展區 (CJK Unified Ideographs Extension) G。象聲詞，在漫畫較常見到。

v2.025 (2020/5/10)
====
- 增加以下 38 字的修改字圖：㖸㗘㘛㜮㤉㧁㨑㪐㽎䁯䃗䇶䖙䠡䢍䢢䯋吂塠揬桊炣烌眡砛肨胮胿膁膎膭𠹷𡢃𤉙𤌍𥔱𦻐𨃩。

v2.024 (2020/3/23)
====
- 增加以下 105
  字的修改字圖：㜲㟷㯓侌傛僇剳剹勠唂嘐噙容岒岭峪崐崘嵊嵱嵺帢廕廥怜憀搿摎柃榕樛歙渰溚溶漻潝灜熔瑢璆瓴疁瘳癊磟祫禴穋竛紒紾綌翏胣腳艅芃葊蓉蓼袗袷裕褡襘詅谹谼谾谿豁豂蹘蹹郤鄝酴醩醼醽鍳鐪闟鞈鞥鞳韐飂餦餴饆饠駗驘髎鰫鴒鷚𠸐𠹸𠹹𡆇𦖿𨀣。
- 以下 5 字改用台灣源：羸臝蠃贏鸁。

v2.023 (2020/3/13)
====
- 增加以下 78 字的修改字圖：㝎䍇偝僗匳妎姙姼媕媖媮媱嫛嫳嬐孏寥崟嶮廖戮扲揄梣檎瀏烴焌煒煺爁爟爣爦爨牏獳礝繆膝膠臙薟藜蘞蘦蟉襝謬踰轇醪鉠鉧銎鎏鏊鏖鑌钁隁隃霒霡霫霮霿靀骽麂黐鼹齌𢫏𤃬𩁹𩃬𩅰。
- 思源黑體 2.001 版包含 4 個位於中日韓統一表意文字擴展區 G、但因當時尚未定案而沒有為之編碼的字形。在思源黑體中，這些字元須透過 IDS (Ideographic Description Sequences) 加上
  OpenType 的 ccmp 功能取得。隨着 Unicode 13.0 於 2020/3/10 發表、這 4 字正式獲得 Unicode 碼位，因此將以下 4 字編碼：U+3106C 𱁬 (CID+61861)、U+30729
  𰜩 (CID+61858)、U+30EDD 𰻝 (CID+61859)、U+30EDE 𰻞 (CID+61857)。將此 4
  字編碼的動作顯然應該在思源黑體進行，所以這項更新本非昭源字體事務（而是等待思源黑體更新、再在本字體引入）。只是基於近月思源黑體開發方 Adobe
  的人事變動，思源字體後續開發尚未明朗，因此暫在本字體處理（之前修正某些屬思源黑體原版的字形錯誤也是這個原因）。

v2.022 (2020/2/24)
==========
- 增收「U+210AB 𡂫 (⿰口蓬)」字，位於中日韓統一表意文字擴展區 (CJK Unified Ideographs Extension) B。
- 微調「U+6C0F 氏」的位置。
- 增加以下 4 字的修改字圖：蓬縫釯銻。蓬、縫二字將夂部件末筆由頓點改為捺，以增強本字體同部件字（如篷、𡂫）的一致性。釯、銻之前對映至日本版字形（取其「金」部件設計），但其實兩字日本版字形的右偏旁並不符本字體選定標準。
- 增加以下 24 字的修改字圖：㩋嘯奫婣橚櫹歗淵潚瀟熽璛簫繡肅蕭蠨鏽驌鱐鷫鼘𤄙𤑳。主要是修改「𣶒」部件的寫法，以香港寫法為基礎但「片」首筆作撇。

v2.021 (2020/1/27)
==========
- 增加以下 9 字的修改字圖：劉擀芩蠄覦鈶鏗飡𤏲。
- 增收「𫬷 (U+2BB37，⿰口騎)」字，位於中日韓統一表意文字擴展區 (CJK Unified Ideographs Extension) E。
- 網頁字型改用 Google Fonts 中的香港版字型 Noto Sans HK 為製作子集之藍本（之前使用的是台灣版 Noto Sans TC）。

v2.020 (2020/1/22)
==========
- 增加以下 262
  字的修改字圖：䤼䥥䬬凎姸娽峇崙崯廞烚焓煍煏燏燐燠爌箜箠箬篋篱篳篴篼簉簙簨簻籈籊籙籝籩蝓衿郪釢釫釺釾鈃鈆鈑鈒鈚鈜鉌鉔鉥鉫銋銍銨銱銾鋄鋊鋐鋘鋝鋣鋩鋬鋮鋶錁錄錈錛錞錥錧錴錵鍁鍃鍇鍐鍔鍖鍟鍤鍦鍧鍭鍮鍰鎉鎒鎛鎡鎪鎯鎲鎷鎸鏂鏇鏏鏐鏓鏚鏠鏬鏮鏰鏵鏺鐀鐋鐎鐏鐓鐕鐖鐝鐥鐩鐭鐯鐻鑊鑐鑒鑔鑞鑢鑤鑨鑮鑱鑴鑵鑹鑾鑿钀钂钃顉飈飥飦飫飵飶飺餂餈餎餐餑餔餕餗餙餜餟餩餪餫餭餱餲餳餷餹餺餻餼饀饁饃饇饊饍饎饐饔饗饘饙饛饜饝饟饡饢𠸎𡅈𢴈𤆣𤏸𤗈𤸻𤺥𥮉𥰡𥲤𥶙𦸅𨧜𨫼𨭌𨯩𨰉㵦㷭㺖䃮䆃䆳䇷䈥䉷䊚䌥䎭䗬䘵䚢䚦䢜䢩䩮䭔䭤䯌䯞䯢䱚䲎䵍䵎旤曃櫎莂觵过还迩迯选逎逓逥逩逫逬逰遀遅遟遱邌餶饏鬇鱑。

v2.019 (2019/12/29)
==========
- 修改以下 27 個含「人」部件字：呤唥囹搇泠舲蛉衾鈪錭鎞鎩鎬鎰鏙鏞鏹鏻鏾鐫鐶陰飣餖餮饕𡃶。
- 修改「𥱊 (U+25C4A)」字字形。
- 增收「𭉝 (U+2D25D，⿰口殊)」字。此字常見於香港粵語書刊，卻要到 2017 年才在 Unicode 10.0 獲收入中日韓統一表意文字擴展區F (CJK Unified Ideographs Extension F)
  ，亦未見收入香港字符集，因此思源黑體並未包含。
- 網頁字型追加六千多個不屬 Big5 或 HKSCS、位於 CJK Ext-A 和 Ext-B 的漢字（多屬《康熙字典》字頭）。

v2.018 (2019/12/16)
==========
- 修正「脂 (U+8102)、腹 (U+8179)」二字字形。
- 「纊 (U+7E8A)」字改回使用香港源（之前錯誤對映至日本源）。

v2.017 (2019/8/2)
==========
- 修正「翁」錯誤對映至韓國版字形的問題。
- 修改「諮」字字形。
- 增加 9 個金部件字「鉚鉞銕銙鋂鋋鋌鍵鏤」的修改字圖。

v2.016 (2019/7/7)
==========
- 增加以下 5 字的修改字圖，繼續增加「人」部件字的一致性：銹鋃鎚𩜠𩟔。
- 承上，增加以下 51 字的修改字圖，涉及元素週期表中的「金」部件字：䥑釕釹鈁鈈鈧鈰鉕鉝鉬鉭鉲鉳鉺銣銥銦銩銪鋦鋯鋱錇錒錸錼鍀鍅鍆鍩鍺鎇鎝鎦鎵鎶鎿鏌鐒鐠鐦鐨鐽鐿鑀鑥鑪𨧀𨨏𨭆𨭎。
- 修改「芒」字字形：改善原版設計問題。
- 修改「𤺧」字字形：此字本來使用思源黑體第一版字形，惟此版字形之設計有誤，今據第二版字圖手動修改。

v2.015 (2019/6/26)
==========
- 增加以下 8 字的修改字圖，繼續增加「人」部件字的一致性：喰鈽鉈鉸銃鋹鎘鐧。
- 更新到 (U+5230) 的字形。
- 更新 Webfont 的 Unicode-range subsetting 策略，以最新的 Noto Sans TC 版本為基礎。

v2.014 (2019/6/15)
==========
- 增加以下 64 字的修改字圖，繼續增加「人」部件字的一致性：㗳䱽令伶俞偷冷啥喻嗒噏塔岑嶺愈拎搭擒於樖淤渝瀚玲瑜疥疹瘀瘉瘡瘩癐癒禽給繪羚翎翕翰聆胗腍膾臉舘艙芥苓荅菸薈診諗諭軨逾鑛領飧飱骱齡龕𢲡。
- 修正銳 (U+92B3) 的字形。
- 更新哋 (U+54CB) 的字形。

v2.013 (2019/5/28)
==========
- 增加以下 96 字的修改字圖：奠煪燇盦笭荼蒼蔭酏酓醌醐醟鈍鈎鈞鈣鈴鉛銀銬銳銷鋅鋼錐錕錘錚錠錨錶鍍鍛鍥鎅鎊鎔鎢鎮鎳鏃鏈鏑鏟鏡鏽鐘鐮鐵鑠鑣鑲鑼鑽靆飩餛餬饞綸蝕論鉉食飢飪飭飯飲飴飼飽飾餃餅餉餌餓餘餚餞餡館餵餸餽餾餿饅饈饉饋饌饑饒。
- 思源黑體將「人」部件兩畫起筆是否相連視為「日韓」和「中港台」的地區標準差異：「日韓」相連，「中港台」則否。本字體則視為設計差異，並以日韓款式（兩畫起筆相連者）為首選。不過，常用字中「食」、「金」部件在左時若出現不同設計會比較顯眼。這次更新，將「食」、「金」部件在左、但因為標準問題而必須使用「中港台」字樣的常用字改為日韓款式，以減少同部件常用字出現的設計不一致情況。

v2.012 (2019/5/12)
==========
- 增加以下 90 字的修改字圖：㙎㜈㜜侫僽喴奼妗姎娏娵娷婈婓婤婼媌媙媥媶媷媺媻媿嫕嫚嫟嫫嫭嫹嬞嬥嬾孈峖𠴕揠揻攍敥椻楲氀灱灴炄炓炩烅烆烇烎烢煘熚犩瓾窶羰翣耬膢舕艛苂荌菨菼萩葌蒘蕠薅薠藀蘡蘮蘶蝛褗覣躽郾隇餒餤餧鰋鶈鷜。 「名 (
  U+540D)」改用舊版台灣版的字形。
- 將「Suzhou Numeral Nine U+3029」的字形映射到「ㄆ (Bopomofo Letter P, U+3106)」。

v2.011 (2019/4/18)
==========
- 取消為字重加上數字的做法，原因是此舉在 Windows 的支援性不佳，例如會有在記事本一類字型選擇對話方塊無法正確將字型歸納為同一家族、Regular 和 Bold 字重有時會出現混亂（明明選擇 Regular
  卻會變成粗體、安裝時系統誤認 Bold 為 Regular 字重然後詢問是否覆蓋）等。為免煩擾，決定放棄這個修改，將字重名稱回復與思源黑體保持一致。
- 增加 46 字的修改版字圖以符合本字體風格，包括「匽妠妦妴姈姖姾崴懲擫煟煸熪猏琵笀筑箎篪篫簪籔籚籧籯葫葳葹葽蒆蓖蔊蔞蕓薷蝘邐酯醭雵霙鶠鼴」43 字及 3 個含「茶」部件字「茶嗏搽」。
- 更新「筵」的修改版字圖以符合思源黑體 2.001 版的廴部件設計。

v2.010 (2019/4/11)
==========
- 基於思源黑體 2.001 版製作，當中修正了思源黑體 2.000 版的若干問題。
