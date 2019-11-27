WHERE语句
==========

## 知识点

* where语句的使用

使用where语句来设定select,update,delete语句数据抽出的条件。

## 实战演习

~~~sql
> select * from users;
> select * from users where score > 20;
> select * from users where score < 30;
> select * from users where score > 20 and score < 30;
> select * from users where team = '勇士';
> select * from users where team != '勇士';
> select * from users where player like '阿%';
> select * from users where player like '阿_';
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
