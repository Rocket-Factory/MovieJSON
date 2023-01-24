# MovieJSON

## 简介
**所有数据均来自互联网，仅供学习使用！**

用于存放电影数据，可当做API使用。数据并不完整。

[https://moviefront.8610000.xyz](https://moviefront.8610000.xyz/)

## 使用说明

### 1.电影
#### 特定电影详情
- `https://moviedb.8610000.xyz/data/<电影ID>.json`
 
*(如: https://moviedb.8610000.xyz/data/35235502.json)*

#### 特定电影相关影视推荐
- `https://moviedb.8610000.xyz/recommendation/<电影ID>.json`

包含电影基础信息和推荐影视列表（前期抓取的电影不存在此项信息）

*(如: https://moviedb.8610000.xyz/recommendation/35256195.json)*

#### 所有电影的基本信息
- `https://moviedb.8610000.xyz/q.json`

包含标题、年份等，用于客户端缓存后检索查询用于客户端缓存后检索查询电影ID

#### 标题筛选
- `https://moviedb.8610000.xyz/suggest/<标题>.json`

获取使用此标题的电影列表（**须将`/ \ : * ? " < > |`替换成`_`**） 

*(如: https://moviedb.8610000.xyz/suggest/芬奇.json)*

---

### 2.影人
#### 特定影人详情
- `https://celebrity.8610000.xyz/data/<影人ID>.json`

包含影人的完整信息

*(如: https://celebrity.8610000.xyz/data/1313742.json)*


#### 名字筛选
- `https://celebrity.8610000.xyz/suggest/<名字>.json`

获取同名的影人列表

*(如: https://celebrity.8610000.xyz/suggest/大卫·叶茨.json)*

---

### 3.榜单
#### 热门影视(每日更新)
- 热门影视：`https://rank.8610000.xyz/hot/<日期>/movie_hot_gaia.json`
- 正在上映：`https://rank.8610000.xyz/hot/<日期>/movie_showing.json`
- 热播剧集：`https://rank.8610000.xyz/hot/<日期>/tv_hot.json`
- 热门综艺：`https://rank.8610000.xyz/hot/<日期>/tv_variety_show.json`

*(如: https://moviedb.8610000.xyz/hot/20220604/movie_hot_gaia.json)*

#### 一周口碑影视(每周更新)
- 电影: `https://rank.8610000.xyz/weekly_best/movie/1.json`
- 华语剧集: `https://rank.8610000.xyz/weekly_best/tv_chinese/1.json`
- 全球剧集: `https://rank.8610000.xyz/weekly_best/tv_global/1.json`

#### 分类经典电影
- 动作: `https://rank.8610000.xyz/category/action/1.json`
- 喜剧: `https://rank.8610000.xyz/category/comedy/1.json`
- 科幻: `https://rank.8610000.xyz/category/scifi/1.json`
- 爱情: `https://rank.8610000.xyz/category/love/1.json`

#### Top250
- `https://rank.8610000.xyz/top250/<页码>.json)`

通过`1.json`, `2.json`, `...`分页, 每页20项


## 更新
#### 2023.01.24
- 新增榜单数据 (Rocket-Factory/MovieRankJSON)
- 移除本项目内的热门影视数据(重定向)

#### 2023.01.23
- 新增影人数据 (Rocket-Factory/CelebrityJSON)

#### 2022.10.22
- 新增相关影视推荐

#### 2022.09.17
- 修改仓库名称
- 修改域名（只做了重定向，原域名可用）
- 移除抓取脚本和抓取队列API

#### 2022.06.04
- 新增热门影视查询
