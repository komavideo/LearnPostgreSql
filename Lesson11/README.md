方便的函数
==========

## 知识点

* length
* concat
* alias
* substring
* random

参考网站：

https://www.postgresql.org/docs/9.5/static/functions.html

## 实战演习

~~~sql
> select player, length(player) from users;
> select player, concat(player, '/', team) from users;
> select player, concat(player, '/', team) as "球员信息" from users;
> select substring(team, 1, 1) as "球队首文字" from users;
> select concat('我', substring(team, 1, 1)) as "球队首文字" from users;
> select random();
> select * from users order by random();
> select * from users order by random() limit 1;
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
