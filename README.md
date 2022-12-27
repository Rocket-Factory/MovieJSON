# MovieJSON

## 简介
**所有数据均来自互联网，仅供学习使用！**

用于存放电影数据，可当做API使用。数据并不完整。

https://moviefront.8610000.xyz

## 使用说明
#### 特定电影详情
- `https://moviedb.8610000.xyz/data/<电影ID>.json`
 
包含特定电影的完整信息 (如https://moviedb.8610000.xyz/data/35235502.json)

#### 特定电影相关影视推荐
- `https://moviedb.8610000.xyz/recommendation/<电影ID>.json`

包含电影基础信息和推荐影视列表（前期抓取的电影不存在此项信息） (如https://moviedb.8610000.xyz/recommendation/35256195.json)

#### 所有电影的基本信息
- `https://moviedb.8610000.xyz/q.json`

包含标题、年份等，用于客户端缓存后检索查询用于客户端缓存后检索查询电影ID

#### 标题筛选电影
- `https://moviedb.8610000.xyz/suggest/<标题>.json`

获取使用此标题的电影列表（**须将`/ \ : * ? " < > |`替换成`_`**） (如https://moviedb.8610000.xyz/suggest/芬奇.json)


#### 热门影视
- 热门影视：`https://moviedb.8610000.xyz/hot/<日期>/movie_hot_gaia.json`
- 正在上映：`https://moviedb.8610000.xyz/hot/<日期>/movie_showing.json`
- 热播剧集：`https://moviedb.8610000.xyz/hot/<日期>/tv_hot.json`
- 热门综艺：`https://moviedb.8610000.xyz/hot/<日期>/tv_variety_show.json`

当天七点前更新 (如https://moviedb.8610000.xyz/hot/20220604/movie_hot_gaia.json)

## 更新

#### 2022.10.22
- 新增相关影视推荐

#### 2022.09.17
- 修改仓库名称
- 修改域名（只做了重定向，原域名可用）
- 移除抓取脚本和抓取队列API

#### 2022.06.04
- 新增热门影视查询
