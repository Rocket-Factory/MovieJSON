# DoubanMovieJSON

## 简介
用于存放豆瓣电影数据，可当做API使用。
完整收录列表：https://douban.8610000.xyz/movies.html

## 使用说明
1. `https://douban.8610000.xyz/data/<豆瓣SubjectID>.json`查看特定电影详情。
2. `https://douban.8610000.xyz/q.json`查看所有电影的基本信息(标题、年份等)，用于客户端缓存后检索查询SubjectID。
3. 每日更新，会有未收录的情况，可通过`https://alagorn.8610000.xyz/api/v1/queue/movie/<豆瓣SubjectID>`加入抓取队列。
