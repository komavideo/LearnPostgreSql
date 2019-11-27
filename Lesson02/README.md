初来乍到数据库
=============

## 知识点

* psql的基础
* 数据库简单操作
* 写个SQL

## 实战演习

~~~bash
$ sudo su postgres
$ psql --version
$ psql -l
$ createdb komablog
$ psql -l
$ psql komablog
> help
> \h
> \?
> \l
> \q
$ psql komablog
> select now();
> select version();
> \q
$ dropdb komablog
$ psql -l
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
