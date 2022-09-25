﻿# **Python 太乙神數 Kintaiyi 堅太乙 年計 月計 日計 時計**
[![Python](https://img.shields.io/pypi/pyversions/kintaiyi)](https://pypi.org/project/kintaiyi/)
[![PIP](https://img.shields.io/pypi/v/kintaiyi)](https://pypi.org/project/kintaiyi/)
[![Downloads](https://img.shields.io/pypi/dm/kintaiyi)](https://pypi.org/project/kintaiyi/)
[![TG](https://img.shields.io/badge/chat-on%20telegram-blue)](https://t.me/gnatnek)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/kinyeah)&nbsp;

![alt text](https://github.com/kentang2017/kintaiyi/blob/master/pic/64459296_2342412609170469_2685042927293431808_n.jpg "太乙")
 ## 1. 導讀 Introduction
太乙神數是古代漢族占卜術的一種，與遁甲，六壬合稱三式，是推算天時以及歷史變化規律的術數學。周武王時以術數"卜世三十，卜年八百"推之，至邵雍形成歷史哲學而大備。據太乙神數推算，上古時有一年冬至日半夜，恰好日月合璧、五星連珠，定為甲子年、甲子月、甲子日、甲子時，稱作太極上元，上元甲子以來的年數，叫太乙積年。由太乙積年再求出太乙流年和太歲值卦，以斷本年各月的氣運凶吉，預測一些重大政治事件和天災人禍。採用五元六紀，三百六十年為一大周期，七十二年為一小周期，太乙每宮居三年，不入中宮，二十四年轉一周，七十二年遊三期。

太乙以一為太極生二目(主、客目)，二目生主客大小客與計神共八將。太乙乃天地之神，其星在太乙之前，統十六神而知風雨、水旱、兵革之事。昔黃帝與蚩尤大戰，適逢大霧，以霧書昏風後相，造指南車克之，是以取太乙之法，傳至今三千餘年，例目以為術數。外閱龍圖，內演龜文，凡天地之所以設君臣父子，之所以立陰陽，太乙了然演數則理昭著，太乙周行流運六十四卦，貴神入門十精之星，使經緯錯縮表理，集為一書。延續至今三千餘年不衰，為當今社會預測、決斷，提供了寶貴依據。

相傳太乙式產生于黃帝戰蚩尤時。其法大扺本于《易緯.乾鑿度》太乙行九宮法。採用五元六紀，三百六十年為一大周期，七十二年為一小周期，太乙每宮居三年，不入中宮，二十四年轉一周，七十二年遊三期。太乙以一為太極生二目(主、客目)，二目生主客大小客與計神共八將。(與易經太極分二儀，二儀生四象，四象生八卦相仿)。以太乙八將所乘十六神之方位關系定出格局。可佔內外祝福。又臨四時之分野，可佔水旱疾疫。再推三基五福大小遊二限，可預測古今治亂。又可推出年卦、月卦等。

Taiyishenshu, one of the Ancient Chinese Divinations, along with Qimendunjia and Dailiuren known as "three styles".


## 2. 安裝套件 Installation
```python
	pip install kintaiyi
	pip install --upgrade sxtwl, numpy, ephem, cn2an 
```
## 3. 起課方式 Quickstart
```python
	from kintaiyi import kintaiyi
	# 0 為年計；1 為月計；2 為日計：3 為時計
	#公元前
	Taiyi(-202,9,16,23,14).pan(1)
	{'太乙計': '月計', '公元日期': '-202年9月16日23時', '干支': ['戊戌', '辛酉', '庚戌', '丙子'], '農曆': {'年': -202, '月': 8, '日': 15}, '年號': '西漢高帝劉邦 高帝四年', '紀元': '第三紀第一甲子元', '時局': {'文': '陽遁十局', '數': 10}, '太乙': 4, '文昌': '丑', '太歲': '子', '合神': '丑', '計神': '寅', '始擊': '子', '定目': '子', '主算': [4, ['無天', '無地', '雜陽']], '客算': [11, ['無地', '陰中重陽']], '定算': [11, ['無地', '陰中重陽']], '九宮': {8: '大游', 3: '客參定參', 4: '主將太乙', 9: '', 5: '五風', 2: '主參八風', 7: '三風', 6: '', 1: '客將定將飛鳥小游'}, '十六宮': {'子': ['太歲', '始擊', '定目'], '丑': ['文昌', '合神', '四神'], '艮': [], '寅': [], '卯': [], '辰': ['君基'], '巽': ['五福'], '巳': ['民基'], '午': ['飛符', '太尊'], '未': ['臣基', '地乙'], '申': [], '坤': [], '酉': [], '戌': ['直符'], '乾': ['帝符'], '亥': ['天乙']}}
	#公元
	Taiyi(658,5,31,0,14).pan(0) 
	{'太乙計': '時計', '公元日期': '658年5月31日0時', '干支': ['戊午', '丁巳', '丙子', '戊子'], '農曆': {'年': 658, '月': 4, '日': 24}, '年號': '唐高宗李治 永徽九年', '紀元': '丙子元第二紀', '時局': '陽遁37局', '太乙': 6, '文昌': '坤', '太歲': '子', '合神': '丑', '計神': '寅', '始擊': '未', '定目': '未', '主算': [7, ['無天', '雜陰']], '客算': [8, ['無天', '雜陽']], '定算': [8, ['無天', '雜陽']], '九宮': {8: '客將定將大游', 3: '五風', 4: '客參定參', 9: '', 5: '', 2: '八風', 7: '主將三風', 6: '太乙', 1: '主參飛鳥小游'}, '十六宮': {'子': ['太歲', '太尊'], '丑': ['合神'], '艮': [], '寅': [], '卯': [], '辰': ['君基', '臣基', '帝符'], '巽': [], '巳': [], '午': [], '未': ['始擊', '定目'], '申': ['民基'], '坤': ['文昌'], '酉': [], '戌': [], '乾': ['五福'], '亥': []}}
	
```
## 3. 太乙古籍

| 年份          | 作者           | 書名                                            | 備註       |
| ------------- | ------------- | --------------------------------------------- | ------------- |
| 隋  | 臨孝恭   | 太一式經        |                                              |               |
| 唐  | 王希明  | 太乙金鏡式經      | 唐王希明撰。希明不詳其裏貫。開元時以方技為內供奉，待詔翰林。是書乃其奉敕所編，見於《新唐書·藝文志》，故書中多自稱臣。而其間推太乙積年有至宋景祐元年者，則後人已有所增入，非盡希明之舊也。|
| 宋  | 楊惟德  | 景佑太乙福應經  | 10卷，收藏於四庫全書  |
| 宋  | 王佐  | 太乙秘書 | 收藏於光緒九年清隱山房叢書  |
| 宋  | 丘浚  | 太乙淘金歌 |   |
| 元  | 曉山老人  | 太乙統宗寶鑒 | 舊題元曉山老人撰，不知其姓名。前有大德七年自序。錢曾《讀書敏求記》，稱其家藏舊鈔《統宗寶鑒》有二本；其一後附《起例》、《真數》、《淘金歌》三書各一卷，其一後附《數林》、《籌數》、《專徵集略》、《神機三鏡》四書各一卷。 |
| 元  | 曉山老人  | 太乙統宗福應紫庭金鏡集成 二十四卷 | 收藏於光緒九年清隱山房叢書  |
| 元  | 曉山老人  | 太乙命書  | 上下卷  |
| 宋  | 佚名 | 太一占鳥法  | 1卷  |
| 宋  | 魏申 | 太一總   | 100卷 |
| 宋  | 張中 | 太一金照辨誤歸正論   | 1卷 |
| 宋  | 楊惟德、王立 | 太一福應集要  | 1卷 |
| 宋  | 佚名 | 太一玄鑒  | 10卷 |
| 宋  | 佚名 | 太一新鑒  | 3卷 |
| 宋  | 佚名 | 遁甲步小遊太一諸將立成圖 | 2卷  |
| 宋  | 知玄子、秦浼 | 太一占玄歌 | 1卷  |
| 宋  | 佚名 | 太一五元新曆  | 1卷 |
| 宋  | 佚名 | 太一七術  | 1卷 |
| 宋  | 佚名 | 太一陰陽定計主客決勝法 | 1卷  |
| 宋  | 佚名 | 太一迴圈曆 | 1卷  |
| 宋  | 佚名 | 太一會運逆順通代記陣圖 | 1卷  |
| 宋  | 胡萬頃 | 太一遁甲萬勝時定主客立成訣 | 1卷  |
| 宋  | 佚名 | 太一集 | 8卷  |
| 宋  | 佚名 | 太一年表 | 1卷  |
| 宋  | 佚名 | 十三神太一 | 1卷  |
| 宋  | 佚名 | 禦序景佑三式太一福應集要 | 10卷  |
| 宋  | 王處訥 | 太一青龍甲寅經 | 1卷  |
| 宋  | 康洙序 | 時遊太一立成 | 1卷  |
| 宋  | 廣夷 | 太一秘歌 | 1卷  |
| 宋  | 佚名  | 太一細行草 | 1卷  |
| 宋  | 佚名  | 太一雜集筆草 | 1卷  |
| 宋  | 佚名  | 太一時計鈐 | 1卷  |
| 宋  | 佚名  | 太一陽九百六經 | 1卷  |
| 宋  | 佚名  | 太一神樞長曆 | 1卷  |
| 宋  | 佚名  | 太一陽局鈐 | 1卷  |
| 宋  | 佚名  | 太一陰局鈐 | 1卷  |
| 宋  | 佚名  | 九宮太一 | 1卷  |
| 宋  | 佚名  | 日遊太一五子元出軍勝負七十二局 | 1卷  |
| 宋  | 佚名  | 九宮應瑞太一圖 | 1卷  |
| 宋  | 佚名  | 太一中天密旨 | 3卷  |
| 宋  | 佚名  | 太一遁甲萬一訣 |   |
| 宋  | 佚名  | 太一陰陽二遁 |   |
| 宋  | 佚名  | 太一金鏡備式錄 | 10卷  |
| 宋  | 佚名  | 太一立成圖 |  1卷 |
| 宋  | 佚名  | 太一飛鳥十精曆 | 1卷  |
| 明  | 潘元焯  | 輯太乙說  |   |
| 明  | 王鳴鶴  | 太乙卷 |  第3冊，出自〈登壇必究〉《武備志》太乙篇 |
| 明  | 茅元儀  | 太乙成書  | 不著撰人名氏。是書以太乙五將奇偶二算演七十二局，視歲神吉凶。其法以上元甲子歲太乙起乾行八宮，每三年一徙。計神起寅，逆行十二辰，天目起甲，順行十六神。又以計神加艮求天目所在，為始擊將，而天目、始擊又各以其算立大將、參將，故必七十六局而五將遊行變動之格始周。 |
| 明  | 潘元焯  | 輯太乙說  |   |
| 明  | 喻龍德輯  | 太乙相天根 | 收錄自喻子十三種秘書兵衡卷12  |
| 明  | 佚名 | 太乙數統宗大全  | 40卷清集福堂刻 6卷3冊全民國中原書局石印  |
| 明  | 李自明 | 太乙遁甲專征賦  | 一卷（浙江範懋柱家天一閣藏本）不著撰人名氏。考焦竑《經籍志》有明員卓《遁甲專征賦》，其名與此相合，或即卓書，或後人所擬作，莫能詳也。其書以遁甲論行軍趨避之用，不外《煙波釣叟歌》中之意，別無所發明。且以太乙命名，而篇中絕無一語及太乙九宮計神主客者，尤為不可解矣。 |
| 明  | 佚名 | 太乙遁局  | 不分卷8卷，明藍格鈔本，國家圖書館館藏   |
| 明  | 佚名 | 太乙歷數  |    |
| 明  | 張德常 | 太乙遁算數理  |    |
| 明  | 佚名 | 太乙燭幽經  |  2卷 |
| 明  | 佚名 | 太乙原古  |  3卷 |
| 明  | 葉容 | 太乙三辰顯異經  |  10卷 |
| 明  | 李元灃 | 太乙九旗曆  |  3卷 |
| 明  | 邢雲路 |太乙書  |  10卷 |
| 明  | 佚名 | 太乙會鈐 |  1卷 |
| 明  | 佚名 | 太乙四種 |   |
| 明  | 佚名 | 太乙十精 | 2卷 |
| 明  | 佚名 | 太乙星書 | 2卷 |
| 明  | 佚名 | 黃帝太乙八門入式訣書 | 3卷 |
| 明  | 佚名 | 太乙金鑰匙 | 1卷 |
| 清  | 劉學誠 | 太乙照神經 | 1卷 |
| 清  | 李自明 | 太乙神數  | 上海大成書局民國11年書刊6厚冊一套全，含太乙淘金歌. 太乙局.太乙人道命法 |
| 清  | 佚名 | 太乙廟算書 | 中國國家圖書館館藏 |
| 清  | 佚名 | 太乙命訣 | 1卷 陳氏曰：稱袁天罡，妄人假 。 |
| 清  | 佚名 | 太乙顯微鈐 | 收錄於《四明天一閣藏書目錄》內。 |
| 清  | 佚名 | 太乙通福應經 | 五本，收錄於《四明天一閣藏書目錄》內。 |
| 清  | 佚名 | 太乙專經賦 | 收錄於《四明天一閣藏書目錄》內。 |
| 清  | 佚名 | 太乙十精風雨賦 | 收錄於《四明天一閣藏書目錄》內。 |
| 清  | 佚名 | 太乙成書 | 收錄於《四明天一閣藏書目錄》內。 |
| 日本  | 河原田寛 | 太乙六壬二占要略 | 日本國會圖書館藏書。 |
| 日本  | 張明澄 | 太乙神數講義 | 明代の太乙は『太乙淘金歌』に始まり、现代の研究では故张明澄先生の讲义録が一番わかりやすく书かれている。太乙命理に関しては『太乙命书』に诸星の复雑な配合によって太乙命理を论じる内容が详しく书かれている。 |




