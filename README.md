汉字相关的数据，如拼音、简繁体等。


## 简繁体转换

有两种思路：

1. 简体与繁体字的对应表。
2. 汉字编码对应表。简体GBK编码 <---> Unicode编码 <---> 繁体字BIG5编码。[VC----实现汉字简繁转换](http://blog.csdn.net/yf210yf/article/details/7850472)



## 已搜集数据

### [Pinyin.dat](/data/Pinyin.dat)

汉字与拼音的对应表，格式如下：

    3400    QIU1
    3401    TIAN3 TIAN4
    3404    KUA4
    3405    WU3
    3406    YIN3
    340C    SI4 YI2
    3416    YE4
    341C    CHOU2
    3421    NUO4

第一列是十六进制的Unicode编码，第二列是拼音+声调，多个发音用空格隔开


### [Pinyin2.dat](/data/Pinyin2.dat)

另一张汉字与拼音对应表，未整理


### [Simple&Traditional.dat](/data/Simple&Traditional.dat)

简繁体字、词的对应表，单字部分同时包含了 `简:繁` 和 `繁:简`，如：

    "垩": "堊",
    ....隔了N行...
    "堊": "垩",

### [字符的不同编码](\data\encode)

有PDF、Word、Excel文件。

Excel文件是[汉字的GB18030与Unicode编码.xls](\data\encode\汉字的GB18030与Unicode编码.xls)，内容如下：

|汉字|GBK(GB18030)编码|Unicode编码|
|---|---|---|
|一|D2BB|4E00|
|丁|B6A1|4E01|
|丂|8140|4E02|




注意简繁体并不是一对一的关系，比如

    "反复": "反複",
    "反复": "反覆",


