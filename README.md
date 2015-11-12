汉字相关的数据与处理方法，如拼音、简繁体等。

目前仅搜集了原始数据。

## 已搜集数据

### 1. [Pinyin.dat](/data/Pinyin.dat)

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

### 2. [Simple&Traditional.dat](/data/Simple&Traditional.dat)

简繁体字、词的对应表，单字部分同时包含了 `简:繁` 和 `繁:简`，如：

    "垩": "堊",
    ....隔了N行...
    "堊": "垩",


注意简繁体并不是一对一的关系，比如

    "反复": "反複",
    "反复": "反覆",


## TODO

1. 处理数据格式，使之更易读取
2. 写 Python 和 Java 版读取与处理的Demo
