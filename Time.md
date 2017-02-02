<h1 id="preface">前言</h1>
因为电影的信息会根据地区的不同而不同，所以在 url 后面需要拼接地区 locationId，获取的方式有两种 ——

- 访问 url：[`https://api-m.mtime.cn/Showtime/HotCitiesByCinema.api`](https://api-m.mtime.cn/Showtime/HotCitiesByCinema.api)
- 将它写在本地，由于 json 较长，我就将它另存为了一个 md 文件，[戳我进链接](https://github.com/jokermonn/-Api/blob/master/area-id.md)

ps：Time 时光 App 是本地存了一份，但同时每次启动 app 又会访问 url，同时将数据重新写入文件

<h2 id="sell_tickets">正在售票(包括正在热映和即将上映)</h2>
url：`https://api-m.mtime.cn/PageSubArea/HotPlayMovies.api?locationId=?`

示例 url：[`https://api-m.mtime.cn/PageSubArea/HotPlayMovies.api?locationId=290`](https://api-m.mtime.cn/PageSubArea/HotPlayMovies.api?locationId=290)

说明：`locationId` 就是[前言](#preface)中所说的 `locationId`

json 示例：

	{
	  "count": 15,
	  "movies": [
	    {
	      "actorName1": "吴亦凡",
	      "actorName2": "林更新",
	      "btnText": "",
	      "commonSpecial": "唐僧\"重色轻友\"与悟空反目",
	      "directorName": "徐克",
	      "img": "http://img5.mtime.cn/mt/2017/01/27/114649.37790398_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": true,
	      "isIMAX": false,
	      "isIMAX3D": true,
	      "isNew": false,
	      "length": 108,
	      "movieId": 208325,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 152,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 1797
	      },
	      "rDay": 28,
	      "rMonth": 1,
	      "rYear": 2017,
	      "ratingFinal": 6.7,
	      "titleCn": "西游伏妖篇",
	      "titleEn": "Journey to the West: Demon Chapter",
	      "type": "奇幻 / 动作 / 喜剧",
	      "wantedCount": 2631
	    },
	    {
	      "actorName1": "成龙",
	      "actorName2": "李治廷",
	      "btnText": "",
	      "commonSpecial": "大哥携“小鲜肉”全球寻宝石",
	      "directorName": "唐季礼",
	      "img": "http://img5.mtime.cn/mt/2017/01/13/191421.14582165_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": true,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 108,
	      "movieId": 217896,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 152,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 1767
	      },
	      "rDay": 28,
	      "rMonth": 1,
	      "rYear": 2017,
	      "ratingFinal": 6.2,
	      "titleCn": "功夫瑜伽",
	      "titleEn": "Kung-Fu Yoga",
	      "type": "动作 / 冒险 / 喜剧",
	      "wantedCount": 1130
	    },
	    {
	      "actorName1": "邓超",
	      "actorName2": "彭于晏",
	      "btnText": "",
	      "commonSpecial": "邓超彭于晏一起街头热血",
	      "directorName": "韩寒",
	      "img": "http://img5.mtime.cn/mt/2017/01/12/181512.62044353_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": true,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 102,
	      "movieId": 237054,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 151,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 1112
	      },
	      "rDay": 28,
	      "rMonth": 1,
	      "rYear": 2017,
	      "ratingFinal": 6.5,
	      "titleCn": "乘风破浪",
	      "titleEn": "Duckweed",
	      "type": "喜剧",
	      "wantedCount": 2803
	    },
	    {
	      "actorName1": "王宝强",
	      "actorName2": "柳岩",
	      "btnText": "",
	      "commonSpecial": "王宝强领衔兄弟帮大战\"金角银角\"",
	      "directorName": "王宝强",
	      "img": "http://img5.mtime.cn/mt/2016/12/22/152717.78232341_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": true,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 100,
	      "movieId": 225095,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 148,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 1089
	      },
	      "rDay": 28,
	      "rMonth": 1,
	      "rYear": 2017,
	      "ratingFinal": 5.7,
	      "titleCn": "大闹天竺",
	      "titleEn": "Buddies In India",
	      "type": "喜剧 / 爱情",
	      "wantedCount": 1188
	    },
	    {
	      "actorName1": "尚雯婕",
	      "actorName2": "曾舜晞",
	      "btnText": "",
	      "commonSpecial": "熊大熊二开启全新探险",
	      "directorName": "丁亮",
	      "img": "http://img5.mtime.cn/mt/2017/01/18/112429.65153551_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 89,
	      "movieId": 235457,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 147,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 769
	      },
	      "rDay": 28,
	      "rMonth": 1,
	      "rYear": 2017,
	      "ratingFinal": 5.8,
	      "titleCn": "熊出没·奇幻空间",
	      "titleEn": "Entangled Worlds",
	      "type": "动画",
	      "wantedCount": 396
	    },
	    {
	      "actorName1": "贾乃亮",
	      "actorName2": "马丽",
	      "btnText": "",
	      "commonSpecial": "",
	      "directorName": "郭大雷",
	      "img": "http://img5.mtime.cn/mt/2017/01/16/104630.29361196_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 0,
	      "movieId": 230769,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 1,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 1
	      },
	      "rDay": 3,
	      "rMonth": 2,
	      "rYear": 2017,
	      "ratingFinal": -1,
	      "titleCn": "东北往事之破马张飞",
	      "titleEn": "North East Past:Po Ma Zhang Fei",
	      "type": "喜剧",
	      "wantedCount": 1678
	    },
	    {
	      "actorName1": "艾丽·范宁",
	      "actorName2": "戴恩·德哈恩",
	      "btnText": "",
	      "commonSpecial": "五光十色梦想秀，勿忘初心够真诚",
	      "directorName": "埃里克·萨默",
	      "img": "http://img5.mtime.cn/mt/2017/01/13/105159.84633417_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 89,
	      "movieId": 234178,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 108,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 294
	      },
	      "rDay": 1,
	      "rMonth": 2,
	      "rYear": 2017,
	      "ratingFinal": 7.6,
	      "titleCn": "了不起的菲丽西",
	      "titleEn": "Ballerina",
	      "type": "动画 / 冒险 / 家庭",
	      "wantedCount": 359
	    },
	    {
	      "actorName1": "艾米·亚当斯",
	      "actorName2": "杰瑞米·雷纳",
	      "btnText": "",
	      "commonSpecial": "用东方哲学拯救世界",
	      "directorName": "丹尼斯·维伦纽瓦",
	      "img": "http://img5.mtime.cn/mt/2017/01/09/150116.98345754_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 116,
	      "movieId": 221966,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 23,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 85
	      },
	      "rDay": 20,
	      "rMonth": 1,
	      "rYear": 2017,
	      "ratingFinal": 7.7,
	      "titleCn": "降临",
	      "titleEn": "Arrival",
	      "type": "科幻 / 悬疑 / 剧情",
	      "wantedCount": 1563
	    },
	    {
	      "actorName1": "范·迪塞尔",
	      "actorName2": "露比·罗丝",
	      "btnText": "",
	      "commonSpecial": "",
	      "directorName": "D·J·卡卢索",
	      "img": "http://img5.mtime.cn/mt/2017/01/05/105822.16893974_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": true,
	      "isNew": false,
	      "length": 107,
	      "movieId": 125805,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 14,
	        "nearestShowDay": 1486627200,
	        "nearestShowtimeCount": 14
	      },
	      "rDay": 10,
	      "rMonth": 2,
	      "rYear": 2017,
	      "ratingFinal": -1,
	      "titleCn": "极限特工：终极回归",
	      "titleEn": "xXx: The Return of Xander Cage",
	      "type": "动作 / 冒险 / 惊悚",
	      "wantedCount": 1358
	    },
	    {
	      "actorName1": "克里斯·帕拉特",
	      "actorName2": "詹妮弗·劳伦斯",
	      "btnText": "",
	      "commonSpecial": "星爵大表姐展开太空冒险",
	      "directorName": "莫腾·泰杜姆",
	      "img": "http://img5.mtime.cn/mt/2016/12/26/113421.22552790_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 116,
	      "movieId": 123883,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 27,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 69
	      },
	      "rDay": 13,
	      "rMonth": 1,
	      "rYear": 2017,
	      "ratingFinal": 7.7,
	      "titleCn": "太空旅客",
	      "titleEn": "Passengers",
	      "type": "冒险 / 剧情 / 爱情",
	      "wantedCount": 2720
	    },
	    {
	      "actorName1": "舒淇",
	      "actorName2": "王千源",
	      "btnText": "",
	      "commonSpecial": "王千源忽悠舒淇，忘忧下隐藏骗局",
	      "directorName": "陈玉勋",
	      "img": "http://img5.mtime.cn/mt/2017/01/12/110132.45466011_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 116,
	      "movieId": 231591,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 36,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 65
	      },
	      "rDay": 27,
	      "rMonth": 1,
	      "rYear": 2017,
	      "ratingFinal": 6.6,
	      "titleCn": "健忘村",
	      "titleEn": "The Village Of No Return",
	      "type": "爱情 / 剧情",
	      "wantedCount": 354
	    },
	    {
	      "actorName1": "安德鲁·加菲尔德",
	      "actorName2": "文斯·沃恩",
	      "btnText": "",
	      "commonSpecial": "加菲演绎铁血柔情",
	      "directorName": "梅尔·吉布森",
	      "img": "http://img5.mtime.cn/mt/2016/11/21/080817.61278717_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 139,
	      "movieId": 219171,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 10,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 33
	      },
	      "rDay": 8,
	      "rMonth": 12,
	      "rYear": 2016,
	      "ratingFinal": 8.4,
	      "titleCn": "血战钢锯岭",
	      "titleEn": "Hacksaw Ridge",
	      "type": "剧情 / 历史 / 战争",
	      "wantedCount": 2637
	    },
	    {
	      "actorName1": "瑞恩·高斯林",
	      "actorName2": "艾玛·斯通",
	      "btnText": "",
	      "commonSpecial": "",
	      "directorName": "达米恩·查泽雷",
	      "img": "http://img5.mtime.cn/mt/2017/01/13/095311.48058459_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": true,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 129,
	      "movieId": 219784,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 18,
	        "nearestShowDay": 1486800000,
	        "nearestShowtimeCount": 31
	      },
	      "rDay": 14,
	      "rMonth": 2,
	      "rYear": 2017,
	      "ratingFinal": 8.3,
	      "titleCn": "爱乐之城",
	      "titleEn": "La La Land",
	      "type": "爱情 / 喜剧 / 剧情",
	      "wantedCount": 1369
	    },
	    {
	      "actorName1": "",
	      "actorName2": "",
	      "btnText": "",
	      "commonSpecial": "北极熊临危受命变身超级特工",
	      "directorName": "",
	      "img": "http://img5.mtime.cn/mt/2017/01/09/143248.22516261_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 90,
	      "movieId": 237747,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 16,
	        "nearestShowDay": 1486022400,
	        "nearestShowtimeCount": 26
	      },
	      "rDay": 13,
	      "rMonth": 1,
	      "rYear": 2017,
	      "ratingFinal": 5.5,
	      "titleCn": "大卫贝肯之倒霉特工熊",
	      "titleEn": "Backkom Bear：Agent 008",
	      "type": "动画 / 家庭 / 冒险",
	      "wantedCount": 220
	    },
	    {
	      "actorName1": "葛优",
	      "actorName2": "谢霆锋",
	      "btnText": "",
	      "commonSpecial": "",
	      "directorName": "叶伟民",
	      "img": "http://img5.mtime.cn/mt/2017/01/10/090134.10115693_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "length": 0,
	      "movieId": 232595,
	      "nearestShowtime": {
	        "isTicket": true,
	        "nearestCinemaCount": 2,
	        "nearestShowDay": 1486627200,
	        "nearestShowtimeCount": 2
	      },
	      "rDay": 10,
	      "rMonth": 2,
	      "rYear": 2017,
	      "ratingFinal": -1,
	      "titleCn": "决战食神",
	      "titleEn": "Cook Up A Storm",
	      "type": "喜剧 / 爱情 / 家庭",
	      "wantedCount": 259
	    }
	  ],
	  "totalCinemaCount": 188,
	  "totalComingMovie": 38,
	  "totalHotMovie": 29
	}

解析：

- `count`：`movies` 链表的长度
- `movies`：热映电影信息
- `actorName1`：主演1
- `actorName2`：主演2
- `commenSpecial`：一句话总结该电影
- `directorName`：导演名
- `img`：图片链接
- `is3D`：是否是 3D 电影
- `isDMAX`：是否是 DMAX 电影
- `isFilter`：???
- `isHot`：是否是热映电影
- `isIMAX`：是否是 IMAX 电影
- `isIMAX3D`：是否是 IMAX3D 电影
- `isNew`：???
- `length`：影片时长
- `movieId`：影片 id，需要提供给[影片详情](#movie_detail)
- `isTicket`：是否有票
- `nearestCinemaCount`：今日上映该电影的影院数量
- `rDay`、`rMonth`、`rYear`：影片上映年月日
- `ratingFinal`：评分
- `titleCn`：影片中文名
- `titleEn`：影片英文名
- `type`：影片类型
- `wantedCount`：多少人想看
- `totalCinemacount`：同城影院数量
- `totalComingMovie`：即将上映影片数量
- `totalHotMovie`：实际正在售票电影数量

<h2 id="hot_movies">正在热映</h2>

url：`https://api-m.mtime.cn/Showtime/LocationMovies.api?locationId=?`

示例 url：[`https://api-m.mtime.cn/Showtime/LocationMovies.api?locationId=290`](https://api-m.mtime.cn/Showtime/LocationMovies.api?locationId=290)

json 示例：

	{
	  "bImg": "http://img5.mtime.cn/mg/2017/01/25/172446.45527982.jpg",
	  "date": "2017-02-02",
	  "lid": 290,
	  "ms": [
	    {
	      "NearestCinemaCount": 152,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 1767,
	      "aN1": "成龙",
	      "aN2": "李治廷",
	      "cC": 152,
	      "commonSpecial": "大哥携“小鲜肉”全球寻宝石",
	      "d": "108",
	      "dN": "唐季礼",
	      "def": 0,
	      "id": 217896,
	      "img": "http://img5.mtime.cn/mt/2017/01/13/191421.14582165_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": true,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "动作 / 冒险 / 喜剧",
	      "p": [
	        "动作冒险喜剧"
	      ],
	      "r": 6.2,
	      "rc": 0,
	      "rd": "20170128",
	      "rsC": 0,
	      "sC": 3003,
	      "t": "功夫瑜伽",
	      "tCn": "功夫瑜伽",
	      "tEn": "Kung-Fu Yoga",
	      "ua": -1,
	      "versions": [],
	      "wantedCount": 1132
	    },
	    {
	      "NearestCinemaCount": 152,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 1797,
	      "aN1": "吴亦凡",
	      "aN2": "林更新",
	      "cC": 152,
	      "commonSpecial": "唐僧\"重色轻友\"与悟空反目",
	      "d": "108",
	      "dN": "徐克",
	      "def": 0,
	      "id": 208325,
	      "img": "http://img5.mtime.cn/mt/2017/01/27/114649.37790398_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": true,
	      "isIMAX": false,
	      "isIMAX3D": true,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "奇幻 / 动作 / 喜剧",
	      "p": [
	        "奇幻动作喜剧"
	      ],
	      "r": 6.7,
	      "rc": 0,
	      "rd": "20170128",
	      "rsC": 0,
	      "sC": 2992,
	      "t": "西游伏妖篇",
	      "tCn": "西游伏妖篇",
	      "tEn": "Journey to the West: Demon Chapter",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 2,
	          "version": "3D"
	        },
	        {
	          "enum": 4,
	          "version": "IMAX3D"
	        },
	        {
	          "enum": 6,
	          "version": "中国巨幕"
	        }
	      ],
	      "wantedCount": 2632
	    },
	    {
	      "NearestCinemaCount": 151,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 1112,
	      "aN1": "邓超",
	      "aN2": "彭于晏",
	      "cC": 151,
	      "commonSpecial": "邓超彭于晏一起街头热血",
	      "d": "102",
	      "dN": "韩寒",
	      "def": 0,
	      "id": 237054,
	      "img": "http://img5.mtime.cn/mt/2017/01/12/181512.62044353_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": true,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "喜剧",
	      "p": [
	        "喜剧"
	      ],
	      "r": 6.5,
	      "rc": 0,
	      "rd": "20170128",
	      "rsC": 0,
	      "sC": 1928,
	      "t": "乘风破浪",
	      "tCn": "乘风破浪",
	      "tEn": "Duckweed",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 2802
	    },
	    {
	      "NearestCinemaCount": 148,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 1089,
	      "aN1": "王宝强",
	      "aN2": "柳岩",
	      "cC": 148,
	      "commonSpecial": "王宝强领衔兄弟帮大战\"金角银角\"",
	      "d": "100",
	      "dN": "王宝强",
	      "def": 0,
	      "id": 225095,
	      "img": "http://img5.mtime.cn/mt/2016/12/22/152717.78232341_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": true,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "喜剧 / 爱情",
	      "p": [
	        "喜剧爱情"
	      ],
	      "r": 5.7,
	      "rc": 0,
	      "rd": "20170128",
	      "rsC": 0,
	      "sC": 1799,
	      "t": "大闹天竺",
	      "tCn": "大闹天竺",
	      "tEn": "Buddies In India",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 1188
	    },
	    {
	      "NearestCinemaCount": 147,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 769,
	      "aN1": "尚雯婕",
	      "aN2": "曾舜晞",
	      "cC": 147,
	      "commonSpecial": "熊大熊二开启全新探险",
	      "d": "89",
	      "dN": "丁亮",
	      "def": 0,
	      "id": 235457,
	      "img": "http://img5.mtime.cn/mt/2017/01/18/112429.65153551_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "动画",
	      "p": [
	        "动画"
	      ],
	      "r": 5.8,
	      "rc": 0,
	      "rd": "20170128",
	      "rsC": 0,
	      "sC": 1247,
	      "t": "熊出没·奇幻空间",
	      "tCn": "熊出没·奇幻空间",
	      "tEn": "Entangled Worlds",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 395
	    },
	    {
	      "NearestCinemaCount": 1,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 1,
	      "aN1": "贾乃亮",
	      "aN2": "马丽",
	      "cC": 104,
	      "commonSpecial": "",
	      "d": "0",
	      "dN": "郭大雷",
	      "def": 0,
	      "id": 230769,
	      "img": "http://img5.mtime.cn/mt/2017/01/16/104630.29361196_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "喜剧",
	      "p": [
	        "喜剧"
	      ],
	      "r": -1,
	      "rc": 0,
	      "rd": "20170203",
	      "rsC": 0,
	      "sC": 779,
	      "t": "东北往事之破马张飞",
	      "tCn": "东北往事之破马张飞",
	      "tEn": "North East Past:Po Ma Zhang Fei",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 1677
	    },
	    {
	      "NearestCinemaCount": 108,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 294,
	      "aN1": "艾丽·范宁",
	      "aN2": "戴恩·德哈恩",
	      "cC": 112,
	      "commonSpecial": "五光十色梦想秀，勿忘初心够真诚",
	      "d": "89",
	      "dN": "埃里克·萨默",
	      "def": 0,
	      "id": 234178,
	      "img": "http://img5.mtime.cn/mt/2017/01/13/105159.84633417_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "动画 / 冒险 / 家庭",
	      "p": [
	        "动画冒险家庭"
	      ],
	      "r": 7.6,
	      "rc": 0,
	      "rd": "20170201",
	      "rsC": 0,
	      "sC": 488,
	      "t": "了不起的菲丽西",
	      "tCn": "了不起的菲丽西",
	      "tEn": "Ballerina",
	      "ua": -1,
	      "versions": [],
	      "wantedCount": 359
	    },
	    {
	      "NearestCinemaCount": 23,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 85,
	      "aN1": "艾米·亚当斯",
	      "aN2": "杰瑞米·雷纳",
	      "cC": 24,
	      "commonSpecial": "用东方哲学拯救世界",
	      "d": "116",
	      "dN": "丹尼斯·维伦纽瓦",
	      "def": 0,
	      "id": 221966,
	      "img": "http://img5.mtime.cn/mt/2017/01/09/150116.98345754_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "科幻 / 悬疑 / 剧情",
	      "p": [
	        "科幻悬疑剧情"
	      ],
	      "r": 7.7,
	      "rc": 0,
	      "rd": "20170120",
	      "rsC": 0,
	      "sC": 198,
	      "t": "降临",
	      "tCn": "降临",
	      "tEn": "Arrival",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        },
	        {
	          "enum": 6,
	          "version": "中国巨幕"
	        }
	      ],
	      "wantedCount": 1563
	    },
	    {
	      "NearestCinemaCount": 14,
	      "NearestDay": 1486627200,
	      "NearestShowtimeCount": 14,
	      "aN1": "范·迪塞尔",
	      "aN2": "露比·罗丝",
	      "cC": 27,
	      "commonSpecial": "",
	      "d": "107",
	      "dN": "D·J·卡卢索",
	      "def": 0,
	      "id": 125805,
	      "img": "http://img5.mtime.cn/mt/2017/01/05/105822.16893974_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": true,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "动作 / 冒险 / 惊悚",
	      "p": [
	        "动作冒险惊悚"
	      ],
	      "r": -1,
	      "rc": 0,
	      "rd": "20170210",
	      "rsC": 0,
	      "sC": 181,
	      "t": "极限特工：终极回归",
	      "tCn": "极限特工：终极回归",
	      "tEn": "xXx: The Return of Xander Cage",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 2,
	          "version": "3D"
	        },
	        {
	          "enum": 4,
	          "version": "IMAX3D"
	        },
	        {
	          "enum": 6,
	          "version": "中国巨幕"
	        }
	      ],
	      "wantedCount": 1359
	    },
	    {
	      "NearestCinemaCount": 27,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 69,
	      "aN1": "克里斯·帕拉特",
	      "aN2": "詹妮弗·劳伦斯",
	      "cC": 28,
	      "commonSpecial": "星爵大表姐展开太空冒险",
	      "d": "116",
	      "dN": "莫腾·泰杜姆",
	      "def": 0,
	      "id": 123883,
	      "img": "http://img5.mtime.cn/mt/2016/12/26/113421.22552790_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "冒险 / 剧情 / 爱情",
	      "p": [
	        "冒险剧情爱情"
	      ],
	      "r": 7.7,
	      "rc": 0,
	      "rd": "20170113",
	      "rsC": 0,
	      "sC": 123,
	      "t": "太空旅客",
	      "tCn": "太空旅客",
	      "tEn": "Passengers",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 2,
	          "version": "3D"
	        },
	        {
	          "enum": 6,
	          "version": "中国巨幕"
	        }
	      ],
	      "wantedCount": 2720
	    },
	    {
	      "NearestCinemaCount": 36,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 65,
	      "aN1": "舒淇",
	      "aN2": "王千源",
	      "cC": 40,
	      "commonSpecial": "王千源忽悠舒淇，忘忧下隐藏骗局",
	      "d": "116",
	      "dN": "陈玉勋",
	      "def": 0,
	      "id": 231591,
	      "img": "http://img5.mtime.cn/mt/2017/01/12/110132.45466011_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "爱情 / 剧情",
	      "p": [
	        "爱情剧情"
	      ],
	      "r": 6.6,
	      "rc": 0,
	      "rd": "20170127",
	      "rsC": 0,
	      "sC": 117,
	      "t": "健忘村",
	      "tCn": "健忘村",
	      "tEn": "The Village Of No Return",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 354
	    },
	    {
	      "NearestCinemaCount": 10,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 33,
	      "aN1": "安德鲁·加菲尔德",
	      "aN2": "文斯·沃恩",
	      "cC": 10,
	      "commonSpecial": "加菲演绎铁血柔情",
	      "d": "139",
	      "dN": "梅尔·吉布森",
	      "def": 0,
	      "id": 219171,
	      "img": "http://img5.mtime.cn/mt/2016/11/21/080817.61278717_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "剧情 / 历史 / 战争",
	      "p": [
	        "剧情历史战争"
	      ],
	      "r": 8.4,
	      "rc": 0,
	      "rd": "20161208",
	      "rsC": 0,
	      "sC": 64,
	      "t": "血战钢锯岭",
	      "tCn": "血战钢锯岭",
	      "tEn": "Hacksaw Ridge",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 2637
	    },
	    {
	      "NearestCinemaCount": 18,
	      "NearestDay": 1486800000,
	      "NearestShowtimeCount": 31,
	      "aN1": "瑞恩·高斯林",
	      "aN2": "艾玛·斯通",
	      "cC": 19,
	      "commonSpecial": "",
	      "d": "129",
	      "dN": "达米恩·查泽雷",
	      "def": 0,
	      "id": 219784,
	      "img": "http://img5.mtime.cn/mt/2017/01/13/095311.48058459_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": true,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "爱情 / 喜剧 / 剧情",
	      "p": [
	        "爱情喜剧剧情"
	      ],
	      "r": 8.3,
	      "rc": 0,
	      "rd": "20170214",
	      "rsC": 0,
	      "sC": 58,
	      "t": "爱乐之城",
	      "tCn": "爱乐之城",
	      "tEn": "La La Land",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        },
	        {
	          "enum": 3,
	          "version": "IMAX"
	        }
	      ],
	      "wantedCount": 1370
	    },
	    {
	      "NearestCinemaCount": 16,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 26,
	      "aN1": "",
	      "aN2": "",
	      "cC": 17,
	      "commonSpecial": "北极熊临危受命变身超级特工",
	      "d": "90",
	      "dN": "",
	      "def": 0,
	      "id": 237747,
	      "img": "http://img5.mtime.cn/mt/2017/01/09/143248.22516261_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "动画 / 家庭 / 冒险",
	      "p": [
	        "动画家庭冒险"
	      ],
	      "r": 5.5,
	      "rc": 0,
	      "rd": "20170113",
	      "rsC": 0,
	      "sC": 46,
	      "t": "大卫贝肯之倒霉特工熊",
	      "tCn": "大卫贝肯之倒霉特工熊",
	      "tEn": "Backkom Bear：Agent 008",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        },
	        {
	          "enum": 2,
	          "version": "3D"
	        }
	      ],
	      "wantedCount": 220
	    },
	    {
	      "NearestCinemaCount": 2,
	      "NearestDay": 1486627200,
	      "NearestShowtimeCount": 2,
	      "aN1": "葛优",
	      "aN2": "谢霆锋",
	      "cC": 9,
	      "commonSpecial": "",
	      "d": "0",
	      "dN": "叶伟民",
	      "def": 0,
	      "id": 232595,
	      "img": "http://img5.mtime.cn/mt/2017/01/10/090134.10115693_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "喜剧 / 爱情 / 家庭",
	      "p": [
	        "喜剧爱情家庭"
	      ],
	      "r": -1,
	      "rc": 0,
	      "rd": "20170210",
	      "rsC": 0,
	      "sC": 33,
	      "t": "决战食神",
	      "tCn": "决战食神",
	      "tEn": "Cook Up A Storm",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 259
	    },
	    {
	      "NearestCinemaCount": 8,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 17,
	      "aN1": "肖央",
	      "aN2": "闫妮",
	      "cC": 11,
	      "commonSpecial": "这生活原来不过是一场春梦",
	      "d": "113",
	      "dN": "宋晓飞",
	      "def": 0,
	      "id": 237503,
	      "img": "http://img5.mtime.cn/mt/2016/12/19/180749.11589052_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "喜剧",
	      "p": [
	        "喜剧"
	      ],
	      "r": 7,
	      "rc": 0,
	      "rd": "20161230",
	      "rsC": 0,
	      "sC": 31,
	      "t": "情圣",
	      "tCn": "情圣",
	      "tEn": "Some Like It Hot",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 1458
	    },
	    {
	      "NearestCinemaCount": 9,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 19,
	      "aN1": "菲丽希缇·琼斯",
	      "aN2": "迭戈·鲁纳",
	      "cC": 11,
	      "commonSpecial": "甄子丹姜文CP毫无违和",
	      "d": "134",
	      "dN": "加里斯·爱德华斯",
	      "def": 0,
	      "id": 214815,
	      "img": "http://img5.mtime.cn/mt/2016/12/06/112818.78182251_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": true,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "动作 / 战争 / 冒险",
	      "p": [
	        "动作战争冒险"
	      ],
	      "r": 7.6,
	      "rc": 0,
	      "rd": "20170106",
	      "rsC": 0,
	      "sC": 31,
	      "t": "星球大战外传：侠盗一号",
	      "tCn": "星球大战外传：侠盗一号",
	      "tEn": "Rogue One: A Star Wars Story",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        },
	        {
	          "enum": 2,
	          "version": "3D"
	        },
	        {
	          "enum": 4,
	          "version": "IMAX3D"
	        },
	        {
	          "enum": 6,
	          "version": "中国巨幕"
	        }
	      ],
	      "wantedCount": 2603
	    },
	    {
	      "NearestCinemaCount": 7,
	      "NearestDay": 1486281600,
	      "NearestShowtimeCount": 19,
	      "aN1": "山新",
	      "aN2": "姚雷",
	      "cC": 7,
	      "commonSpecial": "",
	      "d": "80",
	      "dN": "邓伟锋",
	      "def": 0,
	      "id": 233227,
	      "img": "http://img5.mtime.cn/mt/2017/01/17/173909.17348918_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "动画 / 奇幻 / 冒险",
	      "p": [
	        "动画奇幻冒险"
	      ],
	      "r": -1,
	      "rc": 0,
	      "rd": "20170205",
	      "rsC": 0,
	      "sC": 23,
	      "t": "萤火奇兵",
	      "tCn": "萤火奇兵",
	      "tEn": "Lighting Dindin",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 179
	    },
	    {
	      "NearestCinemaCount": 10,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 10,
	      "aN1": "马特·达蒙",
	      "aN2": "景甜",
	      "cC": 10,
	      "commonSpecial": "来自张艺谋的视觉饕餮盛宴",
	      "d": "104",
	      "dN": "张艺谋",
	      "def": 0,
	      "id": 153307,
	      "img": "http://img5.mtime.cn/mt/2016/11/22/113324.88618874_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": true,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": true,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "奇幻 / 冒险 / 动作",
	      "p": [
	        "奇幻冒险动作"
	      ],
	      "r": 7,
	      "rc": 0,
	      "rd": "20161216",
	      "rsC": 0,
	      "sC": 13,
	      "t": "长城",
	      "tCn": "长城",
	      "tEn": "The Great Wall",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 2,
	          "version": "3D"
	        },
	        {
	          "enum": 4,
	          "version": "IMAX3D"
	        },
	        {
	          "enum": 6,
	          "version": "中国巨幕"
	        }
	      ],
	      "wantedCount": 4827
	    },
	    {
	      "NearestCinemaCount": 4,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 7,
	      "aN1": "神木隆之介",
	      "aN2": "上白石萌音",
	      "cC": 4,
	      "commonSpecial": "穿越时空的遇见",
	      "d": "106",
	      "dN": "新海诚",
	      "def": 0,
	      "id": 232556,
	      "img": "http://img5.mtime.cn/mt/2016/11/07/120120.49850874_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "动画 / 剧情 / 爱情",
	      "p": [
	        "动画剧情爱情"
	      ],
	      "r": 8.4,
	      "rc": 0,
	      "rd": "20161202",
	      "rsC": 0,
	      "sC": 7,
	      "t": "你的名字。",
	      "tCn": "你的名字。",
	      "tEn": "Your Name",
	      "ua": -1,
	      "versions": [],
	      "wantedCount": 6210
	    },
	    {
	      "NearestCinemaCount": 3,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 5,
	      "aN1": "葛优",
	      "aN2": "章子怡",
	      "cC": 3,
	      "commonSpecial": "奢华洋场浮世绘，荒唐岁月生死局",
	      "d": "118",
	      "dN": "程耳",
	      "def": 0,
	      "id": 208911,
	      "img": "http://img5.mtime.cn/mt/2016/12/12/150729.93784100_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "剧情 / 动作 / 悬疑",
	      "p": [
	        "剧情动作悬疑"
	      ],
	      "r": 7.5,
	      "rc": 0,
	      "rd": "20161216",
	      "rsC": 0,
	      "sC": 6,
	      "t": "罗曼蒂克消亡史",
	      "tCn": "罗曼蒂克消亡史",
	      "tEn": "The Wasted Times",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 1594
	    },
	    {
	      "NearestCinemaCount": 2,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 3,
	      "aN1": "海伦·米伦",
	      "aN2": "艾伦·里克曼",
	      "cC": 2,
	      "commonSpecial": "一手杀人一手救人的道德困境",
	      "d": "102",
	      "dN": "加文·胡德",
	      "def": 0,
	      "id": 217924,
	      "img": "http://img5.mtime.cn/mt/2017/01/06/145246.10284065_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "战争 / 剧情 / 悬疑",
	      "p": [
	        "战争剧情悬疑"
	      ],
	      "r": 7.5,
	      "rc": 0,
	      "rd": "20170113",
	      "rsC": 0,
	      "sC": 3,
	      "t": "天空之眼",
	      "tCn": "天空之眼",
	      "tEn": "Eye in the Sky",
	      "ua": -1,
	      "versions": [],
	      "wantedCount": 602
	    },
	    {
	      "NearestCinemaCount": 2,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 2,
	      "aN1": "成龙",
	      "aN2": "黄子韬",
	      "cC": 2,
	      "commonSpecial": "铁道版《虎口脱险》够搞笑",
	      "d": "123",
	      "dN": "丁晟",
	      "def": 0,
	      "id": 225093,
	      "img": "http://img5.mtime.cn/mt/2016/12/12/115745.33946817_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "动作 / 喜剧",
	      "p": [
	        "动作喜剧"
	      ],
	      "r": 6,
	      "rc": 0,
	      "rd": "20161223",
	      "rsC": 0,
	      "sC": 2,
	      "t": "铁道飞虎",
	      "tCn": "铁道飞虎",
	      "tEn": "Railroad Tigers",
	      "ua": -1,
	      "versions": [],
	      "wantedCount": 1288
	    },
	    {
	      "NearestCinemaCount": 1,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 1,
	      "aN1": "殷果儿",
	      "aN2": "任青安",
	      "cC": 1,
	      "commonSpecial": "",
	      "d": "0",
	      "dN": "陆诗雷",
	      "def": 0,
	      "id": 236440,
	      "img": "http://img5.mtime.cn/mt/2016/12/06/174556.65409347_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": true,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": true,
	      "m": "",
	      "movieType": "惊悚 / 恐怖",
	      "p": [
	        "惊悚恐怖"
	      ],
	      "r": 4.9,
	      "rc": 0,
	      "rd": "20170106",
	      "rsC": 0,
	      "sC": 2,
	      "t": "恐怖理发店",
	      "tCn": "恐怖理发店",
	      "tEn": "Ghost In Barber's",
	      "ua": -1,
	      "versions": [],
	      "wantedCount": 389
	    },
	    {
	      "NearestCinemaCount": 1,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 2,
	      "aN1": "韩立",
	      "aN2": "彭波",
	      "cC": 1,
	      "commonSpecial": "",
	      "d": "0",
	      "dN": "赵宏丽",
	      "def": 0,
	      "id": 228494,
	      "img": "http://img5.mtime.cn/mt/2016/11/16/145411.50809496_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": false,
	      "m": "",
	      "movieType": "剧情",
	      "p": [
	        "剧情"
	      ],
	      "r": 4,
	      "rc": 0,
	      "rd": "20170124",
	      "rsC": 0,
	      "sC": 2,
	      "t": "老师也疯狂",
	      "tCn": "老师也疯狂",
	      "tEn": "Crazy Teacher",
	      "ua": -1,
	      "versions": [],
	      "wantedCount": 13
	    },
	    {
	      "NearestCinemaCount": 1,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 1,
	      "aN1": "易烊千玺",
	      "aN2": "陈志荣",
	      "cC": 1,
	      "commonSpecial": "憨萌笨小猪拯救世界",
	      "d": "90",
	      "dN": "陆锦明",
	      "def": 0,
	      "id": 237793,
	      "img": "http://img5.mtime.cn/mt/2016/12/15/101730.19629483_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": false,
	      "m": "",
	      "movieType": "动画",
	      "p": [
	        "动画"
	      ],
	      "r": 5.6,
	      "rc": 0,
	      "rd": "20170107",
	      "rsC": 0,
	      "sC": 1,
	      "t": "猪猪侠之英雄猪少年",
	      "tCn": "猪猪侠之英雄猪少年",
	      "tEn": "Zhu Zhu Xia Zhi Ying Xiong Zhu Shao Nian",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 2,
	          "version": "3D"
	        }
	      ],
	      "wantedCount": 146
	    },
	    {
	      "NearestCinemaCount": 1,
	      "NearestDay": 1486108800,
	      "NearestShowtimeCount": 1,
	      "aN1": "李雪健",
	      "aN2": "",
	      "cC": 1,
	      "commonSpecial": "",
	      "d": "0",
	      "dN": "田壮壮",
	      "def": 0,
	      "id": 21379,
	      "img": "http://img31.mtime.cn/mt/2014/02/23/005911.34508686_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": false,
	      "m": "",
	      "movieType": "",
	      "p": [],
	      "r": -1,
	      "rc": 0,
	      "rd": "0",
	      "rsC": 0,
	      "sC": 1,
	      "t": "鼓书艺人",
	      "tCn": "鼓书艺人",
	      "tEn": "Gu Shu Yi Ren",
	      "ua": -1,
	      "versions": [],
	      "wantedCount": 12
	    },
	    {
	      "NearestCinemaCount": 1,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 1,
	      "aN1": "董子健",
	      "aN2": "李梦",
	      "cC": 1,
	      "commonSpecial": "董子健演绎血性工厂江湖",
	      "d": "96",
	      "dN": "相国强",
	      "def": 0,
	      "id": 215665,
	      "img": "http://img5.mtime.cn/mt/2017/01/09/143916.25458584_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": false,
	      "m": "",
	      "movieType": "喜剧 / 爱情",
	      "p": [
	        "喜剧爱情"
	      ],
	      "r": 6.9,
	      "rc": 0,
	      "rd": "20170113",
	      "rsC": 0,
	      "sC": 1,
	      "t": "少年巴比伦",
	      "tCn": "少年巴比伦",
	      "tEn": "Young Love Lost",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 194
	    },
	    {
	      "NearestCinemaCount": 1,
	      "NearestDay": 1486022400,
	      "NearestShowtimeCount": 1,
	      "aN1": "雅玫",
	      "aN2": "董博睿",
	      "cC": 1,
	      "commonSpecial": "",
	      "d": "90",
	      "dN": "石英杰",
	      "def": 0,
	      "id": 236495,
	      "img": "http://img5.mtime.cn/mt/2016/12/15/093519.84177012_1280X720X2.jpg",
	      "is3D": false,
	      "isDMAX": false,
	      "isFilter": false,
	      "isHot": false,
	      "isIMAX": false,
	      "isIMAX3D": false,
	      "isNew": false,
	      "isTicket": false,
	      "m": "",
	      "movieType": "爱情 / 悬疑",
	      "p": [
	        "爱情悬疑"
	      ],
	      "r": 5.4,
	      "rc": 0,
	      "rd": "20161223",
	      "rsC": 0,
	      "sC": 1,
	      "t": "有迹可循",
	      "tCn": "有迹可循",
	      "tEn": "The Writing's On The Wall",
	      "ua": -1,
	      "versions": [
	        {
	          "enum": 1,
	          "version": "2D"
	        }
	      ],
	      "wantedCount": 113
	    }
	  ],
	  "newActivitiesTime": 0,
	  "totalComingMovie": 39,
	  "voucherMsg": ""
	}

解析：

- `bImg`：???
- `date`：日期
- `lid`：`ms` 数量 x 10？
- `ms`：具体正在热映电影信息
- `aN1`：演员1
- `aN2`：演员2
- `cC`：今日上映该电影的影院数量，同`NearestCinemaCount`
- `d`：影片时长
- `dN`：导演
- `def`：???
- `id`：影片 id，需要提供给[影片详情](#movie_detail)
- `r`：影片评分
- `rd`：影片上映时间
- `sC`：
- `t`：影片名
- `tCn`：影片中文名
- `tEn`：影片英文名
- `versions`：影片观影类型，如 `3D`、`IMAX `等

<h2 id="coming_movies">即将上映</h2>
url：`https://api-m.mtime.cn/Movie/MovieComingNew.api?locationId=?`

示例 url：[`https://api-m.mtime.cn/Movie/MovieComingNew.api?locationId=290`](https://api-m.mtime.cn/Movie/MovieComingNew.api?locationId=290)

json 示例：

	{
	  "attention": [
	    {
	      "actor1": "范·迪塞尔",
	      "actor2": "露比·罗丝",
	      "director": "D·J·卡卢索",
	      "id": 125805,
	      "image": "http://img5.mtime.cn/mt/2017/01/05/105822.16893974_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": true,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 10,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月10日上映",
	      "title": "极限特工：终极回归",
	      "type": "动作 / 冒险 / 惊悚",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/05/105124.83548335.jpg",
	          "length": 30,
	          "title": "极限特工：终极回归 中国版预告片",
	          "url": "http://vf.test.com/Video/2017/01/05/mp4/170105105137886980.mp4",
	          "videoId": 64107
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/02/082857.54680705.jpg",
	          "length": 139,
	          "title": "极限特工：终极回归 中文版终极预告片",
	          "url": "http://vf.test.com/Video/2016/11/02/mp4/161102083059175649.mp4",
	          "videoId": 63180
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/08/05/122731.94053608.jpg",
	          "length": 91,
	          "title": "极限特工：终极回归 中文版预告片",
	          "url": "http://vf.test.com/Video/2016/08/05/mp4/160805122727094193.mp4",
	          "videoId": 61933
	        }
	      ],
	      "wantedCount": 1359
	    },
	    {
	      "actor1": "葛优",
	      "actor2": "谢霆锋",
	      "director": "叶伟民",
	      "id": 232595,
	      "image": "http://img5.mtime.cn/mt/2017/01/10/090134.10115693_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": true,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 10,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月10日上映",
	      "title": "决战食神",
	      "type": "喜剧 / 爱情 / 家庭",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/04/26/130539.79110460.jpg",
	          "length": 188,
	          "title": "锋味江湖之决战食神 开机发布会",
	          "url": "http://vf.test.com/Video/2016/04/26/mp4/160426131314147202.mp4",
	          "videoId": 60087
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/28/152019.33593663.jpg",
	          "length": 93,
	          "title": "决战食神 对决版预告",
	          "url": "http://vf.test.com/Video/2016/11/28/mp4/161128151943156157.mp4",
	          "videoId": 63534
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/27/080931.62471310.jpg",
	          "length": 80,
	          "title": "决战食神  有味儿版预告",
	          "url": "http://vf.test.com/Video/2016/12/27/mp4/161227080852691154.mp4",
	          "videoId": 63981
	        }
	      ],
	      "wantedCount": 259
	    },
	    {
	      "actor1": "瑞恩·高斯林",
	      "actor2": "艾玛·斯通",
	      "director": "达米恩·查泽雷",
	      "id": 219784,
	      "image": "http://img5.mtime.cn/mt/2017/01/13/095311.48058459_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": true,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 14,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月14日上映",
	      "title": "爱乐之城",
	      "type": "爱情 / 喜剧 / 剧情",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/10/080204.77068894.jpg",
	          "length": 132,
	          "title": "爱乐之城 中国版预告片",
	          "url": "http://vf.test.com/Video/2017/01/10/mp4/170110080203660654.mp4",
	          "videoId": 64188
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/04/070429.48900078.jpg",
	          "length": 147,
	          "title": "爱乐之城 预告片",
	          "url": "http://vf.test.com/Video/2016/11/04/mp4/161104070413693181.mp4",
	          "videoId": 63219
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/07/14/083144.32810880.jpg",
	          "length": 86,
	          "title": "爱乐之城 先行版预告片1",
	          "url": "http://vf.test.com/Video/2016/07/14/mp4/160714082904505185.mp4",
	          "videoId": 61438
	        }
	      ],
	      "wantedCount": 1371
	    },
	    {
	      "actor1": "马修·麦康纳",
	      "actor2": "瑞茜·威瑟斯彭",
	      "director": "加斯·詹宁斯",
	      "id": 229728,
	      "image": "http://img5.mtime.cn/mt/2017/01/18/115740.32791274_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 17,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月17日上映",
	      "title": "欢乐好声音",
	      "type": "动画 / 喜剧 / 剧情",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/09/120830.38309775.jpg",
	          "length": 60,
	          "title": "欢乐好声音 中国版预告片",
	          "url": "http://vf.test.com/Video/2017/01/09/mp4/170109121029869887.mp4",
	          "videoId": 64157
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/03/082831.82160305.jpg",
	          "length": 133,
	          "title": "欢乐好声音 中文版预告片2",
	          "url": "http://vf.test.com/Video/2016/11/03/mp4/161103082405038369.mp4",
	          "videoId": 63203
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/10/09/111950.82422468.jpg",
	          "length": 168,
	          "title": "欢乐好声音 中文版预告片",
	          "url": "http://vf.test.com/Video/2016/10/09/mp4/161009111843862501.mp4",
	          "videoId": 62827
	        }
	      ],
	      "wantedCount": 541
	    },
	    {
	      "actor1": "迈克尔·法斯宾德",
	      "actor2": "玛丽昂·歌迪亚",
	      "director": "贾斯汀·库泽尔",
	      "id": 200591,
	      "image": "http://img31.mtime.cn/mt/2016/08/22/142519.84905467_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 24,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月24日上映",
	      "title": "刺客信条",
	      "type": "动作 / 冒险 / 奇幻",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/05/12/123050.65070378.jpg",
	          "length": 137,
	          "title": "刺客信条 预告片",
	          "url": "http://vf.test.com/Video/2016/05/12/mp4/160512123454502023.mp4",
	          "videoId": 60337
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/10/18/212902.44518364.jpg",
	          "length": 158,
	          "title": "刺客信条 预告片2",
	          "url": "http://vf.test.com/Video/2016/10/18/mp4/161018212137309833.mp4",
	          "videoId": 62966
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/10/30/105044.10933663.jpg",
	          "length": 90,
	          "title": "刺客信条 台湾版预告片",
	          "url": "http://vf.test.com/Video/2016/10/30/mp4/161030104432537780.mp4",
	          "videoId": 63143
	        }
	      ],
	      "wantedCount": 1702
	    },
	    {
	      "actor1": "威尔·阿奈特",
	      "actor2": "迈克尔·塞拉",
	      "director": "克里斯·麦凯",
	      "id": 223948,
	      "image": "http://img5.mtime.cn/mt/2017/01/25/142342.49345371_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 3,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月3日上映",
	      "title": "乐高蝙蝠侠大电影",
	      "type": "动画 / 喜剧 / 动作",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/25/111724.11559334.jpg",
	          "length": 119,
	          "title": "乐高蝙蝠侠大电影 中国版预告片",
	          "url": "http://vf.test.com/Video/2017/01/25/mp4/170125111142633999.mp4",
	          "videoId": 64387
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/03/29/085302.53590565.jpg",
	          "length": 109,
	          "title": "乐高蝙蝠侠大电影 中文版先行预告片",
	          "url": "http://vf.test.com/Video/2016/03/29/mp4/160329085241405800.mp4",
	          "videoId": 59641
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/03/25/080636.72674037.jpg",
	          "length": 136,
	          "title": "乐高蝙蝠侠大电影 先行版预告片1",
	          "url": "http://vf.test.com/Video/2016/03/25/mp4/160325080408679403.mp4",
	          "videoId": 59591
	        }
	      ],
	      "wantedCount": 176
	    },
	    {
	      "actor1": "杜天皓",
	      "actor2": "闫妮",
	      "director": "黄美娜",
	      "id": 238265,
	      "image": "http://img5.mtime.cn/mt/2017/01/06/103911.39785227_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 10,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月10日上映",
	      "title": "美容针",
	      "type": "爱情 / 剧情",
	      "videoCount": 1,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/09/134440.69569620.jpg",
	          "length": 77,
	          "title": "美容针 先导预告片",
	          "url": "http://vf.test.com/Video/2017/01/09/mp4/170109134511076173.mp4",
	          "videoId": 64162
	        }
	      ],
	      "wantedCount": 13
	    },
	    {
	      "actor1": "艾玛·沃森",
	      "actor2": "丹·史蒂文斯",
	      "director": "比尔·康顿",
	      "id": 195064,
	      "image": "http://img5.mtime.cn/mt/2017/01/25/112231.90243502_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 17,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月17日上映",
	      "title": "美女与野兽",
	      "type": "家庭 / 奇幻 / 歌舞",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/25/110418.66504658.jpg",
	          "length": 50,
	          "title": "美女与野兽 定档预告主创贺新春",
	          "url": "http://vf.test.com/Video/2017/01/25/mp4/170125110000333356.mp4",
	          "videoId": 64386
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/05/23/202306.44054536.jpg",
	          "length": 92,
	          "title": "美女与野兽 中文版先行预告片",
	          "url": "http://vf.test.com/Video/2016/05/23/mp4/160523202946551232.mp4",
	          "videoId": 60582
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/05/24/094538.98948511.jpg",
	          "length": 90,
	          "title": "美女与野兽 先行版预告片",
	          "url": "http://vf.test.com/Video/2016/05/24/mp4/160524094520169056.mp4",
	          "videoId": 60589
	        }
	      ],
	      "wantedCount": 896
	    },
	    {
	      "actor1": "孔维一",
	      "actor2": "张晨",
	      "director": "张大磊",
	      "id": 234857,
	      "image": "http://img5.mtime.cn/mt/2017/01/20/094746.43579809_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 24,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月24日上映",
	      "title": "八月",
	      "type": "剧情",
	      "videoCount": 2,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/20/195200.22581533.jpg",
	          "length": 82,
	          "title": "八月 预告片",
	          "url": "http://vf.test.com/Video/2016/11/20/mp4/161120195237258006.mp4",
	          "videoId": 63414
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/04/205630.38657752.jpg",
	          "length": 61,
	          "title": "八月 金马征途",
	          "url": "http://vf.test.com/Video/2016/12/04/mp4/161204205849707431.mp4",
	          "videoId": 63627
	        }
	      ],
	      "wantedCount": 143
	    }
	  ],
	  "moviecomings": [
	    {
	      "actor1": "贾乃亮",
	      "actor2": "马丽",
	      "director": "郭大雷",
	      "id": 230769,
	      "image": "http://img5.mtime.cn/mt/2017/01/16/104630.29361196_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": true,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 3,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月3日上映",
	      "title": "东北往事之破马张飞",
	      "type": "喜剧",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/01/211216.75603152.jpg",
	          "length": 58,
	          "title": "东北往事之破马张飞 先行版预告片",
	          "url": "http://vf.test.com/Video/2016/11/01/mp4/161101211204394445.mp4",
	          "videoId": 63176
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/06/215919.97317974.jpg",
	          "length": 89,
	          "title": "东北往事之破马张飞 剧情版预告片",
	          "url": "http://vf.test.com/Video/2016/12/06/mp4/161206215730098083.mp4",
	          "videoId": 63664
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/29/153033.28636603.jpg",
	          "length": 53,
	          "title": "东北往事之破马张飞 彩蛋之为金士杰庆生",
	          "url": "http://vf.test.com/Video/2016/12/29/mp4/161229153012984378.mp4",
	          "videoId": 64028
	        }
	      ],
	      "wantedCount": 1677
	    },
	    {
	      "actor1": "山新",
	      "actor2": "姚雷",
	      "director": "邓伟锋",
	      "id": 233227,
	      "image": "http://img5.mtime.cn/mt/2017/01/17/173909.17348918_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": true,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 5,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月5日上映",
	      "title": "萤火奇兵",
	      "type": "动画 / 奇幻 / 冒险",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/06/29/142348.49429265.jpg",
	          "length": 84,
	          "title": "萤火奇兵 预告片",
	          "url": "http://vf.test.com/Video/2016/06/29/mp4/160629142150295349.mp4",
	          "videoId": 61192
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/07/20/114328.48612333.jpg",
	          "length": 45,
	          "title": "萤火奇兵 先行版预告片",
	          "url": "http://vf.test.com/Video/2016/07/20/mp4/160720114306954253.mp4",
	          "videoId": 61554
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/09/14/132405.13320533.jpg",
	          "length": 93,
	          "title": "预告片2",
	          "url": "http://vf.test.com/Video/2016/09/14/mp4/160914132505167172.mp4",
	          "videoId": 62519
	        }
	      ],
	      "wantedCount": 179
	    },
	    {
	      "actor1": "萨沙·杰克逊",
	      "actor2": "Douglas Tait",
	      "director": "Ethan Wiley",
	      "id": 179087,
	      "image": "http://img5.mtime.cn/mt/2017/01/22/101602.66957401_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 10,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月10日上映",
	      "title": "大脚印",
	      "type": "动作 / 冒险 / 家庭",
	      "videoCount": 1,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/24/175822.56021018.jpg",
	          "length": 64,
	          "title": "大脚印 预告片",
	          "url": "http://vf.test.com/Video/2017/01/24/mp4/170124175549311772.mp4",
	          "videoId": 64381
	        }
	      ],
	      "wantedCount": 1696
	    },
	    {
	      "actor1": "范·迪塞尔",
	      "actor2": "露比·罗丝",
	      "director": "D·J·卡卢索",
	      "id": 125805,
	      "image": "http://img5.mtime.cn/mt/2017/01/05/105822.16893974_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": true,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 10,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月10日上映",
	      "title": "极限特工：终极回归",
	      "type": "动作 / 冒险 / 惊悚",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/05/105124.83548335.jpg",
	          "length": 30,
	          "title": "极限特工：终极回归 中国版预告片",
	          "url": "http://vf.test.com/Video/2017/01/05/mp4/170105105137886980.mp4",
	          "videoId": 64107
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/02/082857.54680705.jpg",
	          "length": 139,
	          "title": "极限特工：终极回归 中文版终极预告片",
	          "url": "http://vf.test.com/Video/2016/11/02/mp4/161102083059175649.mp4",
	          "videoId": 63180
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/08/05/122731.94053608.jpg",
	          "length": 91,
	          "title": "极限特工：终极回归 中文版预告片",
	          "url": "http://vf.test.com/Video/2016/08/05/mp4/160805122727094193.mp4",
	          "videoId": 61933
	        }
	      ],
	      "wantedCount": 1359
	    },
	    {
	      "actor1": "何润东",
	      "actor2": "黄子韬",
	      "director": "高希希",
	      "id": 233535,
	      "image": "http://img5.mtime.cn/mt/2016/12/05/153815.74562620_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 10,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月10日上映",
	      "title": "遊戏规则",
	      "type": "动作 / 剧情",
	      "videoCount": 2,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/06/16/152732.23953199.jpg",
	          "length": 97,
	          "title": "游戏规则 先行版预告片",
	          "url": "http://vf.test.com/Video/2016/06/16/mp4/160616152730378213.mp4",
	          "videoId": 60979
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/25/151653.92063165.jpg",
	          "length": 119,
	          "title": "遊戏规则 剧场版预告片",
	          "url": "http://vf.test.com/Video/2016/11/25/mp4/161125152138922169.mp4",
	          "videoId": 63504
	        }
	      ],
	      "wantedCount": 1298
	    },
	    {
	      "actor1": "葛优",
	      "actor2": "谢霆锋",
	      "director": "叶伟民",
	      "id": 232595,
	      "image": "http://img5.mtime.cn/mt/2017/01/10/090134.10115693_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": true,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 10,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月10日上映",
	      "title": "决战食神",
	      "type": "喜剧 / 爱情 / 家庭",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/04/26/130539.79110460.jpg",
	          "length": 188,
	          "title": "锋味江湖之决战食神 开机发布会",
	          "url": "http://vf.test.com/Video/2016/04/26/mp4/160426131314147202.mp4",
	          "videoId": 60087
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/28/152019.33593663.jpg",
	          "length": 93,
	          "title": "决战食神 对决版预告",
	          "url": "http://vf.test.com/Video/2016/11/28/mp4/161128151943156157.mp4",
	          "videoId": 63534
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/27/080931.62471310.jpg",
	          "length": 80,
	          "title": "决战食神  有味儿版预告",
	          "url": "http://vf.test.com/Video/2016/12/27/mp4/161227080852691154.mp4",
	          "videoId": 63981
	        }
	      ],
	      "wantedCount": 259
	    },
	    {
	      "actor1": "夏望",
	      "actor2": "李子雄",
	      "director": "",
	      "id": 240182,
	      "image": "http://img5.mtime.cn/mt/2017/01/20/105413.34786978_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 12,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月12日上映",
	      "title": "一树一树紫花开",
	      "type": "爱情 / 剧情",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 2
	    },
	    {
	      "actor1": "瑞恩·高斯林",
	      "actor2": "艾玛·斯通",
	      "director": "达米恩·查泽雷",
	      "id": 219784,
	      "image": "http://img5.mtime.cn/mt/2017/01/13/095311.48058459_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": true,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 14,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月14日上映",
	      "title": "爱乐之城",
	      "type": "爱情 / 喜剧 / 剧情",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/10/080204.77068894.jpg",
	          "length": 132,
	          "title": "爱乐之城 中国版预告片",
	          "url": "http://vf.test.com/Video/2017/01/10/mp4/170110080203660654.mp4",
	          "videoId": 64188
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/04/070429.48900078.jpg",
	          "length": 147,
	          "title": "爱乐之城 预告片",
	          "url": "http://vf.test.com/Video/2016/11/04/mp4/161104070413693181.mp4",
	          "videoId": 63219
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/07/14/083144.32810880.jpg",
	          "length": 86,
	          "title": "爱乐之城 先行版预告片1",
	          "url": "http://vf.test.com/Video/2016/07/14/mp4/160714082904505185.mp4",
	          "videoId": 61438
	        }
	      ],
	      "wantedCount": 1371
	    },
	    {
	      "actor1": "郑秀文",
	      "actor2": "张孝全",
	      "director": "刘国楠",
	      "id": 226111,
	      "image": "http://img5.mtime.cn/mt/2017/01/13/102812.15847759_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 14,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月14日上映",
	      "title": "合约男女",
	      "type": "爱情",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/09/102812.66314537.jpg",
	          "length": 87,
	          "title": "《合约男女》定档预告",
	          "url": "http://vf.test.com/Video/2016/12/09/mp4/161209103056602834.mp4",
	          "videoId": 63713
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/09/104151.27832696.jpg",
	          "length": 49,
	          "title": "合约男女 “郑宗孝料”版预告",
	          "url": "http://vf.test.com/Video/2017/01/09/mp4/170109104238449585.mp4",
	          "videoId": 64155
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/15/153012.47982064.jpg",
	          "length": 108,
	          "title": "合约男女 惊天喜地特辑",
	          "url": "http://vf.test.com/Video/2016/12/15/mp4/161215153044122592.mp4",
	          "videoId": 63811
	        }
	      ],
	      "wantedCount": 83
	    },
	    {
	      "actor1": "何炅",
	      "actor2": "钟欣潼",
	      "director": "刘镇伟",
	      "id": 210222,
	      "image": "http://img5.mtime.cn/mt/2016/12/14/110142.40460044_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 14,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月14日上映",
	      "title": "仙球大战",
	      "type": "喜剧 / 古装",
	      "videoCount": 1,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/05/104421.63593269.jpg",
	          "length": 72,
	          "title": "仙球大战 喜剧版预告",
	          "url": "http://vf.test.com/Video/2017/01/05/mp4/170105104351158407.mp4",
	          "videoId": 64106
	        }
	      ],
	      "wantedCount": 65
	    },
	    {
	      "actor1": "岳云鹏",
	      "actor2": "袁姗姗",
	      "director": "钟少雄",
	      "id": 239825,
	      "image": "http://img5.mtime.cn/mt/2017/01/18/101635.58143459_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 14,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月14日上映",
	      "title": "疯岳撬佳人",
	      "type": "喜剧",
	      "videoCount": 1,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/18/104623.32646400.jpg",
	          "length": 41,
	          "title": "疯岳撬佳人 预告片",
	          "url": "http://vf.test.com/Video/2017/01/18/mp4/170118104842125665.mp4",
	          "videoId": 64281
	        }
	      ],
	      "wantedCount": 12
	    },
	    {
	      "actor1": "潘思羽",
	      "actor2": "李英勋",
	      "director": "",
	      "id": 239778,
	      "image": "http://img5.mtime.cn/mt/2017/01/16/102850.35044867_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 14,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月14日上映",
	      "title": "欧爸的情人",
	      "type": "爱情",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 2
	    },
	    {
	      "actor1": "马修·麦康纳",
	      "actor2": "瑞茜·威瑟斯彭",
	      "director": "加斯·詹宁斯",
	      "id": 229728,
	      "image": "http://img5.mtime.cn/mt/2017/01/18/115740.32791274_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 17,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月17日上映",
	      "title": "欢乐好声音",
	      "type": "动画 / 喜剧 / 剧情",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/09/120830.38309775.jpg",
	          "length": 60,
	          "title": "欢乐好声音 中国版预告片",
	          "url": "http://vf.test.com/Video/2017/01/09/mp4/170109121029869887.mp4",
	          "videoId": 64157
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/03/082831.82160305.jpg",
	          "length": 133,
	          "title": "欢乐好声音 中文版预告片2",
	          "url": "http://vf.test.com/Video/2016/11/03/mp4/161103082405038369.mp4",
	          "videoId": 63203
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/10/09/111950.82422468.jpg",
	          "length": 168,
	          "title": "欢乐好声音 中文版预告片",
	          "url": "http://vf.test.com/Video/2016/10/09/mp4/161009111843862501.mp4",
	          "videoId": 62827
	        }
	      ],
	      "wantedCount": 541
	    },
	    {
	      "actor1": "姜武",
	      "actor2": "蒋勤勤",
	      "director": "梁栋",
	      "id": 234954,
	      "image": "http://img5.mtime.cn/mt/2017/01/26/112251.75944569_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 17,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月17日上映",
	      "title": "完美有多美",
	      "type": "爱情 / 奇幻 / 喜剧",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/06/16/101124.95605116.jpg",
	          "length": 42,
	          "title": "完美有多美 先行版预告片",
	          "url": "http://vf.test.com/Video/2016/06/16/mp4/160616101221920272.mp4",
	          "videoId": 60971
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/23/181151.30836037.jpg",
	          "length": 62,
	          "title": "完美有多美 奇幻人生版预告",
	          "url": "http://vf.test.com/Video/2016/11/23/mp4/161123181155825874.mp4",
	          "videoId": 63473
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/03/192259.83000033.jpg",
	          "length": 77,
	          "title": "完美有多美 趣味人生版预告",
	          "url": "http://vf.test.com/Video/2017/01/03/mp4/170103192222431403.mp4",
	          "videoId": 64083
	        }
	      ],
	      "wantedCount": 413
	    },
	    {
	      "actor1": "夏嘉伟",
	      "actor2": "洪剑涛",
	      "director": "夏嘉伟",
	      "id": 239047,
	      "image": "http://img5.mtime.cn/mt/2017/01/12/093035.12849907_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 18,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月18日上映",
	      "title": "来自月亮的我",
	      "type": "爱情 / 奇幻",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 3
	    },
	    {
	      "actor1": "迈克尔·法斯宾德",
	      "actor2": "玛丽昂·歌迪亚",
	      "director": "贾斯汀·库泽尔",
	      "id": 200591,
	      "image": "http://img31.mtime.cn/mt/2016/08/22/142519.84905467_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 24,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月24日上映",
	      "title": "刺客信条",
	      "type": "动作 / 冒险 / 奇幻",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/05/12/123050.65070378.jpg",
	          "length": 137,
	          "title": "刺客信条 预告片",
	          "url": "http://vf.test.com/Video/2016/05/12/mp4/160512123454502023.mp4",
	          "videoId": 60337
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/10/18/212902.44518364.jpg",
	          "length": 158,
	          "title": "刺客信条 预告片2",
	          "url": "http://vf.test.com/Video/2016/10/18/mp4/161018212137309833.mp4",
	          "videoId": 62966
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/10/30/105044.10933663.jpg",
	          "length": 90,
	          "title": "刺客信条 台湾版预告片",
	          "url": "http://vf.test.com/Video/2016/10/30/mp4/161030104432537780.mp4",
	          "videoId": 63143
	        }
	      ],
	      "wantedCount": 1702
	    },
	    {
	      "actor1": "王宁",
	      "actor2": "葛天",
	      "director": "袁杰",
	      "id": 237679,
	      "image": "http://img5.mtime.cn/mt/2016/12/19/180103.80869963_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 24,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月24日上映",
	      "title": "咸鱼传奇",
	      "type": "剧情 / 喜剧",
	      "videoCount": 1,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/18/172548.20649995.jpg",
	          "length": 111,
	          "title": "咸鱼传奇 预告片",
	          "url": "http://vf.test.com/Video/2016/11/18/mp4/161118172534976511.mp4",
	          "videoId": 63406
	        }
	      ],
	      "wantedCount": 244
	    },
	    {
	      "actor1": "余男",
	      "actor2": "凤小岳",
	      "director": "胡雪桦",
	      "id": 215124,
	      "image": "http://img5.mtime.cn/mt/2017/01/17/095545.70547471_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 24,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月24日上映",
	      "title": "上海王",
	      "type": "爱情 / 动作 / 犯罪",
	      "videoCount": 2,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/15/101927.61737226.jpg",
	          "length": 99,
	          "title": "上海王 预告片",
	          "url": "http://vf.test.com/Video/2016/12/15/mp4/161215102003162029.mp4",
	          "videoId": 63805
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/16/192806.56138681.jpg",
	          "length": 110,
	          "title": "上海王 定档预告片",
	          "url": "http://vf.test.com/Video/2017/01/16/mp4/170116192721397685.mp4",
	          "videoId": 64263
	        }
	      ],
	      "wantedCount": 175
	    },
	    {
	      "actor1": "张韶涵",
	      "actor2": "方力申",
	      "director": "雷宇扬",
	      "id": 221560,
	      "image": "http://img5.mtime.cn/mt/2016/12/19/094109.68221541_1280X720X2.jpg",
	      "isFilter": true,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 24,
	      "rMonth": 2,
	      "rYear": 2017,
	      "releaseDate": "2月24日上映",
	      "title": "碟仙诡谭2",
	      "type": "惊悚 / 剧情 / 恐怖",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 109
	    },
	    {
	      "actor1": "何乙轩",
	      "actor2": "辉灿",
	      "director": "王俊潾",
	      "id": 236890,
	      "image": "http://img5.mtime.cn/mt/2017/01/10/172252.85744895_1280X720X2.jpg",
	      "isFilter": true,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 3,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月3日上映",
	      "title": "惊魂绣花鞋",
	      "type": "惊悚 / 恐怖",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 385
	    },
	    {
	      "actor1": "威尔·阿奈特",
	      "actor2": "迈克尔·塞拉",
	      "director": "克里斯·麦凯",
	      "id": 223948,
	      "image": "http://img5.mtime.cn/mt/2017/01/25/142342.49345371_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 3,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月3日上映",
	      "title": "乐高蝙蝠侠大电影",
	      "type": "动画 / 喜剧 / 动作",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/25/111724.11559334.jpg",
	          "length": 119,
	          "title": "乐高蝙蝠侠大电影 中国版预告片",
	          "url": "http://vf.test.com/Video/2017/01/25/mp4/170125111142633999.mp4",
	          "videoId": 64387
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/03/29/085302.53590565.jpg",
	          "length": 109,
	          "title": "乐高蝙蝠侠大电影 中文版先行预告片",
	          "url": "http://vf.test.com/Video/2016/03/29/mp4/160329085241405800.mp4",
	          "videoId": 59641
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/03/25/080636.72674037.jpg",
	          "length": 136,
	          "title": "乐高蝙蝠侠大电影 先行版预告片1",
	          "url": "http://vf.test.com/Video/2016/03/25/mp4/160325080408679403.mp4",
	          "videoId": 59591
	        }
	      ],
	      "wantedCount": 176
	    },
	    {
	      "actor1": "杜天皓",
	      "actor2": "闫妮",
	      "director": "黄美娜",
	      "id": 238265,
	      "image": "http://img5.mtime.cn/mt/2017/01/06/103911.39785227_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 10,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月10日上映",
	      "title": "美容针",
	      "type": "爱情 / 剧情",
	      "videoCount": 1,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/09/134440.69569620.jpg",
	          "length": 77,
	          "title": "美容针 先导预告片",
	          "url": "http://vf.test.com/Video/2017/01/09/mp4/170109134511076173.mp4",
	          "videoId": 64162
	        }
	      ],
	      "wantedCount": 13
	    },
	    {
	      "actor1": "艾伦",
	      "actor2": "王自健",
	      "director": "王宁",
	      "id": 240235,
	      "image": "http://img5.mtime.cn/mt/2017/01/23/193811.24340437_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 10,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月10日上映",
	      "title": "玛格丽特的春天",
	      "type": "喜剧",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 5
	    },
	    {
	      "actor1": "余男",
	      "actor2": "凤小岳",
	      "director": "胡雪桦",
	      "id": 232228,
	      "image": "http://img5.mtime.cn/mt/2017/01/17/094527.56599243_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 16,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月16日上映",
	      "title": "上海王Ⅱ",
	      "type": "剧情",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 320
	    },
	    {
	      "actor1": "艾玛·沃森",
	      "actor2": "丹·史蒂文斯",
	      "director": "比尔·康顿",
	      "id": 195064,
	      "image": "http://img5.mtime.cn/mt/2017/01/25/112231.90243502_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "美国",
	      "rDay": 17,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月17日上映",
	      "title": "美女与野兽",
	      "type": "家庭 / 奇幻 / 歌舞",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/25/110418.66504658.jpg",
	          "length": 50,
	          "title": "美女与野兽 定档预告主创贺新春",
	          "url": "http://vf.test.com/Video/2017/01/25/mp4/170125110000333356.mp4",
	          "videoId": 64386
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/05/23/202306.44054536.jpg",
	          "length": 92,
	          "title": "美女与野兽 中文版先行预告片",
	          "url": "http://vf.test.com/Video/2016/05/23/mp4/160523202946551232.mp4",
	          "videoId": 60582
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img31.mtime.cn/mg/2016/05/24/094538.98948511.jpg",
	          "length": 90,
	          "title": "美女与野兽 先行版预告片",
	          "url": "http://vf.test.com/Video/2016/05/24/mp4/160524094520169056.mp4",
	          "videoId": 60589
	        }
	      ],
	      "wantedCount": 896
	    },
	    {
	      "actor1": "王佑硕",
	      "actor2": "伊娜",
	      "director": "高育新",
	      "id": 239179,
	      "image": "http://img5.mtime.cn/mt/2017/01/06/173613.26293516_1280X720X2.jpg",
	      "isFilter": true,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 17,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月17日上映",
	      "title": "碟仙前传",
	      "type": "惊悚 / 恐怖",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 3
	    },
	    {
	      "actor1": "张蓝艺",
	      "actor2": "刘一辰",
	      "director": "摩撒利",
	      "id": 240095,
	      "image": "http://img5.mtime.cn/mt/2017/01/18/175522.62803379_1280X720X2.jpg",
	      "isFilter": true,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 17,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月17日上映",
	      "title": "通灵姐妹",
	      "type": "惊悚 / 恐怖",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 1
	    },
	    {
	      "actor1": "孔维一",
	      "actor2": "张晨",
	      "director": "张大磊",
	      "id": 234857,
	      "image": "http://img5.mtime.cn/mt/2017/01/20/094746.43579809_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 24,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月24日上映",
	      "title": "八月",
	      "type": "剧情",
	      "videoCount": 2,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/20/195200.22581533.jpg",
	          "length": 82,
	          "title": "八月 预告片",
	          "url": "http://vf.test.com/Video/2016/11/20/mp4/161120195237258006.mp4",
	          "videoId": 63414
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/04/205630.38657752.jpg",
	          "length": 61,
	          "title": "八月 金马征途",
	          "url": "http://vf.test.com/Video/2016/12/04/mp4/161204205849707431.mp4",
	          "videoId": 63627
	        }
	      ],
	      "wantedCount": 143
	    },
	    {
	      "actor1": "李漫荻",
	      "actor2": "齐炫宇",
	      "director": "程中豪",
	      "id": 225824,
	      "image": "http://img5.mtime.cn/mt/2017/01/24/143434.20935571_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 24,
	      "rMonth": 3,
	      "rYear": 2017,
	      "releaseDate": "3月24日上映",
	      "title": "碟仙实录",
	      "type": "惊悚",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 141
	    },
	    {
	      "actor1": "王凯",
	      "actor2": "张鲁一",
	      "director": "苏有朋",
	      "id": 229559,
	      "image": "http://img5.mtime.cn/mt/2017/01/17/160533.74141556_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 1,
	      "rMonth": 4,
	      "rYear": 2017,
	      "releaseDate": "4月1日上映",
	      "title": "嫌疑人X的献身",
	      "type": "剧情 / 悬疑",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/27/104523.93427911.jpg",
	          "length": 59,
	          "title": "嫌疑人X的献身 先行版预告片",
	          "url": "http://vf.test.com/Video/2016/12/27/mp4/161227104957669123.mp4",
	          "videoId": 63991
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/28/141517.96667541.jpg",
	          "length": 60,
	          "title": "嫌疑人X的献身 预告之苏有朋王宝强拜年",
	          "url": "http://vf.test.com/Video/2017/01/28/mp4/170128141620861748.mp4",
	          "videoId": 64407
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/22/095806.41648209.jpg",
	          "length": 68,
	          "title": "嫌疑人X的献身 导演特辑",
	          "url": "http://vf.test.com/Video/2017/01/22/mp4/170122100037436433.mp4",
	          "videoId": 64340
	        }
	      ],
	      "wantedCount": 125
	    },
	    {
	      "actor1": "白百何",
	      "actor2": "黄立行",
	      "director": "徐静蕾",
	      "id": 230023,
	      "image": "http://img5.mtime.cn/mt/2016/12/22/102817.82245509_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 1,
	      "rMonth": 4,
	      "rYear": 2017,
	      "releaseDate": "4月1日上映",
	      "title": "绑架者",
	      "type": "动作 / 犯罪",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 21
	    },
	    {
	      "actor1": "范伟",
	      "actor2": "贾静雯",
	      "director": "王啸坤",
	      "id": 235312,
	      "image": "http://img5.mtime.cn/mt/2016/12/01/181116.49722505_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 1,
	      "rMonth": 4,
	      "rYear": 2017,
	      "releaseDate": "4月1日上映",
	      "title": "有完没完",
	      "type": "喜剧",
	      "videoCount": 1,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/01/180642.47863811.jpg",
	          "length": 96,
	          "title": "有完没完 先导预告",
	          "url": "http://vf.test.com/Video/2016/12/01/mp4/161201180604968347.mp4",
	          "videoId": 63590
	        }
	      ],
	      "wantedCount": 20
	    },
	    {
	      "actor1": "黄轩",
	      "actor2": "段奕宏",
	      "director": "麦兆辉",
	      "id": 238038,
	      "image": "http://img5.mtime.cn/mt/2016/12/10/155946.61412202_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 1,
	      "rMonth": 4,
	      "rYear": 2017,
	      "releaseDate": "4月1日上映",
	      "title": "非凡任务",
	      "type": "动作 / 犯罪",
	      "videoCount": 3,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/12/10/163648.55628100.jpg",
	          "length": 63,
	          "title": "非凡任务 定档预告片",
	          "url": "http://vf.test.com/Video/2016/12/10/mp4/161210163607609153.mp4",
	          "videoId": 63746
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/16/130234.70843791.jpg",
	          "length": 30,
	          "title": "非凡任务 预告片之“以毒攻毒”",
	          "url": "http://vf.test.com/Video/2017/01/16/mp4/170116130209623257.mp4",
	          "videoId": 64253
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2017/01/17/220531.24014653.jpg",
	          "length": 91,
	          "title": "非凡任务 制作特辑之血肉火光",
	          "url": "http://vf.test.com/Video/2017/01/17/mp4/170117220511628715.mp4",
	          "videoId": 64278
	        }
	      ],
	      "wantedCount": 17
	    },
	    {
	      "actor1": "李诚儒",
	      "actor2": "王姬",
	      "director": "李诚儒",
	      "id": 236426,
	      "image": "http://img31.mtime.cn/mt/2016/08/30/143750.18410565_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "",
	      "rDay": 1,
	      "rMonth": 4,
	      "rYear": 2017,
	      "releaseDate": "4月1日上映",
	      "title": "大导归来",
	      "type": "喜剧",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 3
	    },
	    {
	      "actor1": "殷果儿",
	      "actor2": "黄梓城",
	      "director": "陆诗雷",
	      "id": 240098,
	      "image": "http://img5.mtime.cn/mt/2017/01/19/144035.50538009_1280X720X2.jpg",
	      "isFilter": true,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 1,
	      "rMonth": 4,
	      "rYear": 2017,
	      "releaseDate": "4月1日上映",
	      "title": "恐怖电影院2",
	      "type": "惊悚 / 恐怖",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 1
	    },
	    {
	      "actor1": "",
	      "actor2": "",
	      "director": "",
	      "id": 239083,
	      "image": "http://img5.mtime.cn/mt/2017/01/04/173023.52332967_1280X720X2.jpg",
	      "isFilter": true,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 14,
	      "rMonth": 4,
	      "rYear": 2017,
	      "releaseDate": "4月14日上映",
	      "title": "怨灵宿舍之白纸女生",
	      "type": "惊悚 / 恐怖",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 2
	    },
	    {
	      "actor1": "黄渤",
	      "actor2": "徐静蕾",
	      "director": "陈正道",
	      "id": 233371,
	      "image": "http://img5.mtime.cn/mt/2016/11/20/232349.42198888_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": true,
	      "locationName": "中国",
	      "rDay": 28,
	      "rMonth": 4,
	      "rYear": 2017,
	      "releaseDate": "4月28日上映",
	      "title": "记忆大师",
	      "type": "剧情 / 悬疑",
	      "videoCount": 2,
	      "videos": [
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/20/230117.88259394.jpg",
	          "length": 92,
	          "title": "记忆大师 先行版预告片",
	          "url": "http://vf.test.com/Video/2016/11/20/mp4/161120230220539135.mp4",
	          "videoId": 63415
	        },
	        {
	          "hightUrl": "",
	          "image": "http://img5.mtime.cn/mg/2016/11/23/194434.38545702.jpg",
	          "length": 109,
	          "title": "记忆大师 定档发布会",
	          "url": "http://vf.test.com/Video/2016/11/23/mp4/161123194827200179.mp4",
	          "videoId": 63475
	        }
	      ],
	      "wantedCount": 199
	    },
	    {
	      "actor1": "黄磊",
	      "actor2": "李立群",
	      "director": "黄磊",
	      "id": 237670,
	      "image": "http://img5.mtime.cn/mt/2017/01/18/095513.39940063_1280X720X2.jpg",
	      "isFilter": false,
	      "isTicket": false,
	      "isVideo": false,
	      "locationName": "中国",
	      "rDay": 28,
	      "rMonth": 4,
	      "rYear": 2017,
	      "releaseDate": "4月28日上映",
	      "title": "麻烦家族",
	      "type": "喜剧 / 家庭",
	      "videoCount": 0,
	      "videos": [],
	      "wantedCount": 7
	    }
	  ]
	}

解析：

首先大体分为两个部分 ——

- `attention`：最受关注
- `moviecomings`：即将上映

接下来就是里面具体的字段：

- `videos`：预告片，不过我们无权访问

<h2 id="movie_roles">演职员表</h2>

url：`https://api-m.mtime.cn/Movie/MovieCreditsWithTypes.api?movieId=?`

示例 url：[`https://api-m.mtime.cn/Movie/MovieCreditsWithTypes.api?movieId=217896`](https://api-m.mtime.cn/Movie/MovieCreditsWithTypes.api?movieId=217896)

json 示例：

	{
	  "types": [
	    {
	      "typeName": "导演",
	      "typeNameEn": "Director",
	      "persons": [
	        {
	          "id": 892951,
	          "name": "唐季礼",
	          "nameEn": "Stanley Tong",
	          "image": "http://img31.mtime.cn/ph/2014/02/22/192821.88623670_1280X720X2.jpg"
	        }
	      ]
	    },
	    {
	      "typeName": "演员",
	      "typeNameEn": "Actor",
	      "persons": [
	        {
	          "id": 892908,
	          "name": "成龙",
	          "nameEn": "Jackie Chan",
	          "image": "http://img31.mtime.cn/ph/2014/02/28/112422.17365543_1280X720X2.jpg",
	          "personate": "Jack",
	          "personateCn": "",
	          "personateEn": "Jack",
	          "roleCover": "http://img5.mtime.cn/mg/2017/01/11/145413.83105118_120X120X4.jpg"
	        },
	        {
	          "id": 1706195,
	          "name": "李治廷",
	          "nameEn": "Aarif Lee",
	          "image": "http://img31.mtime.cn/ph/2016/08/29/141047.77357073_1280X720X2.jpg",
	          "personate": "李琼斯",
	          "personateCn": "李琼斯",
	          "personateEn": "",
	          "roleCover": "http://img5.mtime.cn/mg/2017/01/11/145626.54701937_120X120X4.jpg"
	        },
	        {
	          "id": 2064407,
	          "name": "张艺兴",
	          "nameEn": "Lay",
	          "image": "http://img31.mtime.cn/ph/2014/08/27/104030.26360119_1280X720X2.jpg",
	          "personate": "小光",
	          "personateCn": "小光",
	          "personateEn": "",
	          "roleCover": "http://img5.mtime.cn/mg/2017/01/11/145804.83807897_120X120X4.jpg"
	        },
	        {
	          "id": 2203563,
	          "name": "母其弥雅",
	          "nameEn": "Miya Muqi",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/095911.30364656_1280X720X2.jpg",
	          "personate": "诺敏",
	          "personateCn": "诺敏",
	          "personateEn": "Nuomin",
	          "roleCover": "http://img5.mtime.cn/mg/2017/01/11/150412.43179613_120X120X4.jpg"
	        },
	        {
	          "id": 1140379,
	          "name": "索努·苏德",
	          "nameEn": "Sonu Sood",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/095224.40512168_1280X720X2.jpg",
	          "personate": "Randall",
	          "personateCn": "",
	          "personateEn": "Randall",
	          "roleCover": "http://img5.mtime.cn/mg/2017/01/11/150056.25650637_120X120X4.jpg"
	        },
	        {
	          "id": 2203562,
	          "name": "迪莎·帕塔尼",
	          "nameEn": "Disha Patani",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/094546.99646978_1280X720X2.jpg",
	          "personate": "Ashmita",
	          "personateCn": "",
	          "personateEn": "Ashmita",
	          "roleCover": "http://img5.mtime.cn/mg/2017/01/11/150524.40491808_120X120X4.jpg"
	        },
	        {
	          "id": 893302,
	          "name": "曾志伟",
	          "nameEn": "Eric Tsang",
	          "image": "http://img31.mtime.cn/ph/2016/08/28/113831.10100344_1280X720X2.jpg",
	          "personate": "",
	          "personateCn": "",
	          "personateEn": ""
	        },
	        {
	          "id": 2059040,
	          "name": "艾米拉·达斯特",
	          "nameEn": "Amyra Dastur",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/094454.55559449_1280X720X2.jpg",
	          "personate": "Kyra",
	          "personateCn": "",
	          "personateEn": "Kyra"
	        },
	        {
	          "id": 2161891,
	          "name": "尚语贤",
	          "nameEn": "Yuxian Shang",
	          "image": "http://img31.mtime.cn/ph/2015/09/08/162552.82189307_1280X720X2.jpg",
	          "personate": "",
	          "personateCn": "",
	          "personateEn": ""
	        },
	        {
	          "id": 1951559,
	          "name": "姜雯",
	          "nameEn": "Coco",
	          "image": "http://img31.mtime.cn/ph/2016/08/29/105432.78324758_1280X720X2.jpg",
	          "personate": "",
	          "personateCn": "",
	          "personateEn": ""
	        },
	        {
	          "id": 1732882,
	          "name": "",
	          "nameEn": "Aarif Lee",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/095621.93396396_1280X720X2.jpg",
	          "personate": "Jones Lee",
	          "personateCn": "",
	          "personateEn": "Jones Lee"
	        },
	        {
	          "id": 2203564,
	          "name": "",
	          "nameEn": "Yixing Zhang",
	          "image": "http://img31.mtime.cn/ph/1564/2203564/2203564_1280X720X2.jpg",
	          "personate": "Xiaoguang",
	          "personateCn": "",
	          "personateEn": "Xiaoguang"
	        },
	        {
	          "id": 2203565,
	          "name": "",
	          "nameEn": "Ágúst Bjarnason",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/100330.15393071_1280X720X2.jpg",
	          "personate": "Snowmobile henchman       (as Agust Bjarnason)",
	          "personateCn": "",
	          "personateEn": "Snowmobile henchman       (as Agust Bjarnason)"
	        },
	        {
	          "id": 1312004,
	          "name": "",
	          "nameEn": "Damian Mavis",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/100501.64422583_1280X720X2.jpg",
	          "personate": "Mercenary",
	          "personateCn": "",
	          "personateEn": "Mercenary"
	        },
	        {
	          "id": 2091930,
	          "name": "托默·奥兹",
	          "nameEn": "Tomer Oz",
	          "image": "http://img31.mtime.cn/ph/2016/06/13/105506.61299409_1280X720X2.jpg",
	          "personate": "Hit Man",
	          "personateCn": "",
	          "personateEn": "Hit Man"
	        },
	        {
	          "id": 2195708,
	          "name": "",
	          "nameEn": "Adam St",
	          "image": "http://img31.mtime.cn/ph/2016/06/01/114914.77959182_1280X720X2.jpg",
	          "personate": "Body Guard       (as Adam St)",
	          "personateCn": "",
	          "personateEn": "Body Guard       (as Adam St)"
	        },
	        {
	          "id": 2091931,
	          "name": "乔尔·阿德里安",
	          "nameEn": "Joel Adrian",
	          "image": "http://img31.mtime.cn/ph/2016/06/13/105635.20225670_1280X720X2.jpg",
	          "personate": "Hit Man",
	          "personateCn": "",
	          "personateEn": "Hit Man"
	        },
	        {
	          "id": 1963992,
	          "name": "保罗·菲利普·克拉克",
	          "nameEn": "Paul Philip Clark",
	          "image": "http://img31.mtime.cn/ph/2016/06/13/105605.23569309_1280X720X2.jpg",
	          "personate": "Max",
	          "personateCn": "",
	          "personateEn": "Max"
	        },
	        {
	          "id": 2203566,
	          "name": "",
	          "nameEn": "Najmeddin AlHadad",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/100807.53877810_1280X720X2.jpg",
	          "personate": "Hit Man",
	          "personateCn": "",
	          "personateEn": "Hit Man"
	        },
	        {
	          "id": 1968854,
	          "name": "",
	          "nameEn": "Eskindir Tesfay",
	          "image": "http://img31.mtime.cn/ph/854/1968854/1968854_1280X720X2.jpg",
	          "personate": "Mercenary",
	          "personateCn": "",
	          "personateEn": "Mercenary"
	        },
	        {
	          "id": 939396,
	          "name": "张国立",
	          "nameEn": "Guoli Zhang",
	          "image": "http://img31.mtime.cn/ph/2016/08/25/111854.90067184_1280X720X2.jpg",
	          "personate": "",
	          "personateCn": "",
	          "personateEn": ""
	        },
	        {
	          "id": 2015518,
	          "name": "",
	          "nameEn": "Fatih Ugurlu",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/101109.33845987_1280X720X2.jpg",
	          "personate": "Randall's Man",
	          "personateCn": "",
	          "personateEn": "Randall's Man"
	        },
	        {
	          "id": 2203567,
	          "name": "",
	          "nameEn": "Alessio Miano",
	          "image": "http://img31.mtime.cn/ph/1567/2203567/2203567_1280X720X2.jpg",
	          "personate": "Hit Man",
	          "personateCn": "",
	          "personateEn": "Hit Man"
	        },
	        {
	          "id": 1503568,
	          "name": "胡明",
	          "nameEn": "Ming Hu",
	          "image": "http://img31.mtime.cn/ph/2014/04/23/095827.42282773_1280X720X2.jpg",
	          "personate": "",
	          "personateCn": "",
	          "personateEn": ""
	        },
	        {
	          "id": 2203568,
	          "name": "",
	          "nameEn": "Erika Herbert",
	          "image": "http://img31.mtime.cn/ph/2016/08/30/101259.25589888_1280X720X2.jpg",
	          "personate": "Mother       (uncredited)",
	          "personateCn": "",
	          "personateEn": "Mother       (uncredited)"
	        },
	        {
	          "id": 1749911,
	          "name": "马铁摩",
	          "nameEn": "Temur Mamisashvili",
	          "image": "http://img31.mtime.cn/ph/2016/06/13/105235.33616709_1280X720X2.jpg",
	          "personate": "Hit Man",
	          "personateCn": "",
	          "personateEn": "Hit Man"
	        },
	        {
	          "id": 2104097,
	          "name": "凯文·李",
	          "nameEn": "Kevin Lee",
	          "image": "http://img31.mtime.cn/ph/2015/04/03/115050.53836684_1280X720X2.jpg",
	          "personate": "Hit Man",
	          "personateCn": "",
	          "personateEn": "Hit Man"
	        },
	        {
	          "id": 2175554,
	          "name": "",
	          "nameEn": "Sajjad Delafrooz",
	          "image": "http://img31.mtime.cn/ph/1554/2175554/2175554_1280X720X2.jpg",
	          "personate": "Rich man in Hotel",
	          "personateCn": "",
	          "personateEn": "Rich man in Hotel"
	        },
	        {
	          "id": 1963993,
	          "name": "",
	          "nameEn": "David Torok",
	          "image": "http://img31.mtime.cn/ph/1993/1963993/1963993_1280X720X2.jpg",
	          "personate": "Hit Man",
	          "personateCn": "",
	          "personateEn": "Hit Man"
	        },
	        {
	          "id": 2112626,
	          "name": "",
	          "nameEn": "Matthew Ray Ruggles",
	          "image": "http://img31.mtime.cn/ph/626/2112626/2112626_1280X720X2.jpg",
	          "personate": "Auctioneer",
	          "personateCn": "",
	          "personateEn": "Auctioneer"
	        },
	        {
	          "id": 2209365,
	          "name": "达伦·格罗夫纳",
	          "nameEn": "Darren Grosvenor",
	          "image": "http://img31.mtime.cn/ph/2016/06/21/093053.97975829_1280X720X2.jpg",
	          "personate": "Randall's Accountant",
	          "personateCn": "",
	          "personateEn": "Randall's Accountant"
	        },
	        {
	          "id": 2227722,
	          "name": "",
	          "nameEn": "Franz Rügamer",
	          "image": "http://img31.mtime.cn/ph/1722/2227722/2227722_1280X720X2.jpg",
	          "personate": "Bodyguard",
	          "personateCn": "",
	          "personateEn": "Bodyguard"
	        },
	        {
	          "id": 2227723,
	          "name": "",
	          "nameEn": "Ebrahim Hassan",
	          "image": "http://img31.mtime.cn/ph/1723/2227723/2227723_1280X720X2.jpg",
	          "personate": "Hit Man",
	          "personateCn": "",
	          "personateEn": "Hit Man"
	        },
	        {
	          "id": 2227724,
	          "name": "",
	          "nameEn": "Anthony Gavard",
	          "image": "http://img31.mtime.cn/ph/1724/2227724/2227724_1280X720X2.jpg",
	          "personate": "Auction presenter",
	          "personateCn": "",
	          "personateEn": "Auction presenter"
	        },
	        {
	          "id": 2227725,
	          "name": "",
	          "nameEn": "Joshua Linder",
	          "image": "http://img31.mtime.cn/ph/1725/2227725/2227725_1280X720X2.jpg",
	          "personate": "Hit Man",
	          "personateCn": "",
	          "personateEn": "Hit Man"
	        },
	        {
	          "id": 2129733,
	          "name": "成家班",
	          "nameEn": "Jiaban Cheng",
	          "image": "http://img31.mtime.cn/ph/1733/2129733/2129733_1280X720X2.jpg",
	          "personate": "",
	          "personateCn": "",
	          "personateEn": ""
	        },
	        {
	          "id": 1951873,
	          "name": "",
	          "nameEn": "Paul Allica",
	          "image": "http://img31.mtime.cn/ph/1873/1951873/1951873_1280X720X2.jpg",
	          "personate": "Mercenary",
	          "personateCn": "",
	          "personateEn": "Mercenary"
	        }
	      ]
	    },
	    {
	      "typeName": "编剧",
	      "typeNameEn": "Writer",
	      "persons": [
	        {
	          "id": 892951,
	          "name": "唐季礼",
	          "nameEn": "Stanley Tong",
	          "image": "http://img31.mtime.cn/ph/2014/02/22/192821.88623670_1280X720X2.jpg"
	        }
	      ]
	    },
	    {
	      "typeName": "制作人",
	      "typeNameEn": "Produced by",
	      "persons": [
	        {
	          "id": 2038377,
	          "name": "",
	          "nameEn": "Maxine De Vere",
	          "image": "http://img31.mtime.cn/ph/377/2038377/2038377_1280X720X2.jpg"
	        },
	        {
	          "id": 1209821,
	          "name": "董韵诗",
	          "nameEn": "Barbie Tung",
	          "image": "http://img31.mtime.cn/ph/2016/09/05/174813.15229657_1280X720X2.jpg"
	        }
	      ]
	    },
	    {
	      "typeName": "美术设计",
	      "typeNameEn": "Art Direction by",
	      "persons": [
	        {
	          "id": 2203560,
	          "name": "",
	          "nameEn": "Zhen Wu",
	          "image": "http://img31.mtime.cn/ph/1560/2203560/2203560_1280X720X2.jpg"
	        }
	      ]
	    },
	    {
	      "typeName": "服装设计",
	      "typeNameEn": "Costume Design by",
	      "persons": [
	        {
	          "id": 1265610,
	          "name": "黄家仪",
	          "nameEn": "Phoebe Wong",
	          "image": "http://img31.mtime.cn/ph/1610/1265610/1265610_1280X720X2.jpg"
	        }
	      ]
	    },
	    {
	      "typeName": "视觉特效总监",
	      "typeNameEn": "Visual Effects Supervisor",
	      "persons": [
	        {
	          "id": 2239688,
	          "name": "",
	          "nameEn": "Khandu Bidkar",
	          "image": "http://img31.mtime.cn/ph/1688/2239688/2239688_1280X720X2.jpg"
	        }
	      ]
	    },
	    {
	      "typeName": "动作指导",
	      "typeNameEn": "Choreographer",
	      "persons": [
	        {
	          "id": 892951,
	          "name": "唐季礼",
	          "nameEn": "Stanley Tong",
	          "image": "http://img31.mtime.cn/ph/2014/02/22/192821.88623670_1280X720X2.jpg"
	        },
	        {
	          "id": 1865296,
	          "name": "伍刚",
	          "nameEn": "Gang Wu",
	          "image": "http://img5.mtime.cn/ph/2016/11/26/222616.41967971_1280X720X2.jpg"
	        }
	      ]
	    },
	    {
	      "typeName": "副导演/助理导演",
	      "typeNameEn": "Assistant Director",
	      "persons": [
	        {
	          "id": 1893463,
	          "name": "",
	          "nameEn": "James Cho",
	          "image": "http://img31.mtime.cn/ph/1463/1893463/1893463_1280X720X2.jpg"
	        },
	        {
	          "id": 1467335,
	          "name": "",
	          "nameEn": "Garun Danielsdottir",
	          "image": "http://img31.mtime.cn/ph/1335/1467335/1467335_1280X720X2.jpg"
	        },
	        {
	          "id": 1270086,
	          "name": "",
	          "nameEn": "Nicola Marzano",
	          "image": "http://img31.mtime.cn/ph/86/1270086/1270086_1280X720X2.jpg"
	        }
	      ]
	    },
	    {
	      "typeName": "声音部门",
	      "typeNameEn": "Sound Department",
	      "persons": [
	        {
	          "id": 2203561,
	          "name": "",
	          "nameEn": "Sindri Þór Kárason",
	          "image": "http://img31.mtime.cn/ph/1561/2203561/2203561_1280X720X2.jpg"
	        },
	        {
	          "id": 2227721,
	          "name": "",
	          "nameEn": "Skuli Helgi Sigurgislason",
	          "image": "http://img31.mtime.cn/ph/1721/2227721/2227721_1280X720X2.jpg"
	        }
	      ]
	    }
	  ]
	}

解析：

- `typeName`：已知取值有`导演`、`演员`、`编剧`等
- `typeNameEn`：`typeName` 字段对应的英文
- `persons`：具体人员信息
- `id`：人员 id
- `name`：人员姓名
- `nameEn`：人员英文名

以下字段是演员特有的：

- `image`：人员照片
- `personate`：饰演角色名
- `personateCn`：饰演角色名的中文名
- `personateEn`：饰演角色名的英文名
- `roleCover`：饰演角色剧照

人员详细信息 url：`https://ticket-api-m.mtime.cn/person/detail.api?personId=?&cityId=？`

示例 url：[`https://ticket-api-m.mtime.cn/person/detail.api?personId=892908&cityId=290`](https://ticket-api-m.mtime.cn/person/detail.api?personId=892908&cityId=290)

解析：就是上面获取到的人员 id 和你的地区 id 拼接上去就可以了，这里的内容挺多的，后期笔者再扩展

<h2 id="movie_detail">影片详情</h2>

url：`https://ticket-api-m.mtime.cn/movie/detail.api?locationId=?&movieId=?`

解析：其中 `locationId` 就不做多解释了，`movieId` 可以分别从[正在售票](#sell_tickets)、[正在热映](#hot_movies)、[即将上映](#coming_movies)对应 json 的 `movieId`、`id`、`id` 字段中获取

示例 url：[`https://ticket-api-m.mtime.cn/movie/detail.api?locationId=290&movieId=125805`](https://ticket-api-m.mtime.cn/movie/detail.api?locationId=290&movieId=125805)

json 示例：

	{
	  "code": "1",
	  "data": {
	    "advertisement": {
	      "advList": [
	        {
	          "advTag": "",
	          "endDate": 1514649599,
	          "isHorizontalScreen": false,
	          "isOpenH5": false,
	          "startDate": 1451577600,
	          "tag": "西游伏妖篇（票务）",
	          "type": "203",
	          "typeName": "影片详情页banner2",
	          "url": "https://static4da.mtime.cn/feature/mobile/banner/2017/0122/210.html"
	        }
	      ],
	      "count": 1,
	      "error": "",
	      "success": true
	    },
	    "basic": {
	      "actors": [
	        {
	          "actorId": 913378,
	          "img": "http://img31.mtime.cn/ph/2014/09/01/170748.64755972_1280X720X2.jpg",
	          "name": "范·迪塞尔",
	          "nameEn": "Vin Diesel",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/162613.85098094.jpg",
	          "roleName": "Xander Cage"
	        },
	        {
	          "actorId": 1763914,
	          "img": "http://img21.mtime.cn/ph/2010/06/25/094715.29791367_1280X720X2.jpg",
	          "name": "露比·罗丝",
	          "nameEn": "Ruby Rose",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/162801.28633700.jpg",
	          "roleName": "Adele Wolff"
	        },
	        {
	          "actorId": 1266158,
	          "img": "http://img31.mtime.cn/ph/2016/05/04/162943.45619387_1280X720X2.jpg",
	          "name": "妮娜·杜波夫",
	          "nameEn": "Nina Dobrev",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/163459.85286563.jpg",
	          "roleName": "Rebecca 'Becky'"
	        },
	        {
	          "actorId": 893008,
	          "img": "http://img31.mtime.cn/ph/2014/03/13/164116.22404345_1280X720X2.jpg",
	          "name": "甄子丹",
	          "nameEn": "Donnie Yen",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/162631.30237748.jpg",
	          "roleName": "Xiang"
	        },
	        {
	          "actorId": 1403701,
	          "img": "http://img31.mtime.cn/ph/2016/04/05/153734.26333599_1280X720X2.jpg",
	          "name": "迪皮卡·帕度柯妮",
	          "nameEn": "Deepika Padukone",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/163611.99195116.jpg",
	          "roleName": "Serena Unger"
	        },
	        {
	          "actorId": 913101,
	          "img": "http://img31.mtime.cn/ph/2014/03/14/152328.88324192_1280X720X2.jpg",
	          "name": "塞缪尔·杰克逊",
	          "nameEn": "Samuel L. Jackson",
	          "roleImg": "",
	          "roleName": "Agent Augustus Eugene Gibbons"
	        },
	        {
	          "actorId": 938310,
	          "img": "http://img31.mtime.cn/ph/2014/02/22/202102.28239250_1280X720X2.jpg",
	          "name": "托尼·贾",
	          "nameEn": "Tony Jaa",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/163434.84663336.jpg",
	          "roleName": "Talon"
	        },
	        {
	          "actorId": 1981491,
	          "img": "http://img31.mtime.cn/ph/2016/06/15/141117.21300390_1280X720X2.jpg",
	          "name": "吴亦凡",
	          "nameEn": "Kris Wu",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/162650.25424635.jpg",
	          "roleName": "Harvard"
	        },
	        {
	          "actorId": 915029,
	          "img": "http://img5.mtime.cn/ph/2017/01/12/165011.48068899_1280X720X2.jpg",
	          "name": "托妮·科莱特",
	          "nameEn": "Toni Collette",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/163402.87655748.jpg",
	          "roleName": "Jane Marke"
	        },
	        {
	          "actorId": 926008,
	          "img": "http://img31.mtime.cn/ph/2016/04/07/144735.68017937_1280X720X2.jpg",
	          "name": "罗伊·麦克凯恩",
	          "nameEn": "Rory McCann",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/163308.86236332.jpg",
	          "roleName": "Tennyson Torch"
	        },
	        {
	          "actorId": 2201494,
	          "img": "http://img5.mtime.cn/ph/2016/11/02/092530.84997401_1280X720X2.jpg",
	          "name": "尼基·詹姆",
	          "nameEn": "Nicky Jam",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/163152.53635568.jpg",
	          "roleName": "Lazarus"
	        },
	        {
	          "actorId": 2098727,
	          "img": "http://img31.mtime.cn/ph/2015/07/01/114143.59711468_1280X720X2.jpg",
	          "name": "内马尔",
	          "nameEn": "Neymar",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/163524.98203922.jpg",
	          "roleName": ""
	        },
	        {
	          "actorId": 1416487,
	          "img": "http://img31.mtime.cn/ph/2016/08/29/184141.26902742_1280X720X2.jpg",
	          "name": "",
	          "nameEn": "Michael Bisping",
	          "roleImg": "http://img5.mtime.cn/mg/2017/01/05/163040.43362207.jpg",
	          "roleName": "Hawk"
	        },
	        {
	          "actorId": 2084677,
	          "img": "http://img31.mtime.cn/ph/2015/09/09/101940.19419320_1280X720X2.jpg",
	          "name": "赫敏·科菲尔德",
	          "nameEn": "Hermione Corfield",
	          "roleImg": "",
	          "roleName": "Ainsley"
	        },
	        {
	          "actorId": 921201,
	          "img": "http://img31.mtime.cn/ph/2014/04/15/111254.75720606_1280X720X2.jpg",
	          "name": "艾尔·斯帕恩扎",
	          "nameEn": "Al Sapienza",
	          "roleImg": "",
	          "roleName": "CIA Director"
	        },
	        {
	          "actorId": 1232892,
	          "img": "http://img5.mtime.cn/ph/2017/01/05/145035.65755647_1280X720X2.jpg",
	          "name": "",
	          "nameEn": "Helena-Alexis Seymour",
	          "roleImg": "",
	          "roleName": "Ainsley's Girl #2"
	        },
	        {
	          "actorId": 2218074,
	          "img": "http://img31.mtime.cn/ph/2016/08/29/184313.10828827_1280X720X2.jpg",
	          "name": "",
	          "nameEn": "Megan Soo",
	          "roleImg": "",
	          "roleName": "Ainsley's Girl #4"
	        },
	        {
	          "actorId": 1165261,
	          "img": "http://img5.mtime.cn/ph/2017/01/05/144835.67747637_1280X720X2.jpg",
	          "name": "",
	          "nameEn": "Jonathan Whittaker",
	          "roleImg": "",
	          "roleName": "President"
	        },
	        {
	          "actorId": 2218075,
	          "img": "http://img5.mtime.cn/ph/2017/01/05/144739.37346974_1280X720X2.jpg",
	          "name": "",
	          "nameEn": "Kristen Kurnik",
	          "roleImg": "",
	          "roleName": "Ainsley's Girl #5"
	        },
	        {
	          "actorId": 1023991,
	          "img": "http://img5.mtime.cn/ph/2017/01/05/144625.10720932_1280X720X2.jpg",
	          "name": "",
	          "nameEn": "Gary 'Si-Jo' Foo",
	          "roleImg": "",
	          "roleName": "NSA Contractor"
	        }
	      ],
	      "award": {
	        "awardList": [],
	        "totalNominateAward": 0,
	        "totalWinAward": 0
	      },
	      "commentSpecial": "",
	      "community": {},
	      "director": {
	        "directorId": 903521,
	        "img": "http://img31.mtime.cn/ph/2016/09/02/144150.57291017_1280X720X2.jpg",
	        "name": "D·J·卡卢索",
	        "nameEn": "D.J. Caruso"
	      },
	      "festivals": [],
	      "hotRanking": 5,
	      "img": "http://img5.mtime.cn/mt/2017/01/05/105822.16893974_1280X720X2.jpg",
	      "is3D": true,
	      "isDMAX": true,
	      "isEggHunt": false,
	      "isFilter": false,
	      "isIMAX": false,
	      "isIMAX3D": true,
	      "isTicket": true,
	      "message": "该操作将清除您对该片的评分！是否确认？",
	      "mins": "107分钟",
	      "movieId": 125805,
	      "name": "极限特工：终极回归",
	      "nameEn": "xXx: The Return of Xander Cage",
	      "overallRating": -1,
	      "personCount": 123,
	      "quizGame": {},
	      "releaseArea": "中国",
	      "releaseDate": "20170210",
	      "showCinemaCount": 27,
	      "showDay": 1486627200,
	      "showtimeCount": 14,
	      "stageImg": {
	        "count": 124,
	        "list": [
	          {
	            "imgId": 7180661,
	            "imgUrl": "http://img31.mtime.cn/pi/2016/04/06/163644.66635601_1280X720X2.jpg"
	          },
	          {
	            "imgId": 7301637,
	            "imgUrl": "http://img5.mtime.cn/pi/2016/11/02/174909.42908242_1280X720X2.jpg"
	          },
	          {
	            "imgId": 7203067,
	            "imgUrl": "http://img31.mtime.cn/pi/2016/04/07/160807.83892239_1280X720X2.jpg"
	          },
	          {
	            "imgId": 7301211,
	            "imgUrl": "http://img5.mtime.cn/pi/2016/11/01/091327.68190533_1280X720X2.jpg"
	          }
	        ]
	      },
	      "story": "《极限特工3》将故事聚焦在由范·迪塞尔带头的的特工小队和以甄子丹为首的反派组织之间的对决。在这部作品中，迪塞尔饰演的特工凯奇不再是孤胆英雄，他将与一群出色的伙伴共同作战：塞缪尔·杰克逊饰演的国安局特工，印度女星迪皮卡·帕度柯妮饰演的与凯奇颇有渊源的女猎人，凭借《吸血鬼日记》走红的妮娜·杜波夫扮演的技术专家，《女子监狱》女星露比·罗丝饰演的狙击手，中国当红偶像演员吴亦凡饰演的特工Nicks。",
	      "style": {
	        "isLeadPage": 0,
	        "leadImg": "https://img2.mtime.cn/mg/.jpg",
	        "leadUrl": ""
	      },
	      "totalNominateAward": 0,
	      "totalWinAward": 0,
	      "type": [
	        "动作",
	        "冒险",
	        "惊悚"
	      ],
	      "url": "https://movie.mtime.com/125805/",
	      "video": {
	        "count": 18,
	        "hightUrl": "https://vfx.mtime.cn/Video/2017/01/05/mp4/170105105137886980.mp4",
	        "img": "http://img5.mtime.cn/mg/2017/01/05/105124.57142324_235X132X4.jpg",
	        "title": "极限特工：终极回归 中国版预告片",
	        "url": "https://vfx.mtime.cn/Video/2017/01/05/mp4/170105105137886980_480.mp4",
	        "videoId": 64107
	      }
	    },
	    "boxOffice": {
	      "movieId": 125805,
	      "ranking": 41,
	      "todayBox": 0,
	      "todayBoxDes": "",
	      "todayBoxDesUnit": "",
	      "totalBox": 0,
	      "totalBoxDes": "",
	      "totalBoxUnit": ""
	    },
	    "live": {},
	    "related": {
	      "goodsCount": 0,
	      "goodsList": [],
	      "relateId": 0,
	      "relatedUrl": "https://mall-wv.mtime.cn/#!/commerce/list/",
	      "type": 0
	    }
	  },
	  "msg": "成功",
	  "showMsg": ""
	}

解析：其中`advertisement`、`related`是无关字段，不做解析

- `basic`：具体内容
- `actors`：演员信息
- `actorId`：演员 id
- `img`：演员照片
- `name`：演员名
- `nameEn`：演员英文名
- `roleImg`：影片中饰演角色图片
- `roleName`：影片中饰演角色名字
- `award`：获得的奖项？
- `commentSpecial`：一句话总结该电影
- `community`：???
- `director`：导演信息
- `hotRanking`：热映排行榜
- `img`：剧照
- `releaseArea`：上映地区
- `stageImg`：影片剧照
- `story`：剧情简介
- `video`：预告片
- `boxOffice`：专业解读内容
- `ranking`：票房排名
- `todayBox`：今日实时票房量
- `todayBoxDes` 和 `todayBoxDesUnit`：今日实时票房量
- `totalBox` 和 `totalBoxUnit`：累计票房量

ps：这里还有一些字段没有解析，由于采样不够大，所以笔者也无法判断部分字段含义

<h2 id="movie_comment">影片评论</h2>

url：`https://ticket-api-m.mtime.cn/movie/hotComment.api?movieId=?`

示例 url：[`https://ticket-api-m.mtime.cn/movie/hotComment.api?movieId=125805`](https://ticket-api-m.mtime.cn/movie/hotComment.api?movieId=125805)

json 示例：

	{
	  "code": "1",
	  "data": {
	    "mini": {
	      "list": [
	        {
	          "commentDate": 1485949110,
	          "commentId": 41530503,
	          "content": "小小可惜，甄子丹已经过了最能打的年纪，倘若在杀破狼时期的话，甄子丹一定发挥的更好！",
	          "headImg": "//img32.mtime.cn/up/2016/04/21/164216.20185739_128X128.jpg",
	          "img": "",
	          "isHot": false,
	          "isPraise": false,
	          "locationName": "温哥华",
	          "nickname": "百家影评",
	          "praiseCount": 1,
	          "rating": 0,
	          "replyCount": 0
	        },
	        {
	          "commentDate": 1485103881,
	          "commentId": 41436292,
	          "content": "敢問吳先生於戲內之作用為......？",
	          "headImg": "//img32.mtime.cn/up/2014/02/20/145006.56345759_128X128.jpg",
	          "img": "",
	          "isHot": false,
	          "isPraise": false,
	          "locationName": "Macao",
	          "nickname": "pan88",
	          "praiseCount": 7,
	          "rating": 6.8,
	          "replyCount": 7
	        },
	        {
	          "commentDate": 1485085100,
	          "commentId": 41433946,
	          "content": "迪塞尔和甄子丹全程耍酷...吴亦凡的角色没什么存在感. 托尼贾也没有什么表现的机会. 剧情超级套路,看到开头就猜的差不多了. 看着有种低配版敢死队的感觉...尤其是第二部男主角出现的那一会",
	          "headImg": "/img2.mtime.cn/u/507/1116507/7427a21d-5bc2-4bf0-88b0-2036f6a83ce7/128X128.jpg",
	          "img": "",
	          "isHot": false,
	          "isPraise": false,
	          "locationName": "南昌",
	          "nickname": "冰封虾子",
	          "praiseCount": 0,
	          "rating": 7,
	          "replyCount": 0
	        }
	      ],
	      "total": 106
	    },
	    "plus": {
	      "list": [
	        {
	          "commentDate": 1468225860,
	          "commentId": 7967852,
	          "content": "\n常年锃光瓦亮的光头、一身健硕的肌肉、还有那永恒不变的T恤背心，这是一位令人为之惊讶、欢呼的糙汉，他便是范·迪塞尔。\n\n糙汉的《速激》人生\n\n\n\n提到老范，你最熟悉他哪部电影？那肯定没有其他答案，肯定是《速度与激情》系列了。\n这部全球最风靡的赛车题材系列电影起初的男一号是保罗·沃克饰演的卧底警察，但电影上映后人们发现，老范才是最吸引眼球的。\n拍摄《速度与激情2》时，老范因为档期原因没有参演，电影...",
	          "headImg": "//img32.mtime.cn/up/2013/06/26/161117.68950441_128X128.jpg",
	          "isWantSee": false,
	          "locationName": "",
	          "nickname": "冷子墨",
	          "rating": 7,
	          "replyCount": 4,
	          "title": "biubiubiu！看大汉玩转你的小心跳！——范·迪塞尔"
	        }
	      ],
	      "total": 2
	    }
	  },
	  "msg": "",
	  "showMsg": ""
	}

解析：

- `mini` 是短评，更多短评访问 url：[`https://api-m.mtime.cn/Showtime/HotMovieComments.api?pageIndex=1&movieId=217896`](https://api-m.mtime.cn/Showtime/HotMovieComments.api?pageIndex=1&movieId=217896)
- `plus` 是长评，更多长评访问 url：[`https://api-m.mtime.cn/Movie/HotLongComments.api?pageIndex=1&movieId=217896`](https://api-m.mtime.cn/Movie/HotLongComments.api?pageIndex=1&movieId=217896)
- `ca`：用户名
- `caimg`：用户头像
- `cal`：用户地区
- `cd`：用户评论时间
- `ce`：用户评论内容
- `ceimg`：评论内容中的图片地址
- `commentCount`：评论点赞量
- `cr`：用户评分
- `isHot`：是否是热门评论
- `tweetId`：???

<h2 id="trailer">预告片&拍摄花絮</h2>

url：`https://api-m.mtime.cn/Movie/Video.api?pageIndex=?&movieId=?`

示例 url：`https://api-m.mtime.cn/Movie/Video.api?pageIndex=1&movieId=217896`

解析：`pageIndex` 就是分页值，`movieId` 可以分别从[正在售票](#sell_tickets)、[正在热映](#hot_movies)、[即将上映](#coming_movies)对应 json 的 `movieId`、`id`、`id` 字段中获取

json 示例：

	{
	  "totalPageCount": 1,
	  "totalCount": 13,
	  "videoList": [
	    {
	      "id": 63236,
	      "url": "https://vfx.mtime.cn/Video/2016/11/06/mp4/161106175251674452_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2016/11/06/mp4/161106175251674452.mp4",
	      "image": "http://img5.mtime.cn/mg/2016/11/06/175108.73063349_235X132X4.jpg",
	      "title": "功夫瑜伽 先行版预告片",
	      "type": 0,
	      "length": 73
	    },
	    {
	      "id": 63798,
	      "url": "https://vfx.mtime.cn/Video/2016/12/14/mp4/161214210123816534_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2016/12/14/mp4/161214210123816534.mp4",
	      "image": "http://img5.mtime.cn/mg/2016/12/14/210343.18175212_235X132X4.jpg",
	      "title": "功夫瑜伽 “冰岛版”预告片",
	      "type": 0,
	      "length": 78
	    },
	    {
	      "id": 64069,
	      "url": "https://vfx.mtime.cn/Video/2017/01/03/mp4/170103113525291888_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2017/01/03/mp4/170103113525291888.mp4",
	      "image": "http://img5.mtime.cn/mg/2017/01/03/113548.24951108_235X132X4.jpg",
	      "title": "功夫瑜伽 印度版预告片",
	      "type": 0,
	      "length": 106
	    },
	    {
	      "id": 64218,
	      "url": "https://vfx.mtime.cn/Video/2017/01/12/mp4/170112140240922553_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2017/01/12/mp4/170112140240922553.mp4",
	      "image": "http://img5.mtime.cn/mg/2017/01/12/140320.88371998_235X132X4.jpg",
	      "title": "功夫瑜伽 迪拜版预告片",
	      "type": 0,
	      "length": 99
	    },
	    {
	      "id": 64284,
	      "url": "https://vfx.mtime.cn/Video/2017/01/18/mp4/170118113206598838_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2017/01/18/mp4/170118113206598838.mp4",
	      "image": "http://img5.mtime.cn/mg/2017/01/18/111104.16810177_235X132X4.jpg",
	      "title": "功夫瑜伽 主题曲MV",
	      "type": 0,
	      "length": 207
	    },
	    {
	      "id": 64356,
	      "url": "https://vfx.mtime.cn/Video/2017/01/23/mp4/170123112522947195_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2017/01/23/mp4/170123112522947195.mp4",
	      "image": "http://img5.mtime.cn/mg/2017/01/23/112537.91911011_235X132X4.jpg",
	      "title": "功夫瑜伽 小朋友专属预告片",
	      "type": 0,
	      "length": 89
	    },
	    {
	      "id": 64406,
	      "url": "https://vfx.mtime.cn/Video/2017/01/28/mp4/170128094656851772_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2017/01/28/mp4/170128094656851772.mp4",
	      "image": "http://img5.mtime.cn/mg/2017/01/28/094614.86140407_235X132X4.jpg",
	      "title": "功夫瑜伽 终极版预告片",
	      "type": 0,
	      "length": 127
	    },
	    {
	      "id": 63634,
	      "url": "https://vfx.mtime.cn/Video/2016/12/05/mp4/161205114045752200_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2016/12/05/mp4/161205114045752200.mp4",
	      "image": "http://img5.mtime.cn/mg/2016/12/05/114114.55326124_235X132X4.jpg",
	      "title": "功夫瑜伽 制作特辑之成龙",
	      "type": 2,
	      "length": 156
	    },
	    {
	      "id": 63903,
	      "url": "https://vfx.mtime.cn/Video/2016/12/21/mp4/161221110137243810_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2016/12/21/mp4/161221110137243810.mp4",
	      "image": "http://img5.mtime.cn/mg/2016/12/21/110219.83724407_235X132X4.jpg",
	      "title": "功夫瑜伽 特辑之功夫三傻",
	      "type": 2,
	      "length": 193
	    },
	    {
	      "id": 63986,
	      "url": "https://vfx.mtime.cn/Video/2016/12/27/mp4/161227095303140567_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2016/12/27/mp4/161227095303140567.mp4",
	      "image": "http://img5.mtime.cn/mg/2016/12/27/095237.96025557_235X132X4.jpg",
	      "title": "功夫瑜伽 特辑之印度大妈挑战中国大妈",
	      "type": 2,
	      "length": 87
	    },
	    {
	      "id": 64198,
	      "url": "https://vfx.mtime.cn/Video/2017/01/10/mp4/170110121037476449_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2017/01/10/mp4/170110121037476449.mp4",
	      "image": "http://img5.mtime.cn/mg/2017/01/10/120314.55459189_235X132X4.jpg",
	      "title": "功夫瑜伽 特辑之功夫三傻闹印度",
	      "type": 2,
	      "length": 220
	    },
	    {
	      "id": 64313,
	      "url": "https://vfx.mtime.cn/Video/2017/01/19/mp4/170119231711782382_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2017/01/19/mp4/170119231711782382.mp4",
	      "image": "http://img5.mtime.cn/mg/2017/01/19/231703.24454779_235X132X4.jpg",
	      "title": "功夫瑜伽 家宴",
	      "type": 4,
	      "length": 268
	    },
	    {
	      "id": 64022,
	      "url": "https://vfx.mtime.cn/Video/2016/12/29/mp4/161229112814109234_480.mp4",
	      "hightUrl": "https://vfx.mtime.cn/Video/2016/12/29/mp4/161229112814109234.mp4",
	      "image": "http://img5.mtime.cn/mg/2016/12/29/112817.18601940_235X132X4.jpg",
	      "title": "功夫瑜伽 主题曲MV",
	      "type": 5,
	      "length": 190
	    }
	  ]
	}

解析：

- `id`：预告片 id
- `url`：普通质量预告片链接
- `highUlr`：高质量预告片链接
- `img`：预告片图片
- `title`：预告片名称
- `type`：???
- `length`：预告片时长

<h2 id="stage_photo">剧照</h2>

url：`https://api-m.mtime.cn/Movie/ImageAll.api?movieId=?`

示例 url：[`https://api-m.mtime.cn/Movie/ImageAll.api?movieId=217896`](https://api-m.mtime.cn/Movie/ImageAll.api?movieId=217896)

json 示例：

	{
	  "images": [
	    {
	      "id": 7317312,
	      "image": "http://img5.mtime.cn/pi/2016/12/25/153213.67270192_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7323610,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/112857.23537009_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7323611,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/112901.48483314_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7288031,
	      "image": "http://img5.mtime.cn/pi/2016/09/27/100236.18479285_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7288032,
	      "image": "http://img5.mtime.cn/pi/2016/09/27/100309.34482906_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7288033,
	      "image": "http://img5.mtime.cn/pi/2016/09/27/100327.73956949_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7288034,
	      "image": "http://img5.mtime.cn/pi/2016/09/27/100343.59399776_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7288035,
	      "image": "http://img5.mtime.cn/pi/2016/09/27/100359.71284743_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7288036,
	      "image": "http://img5.mtime.cn/pi/2016/09/27/100417.94537188_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7304269,
	      "image": "http://img5.mtime.cn/pi/2016/11/14/094945.36759738_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7309785,
	      "image": "http://img5.mtime.cn/pi/2016/12/01/100955.65781749_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7309786,
	      "image": "http://img5.mtime.cn/pi/2016/12/01/100958.23254707_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7309787,
	      "image": "http://img5.mtime.cn/pi/2016/12/01/101001.50413875_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7309788,
	      "image": "http://img5.mtime.cn/pi/2016/12/01/101004.22993693_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7309789,
	      "image": "http://img5.mtime.cn/pi/2016/12/01/101009.16913162_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7309790,
	      "image": "http://img5.mtime.cn/pi/2016/12/01/101012.14415733_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7288030,
	      "image": "http://img5.mtime.cn/pi/2016/09/27/095732.34817739_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7304270,
	      "image": "http://img5.mtime.cn/pi/2016/11/14/095036.13955563_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7304271,
	      "image": "http://img5.mtime.cn/pi/2016/11/14/095039.60472997_1000X1000.jpg",
	      "type": 1
	    },
	    {
	      "id": 7308660,
	      "image": "http://img5.mtime.cn/pi/2016/11/28/103341.73539153_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7308661,
	      "image": "http://img5.mtime.cn/pi/2016/11/28/103345.73051395_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7308662,
	      "image": "http://img5.mtime.cn/pi/2016/11/28/103348.33837903_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7308663,
	      "image": "http://img5.mtime.cn/pi/2016/11/28/103350.83146023_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7308664,
	      "image": "http://img5.mtime.cn/pi/2016/11/28/103354.41292267_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7308665,
	      "image": "http://img5.mtime.cn/pi/2016/11/28/103357.81667685_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313339,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202630.66269199_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313340,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202633.30582896_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313341,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202637.69045721_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313342,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202641.39031204_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313343,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202644.76393488_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313344,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202647.38157794_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313345,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202651.23366997_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313346,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202654.65632846_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313347,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202659.87220082_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313348,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202703.74518412_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313349,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202708.30410417_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313350,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202711.94424044_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313351,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202715.93670189_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7313352,
	      "image": "http://img5.mtime.cn/pi/2016/12/14/202720.18250387_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7317307,
	      "image": "http://img5.mtime.cn/pi/2016/12/25/152911.45158467_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7317308,
	      "image": "http://img5.mtime.cn/pi/2016/12/25/152954.91054710_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7317309,
	      "image": "http://img5.mtime.cn/pi/2016/12/25/153054.60942834_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7317310,
	      "image": "http://img5.mtime.cn/pi/2016/12/25/153112.46436308_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7317311,
	      "image": "http://img5.mtime.cn/pi/2016/12/25/153129.44103504_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7319758,
	      "image": "http://img5.mtime.cn/pi/2017/01/03/143151.12943816_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7319759,
	      "image": "http://img5.mtime.cn/pi/2017/01/03/143154.56254231_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7319760,
	      "image": "http://img5.mtime.cn/pi/2017/01/03/143158.91706419_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7319761,
	      "image": "http://img5.mtime.cn/pi/2017/01/03/143202.57687852_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7319762,
	      "image": "http://img5.mtime.cn/pi/2017/01/03/143207.14268299_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7319763,
	      "image": "http://img5.mtime.cn/pi/2017/01/03/143210.66233834_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7319764,
	      "image": "http://img5.mtime.cn/pi/2017/01/03/143213.70455693_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7319765,
	      "image": "http://img5.mtime.cn/pi/2017/01/03/143216.82153420_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7323613,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/113015.19889817_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7323614,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/113024.42342672_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7323615,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/113033.12351799_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7323616,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/113043.60433630_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7323617,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/113051.43500164_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7323618,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/113103.27723095_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7323619,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/113117.64371573_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7323620,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/113124.81430558_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7323621,
	      "image": "http://img5.mtime.cn/pi/2017/01/12/113131.12368570_1000X1000.jpg",
	      "type": 6
	    },
	    {
	      "id": 7052570,
	      "image": "http://img31.mtime.cn/pi/2015/05/19/090434.37804212_1000X1000.jpg",
	      "type": 31
	    },
	    {
	      "id": 7052571,
	      "image": "http://img31.mtime.cn/pi/2015/05/19/090453.32261291_1000X1000.jpg",
	      "type": 31
	    },
	    {
	      "id": 7241722,
	      "image": "http://img31.mtime.cn/pi/2016/06/12/092440.51513094_1000X1000.jpg",
	      "type": 31
	    },
	    {
	      "id": 7241721,
	      "image": "http://img31.mtime.cn/pi/2016/06/12/092440.91370777_1000X1000.jpg",
	      "type": 31
	    },
	    {
	      "id": 7241720,
	      "image": "http://img31.mtime.cn/pi/2016/06/12/092440.96437634_1000X1000.jpg",
	      "type": 31
	    },
	    {
	      "id": 7241719,
	      "image": "http://img31.mtime.cn/pi/2016/06/12/092439.16195808_1000X1000.jpg",
	      "type": 31
	    },
	    {
	      "id": 7241718,
	      "image": "http://img31.mtime.cn/pi/2016/06/12/092439.81902909_1000X1000.jpg",
	      "type": 31
	    },
	    {
	      "id": 7241717,
	      "image": "http://img31.mtime.cn/pi/2016/06/12/092438.54175552_1000X1000.jpg",
	      "type": 31
	    },
	    {
	      "id": 7241716,
	      "image": "http://img31.mtime.cn/pi/2016/06/12/092438.89530314_1000X1000.jpg",
	      "type": 31
	    },
	    {
	      "id": 7315530,
	      "image": "http://img5.mtime.cn/pi/2016/12/21/112620.53471128_1000X1000.jpg",
	      "type": 41
	    },
	    {
	      "id": 7315531,
	      "image": "http://img5.mtime.cn/pi/2016/12/21/112626.40033778_1000X1000.jpg",
	      "type": 41
	    },
	    {
	      "id": 7315532,
	      "image": "http://img5.mtime.cn/pi/2016/12/21/112633.57756841_1000X1000.jpg",
	      "type": 41
	    },
	    {
	      "id": 7315533,
	      "image": "http://img5.mtime.cn/pi/2016/12/21/112640.64664028_1000X1000.jpg",
	      "type": 41
	    },
	    {
	      "id": 7315534,
	      "image": "http://img5.mtime.cn/pi/2016/12/21/112647.90329276_1000X1000.jpg",
	      "type": 41
	    },
	    {
	      "id": 7315535,
	      "image": "http://img5.mtime.cn/pi/2016/12/21/112654.24739724_1000X1000.jpg",
	      "type": 41
	    },
	    {
	      "id": 7315536,
	      "image": "http://img5.mtime.cn/pi/2016/12/21/112702.53654087_1000X1000.jpg",
	      "type": 41
	    }
	  ],
	  "imageTypes": [
	    {
	      "type": -1,
	      "typeName": "显示所有"
	    },
	    {
	      "type": 6,
	      "typeName": "剧照"
	    },
	    {
	      "type": 1,
	      "typeName": "海报"
	    },
	    {
	      "type": 41,
	      "typeName": "工作照"
	    },
	    {
	      "type": 31,
	      "typeName": "新闻图片"
	    }
	  ]
	}

解析：

- `images`：图片内容
- `id`：图片 id
- `image`：图片链接
- `type`：图片类型码
- `imageTypes`：图片类型内容
- `typeName`：图片类型码对应的图片所属类型