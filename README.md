# DoubanMovieJSON

## 简介
用于存放豆瓣电影数据，可当做API使用。

数据并不完整，已收录列表见：https://douban.8610000.xyz/movies.html

## 使用说明
1. `https://douban.8610000.xyz/data/<豆瓣电影ID>.json`查看特定电影详情。
2. `https://douban.8610000.xyz/q.json`查看所有电影的基本信息(标题、年份等)，用于客户端缓存后检索查询SubjectID。
3. `https://alagorn.8610000.xyz/api/v1/queue/movie/<豆瓣电影ID>`加入抓取队列（定时提交到Github，最长有一天延迟才能使用）。

## 协助完善
**在浏览豆瓣电影页面时自动提交抓取。**
- 安装脚本：https://greasyfork.org/zh-CN/scripts/427606-doubanmoviejson
- 或在[Release](https://github.com/Rocket-Factory/DoubanMovieJSON/releases)中下载对应浏览器的辅助扩展。
