# 1- 总览
```dataview
TABLE title AS 标题, file.mtime AS 修改时间
WHERE (
  contains(file.path, "概念") OR
  contains(file.path, "视频记录") OR
  contains(file.path, "DDD")

)
SORT file.mtime DESC
LIMIT 10
```
