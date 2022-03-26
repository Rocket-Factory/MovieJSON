# DoubanMovieJSON

## 简介
用于存放豆瓣电影数据，可当做API使用。

数据并不完整，已收录列表见：https://douban.8610000.xyz/movies.html

## 使用说明
1. `https://douban.8610000.xyz/data/<豆瓣电影ID>.json`查看特定电影详情。
(如https://douban.8610000.xyz/data/35235502.json)
3. `https://douban.8610000.xyz/q.json`查看所有电影的基本信息(标题、年份等)，用于客户端缓存后检索查询SubjectID。
5. `https://douban.8610000.xyz/api/v1/queue/movie/<豆瓣电影ID>`加入抓取队列（10W次请求/日，定时提交，有延迟）(如https://douban.8610000.xyz/api/v1/queue/movie/26882248)

## 协助完善
**在浏览豆瓣电影页面时自动提交抓取。**
- 安装脚本：https://greasyfork.org/zh-CN/scripts/427606-doubanmoviejson
