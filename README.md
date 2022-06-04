# DoubanMovieJSON

## 简介
**所有数据均来自互联网，仅供学习使用！**

用于存放豆瓣电影数据，可当做API使用。数据并不完整，已收录列表见：

https://douban.8610000.xyz/movies.html

## 使用说明
#### 特定电影详情
- `https://douban.8610000.xyz/data/<豆瓣电影ID>.json`
 
包含特定电影的完整信息 (如https://douban.8610000.xyz/data/35235502.json)

#### 所有电影的基本信息
- `https://douban.8610000.xyz/q.json`

包含标题、年份等，用于客户端缓存后检索查询用于客户端缓存后检索查询电影ID

#### 标题筛选电影
- `https://douban.8610000.xyz/suggest/<标题>.json`

获取使用此标题的电影列表（**须将`/ \ : * ? " < > |`替换成`_`**） (如https://douban.8610000.xyz/suggest/芬奇.json)


#### 热门影视
- 豆瓣热门：`https://douban.8610000.xyz/hot/<日期>/movie_hot_gaia.json`
- 影院热映：`https://douban.8610000.xyz/hot/<日期>/movie_showing.json`
- 热播剧集：`https://douban.8610000.xyz/hot/<日期>/tv_hot.json`
- 热门综艺：`https://douban.8610000.xyz/hot/<日期>/tv_variety_show.json`

当天七点前更新 (如https://douban.8610000.xyz/hot/20220604/movie_hot_gaia.json)

#### 加入抓取队列
- `https://douban.8610000.xyz/api/v1/queue/movie/<豆瓣电影ID>`

10W次请求/日，定时提交，有延迟 (如https://douban.8610000.xyz/api/v1/queue/movie/26882248)

## 协助完善
**在浏览豆瓣电影页面时自动提交抓取。**
- 安装脚本：https://greasyfork.org/zh-CN/scripts/427606-doubanmoviejson


## 更新
#### 2022.06.04
- 新增热门影视查询
