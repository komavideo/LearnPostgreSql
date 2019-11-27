数据抽出选项
===========

## 知识点

select语句在抽出数据时，可以对语句设置更多的选项，已得到想要的数据。

* order by
* limit
* offset

## 实战演习

~~~sql
> select * from users order by score asc;
> select * from users order by score desc;
> select * from users order by team;
> select * from users order by team, score;
> select * from users order by team, score desc;
> select * from users order by team desc, score desc;
> select * from users order by score desc limit 3;
> select * from users order by score desc limit 3 offset 1;
> select * from users order by score desc limit 3 offset 2;
> select * from users order by score desc limit 3 offset 3;
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
