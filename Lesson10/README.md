统计抽出数据
===========

## 知识点

* distinct
* sum
* max/min
* group by/having

## 实战演习

~~~sql
> select distinct team from users;
> select sum(score) from users;
> select max(score) from users;
> select min(score) from users;
> select * from users where score = (select max(score) from users);
> select * from users where score = (select min(score) from users);
> select team, max(score) from users group by team;
> select team, max(score) from users group by team having max(score) >= 25;
> select team, max(score) from users group by team having max(score) >= 25 order by max(score);
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
