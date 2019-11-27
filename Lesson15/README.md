使用视图
========

## 视图概念

视图（View）是从一个或多个表导出的对象。视图与表不同，视图是一个虚表，即视图所对应的数据不进行实际存储，数据库中只存储视图的定义，在对视图的数据进行操作时，系统根据视图的定义去操作与视图相关联的基本表。

## 小马解释

视图就是一个SELECT语句，把业务系统中常用的SELECT语句简化成一个类似于表的对象，便于简单读取和开发。

## 知识点

* 使用数据库视图(view)
  + create view ...
  + drop view ...

## 实战演习

~~~sql
> select u.player, t.content from users as u, twitters as t where u.id = t.user_id and u.id = 1;
> create view curry_twitters as select u.player, t.content from users as u, twitters as t where u.id = t.user_id and u.id = 1;
> \dv
> \d curry_twitters
> select * from curry_twitters;
> drop view curry_twitters;
> \dv
~~~

## 实战建议

在自己项目中，为了提高数据查询速度，可在表中加入索引index。同时对于经常需要查询的语句，可以提前建立视图view，方便于编码和管理。

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
