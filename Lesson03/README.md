操作数据表
=========

## 知识点

* create table
* drop table
* psql使用

## 实战演习

~~~bash
$ sudo su postgres
$ createdb komablog
$ psql -l
$ psql komablog
> create table posts (title varchar(255), content text);
> \dt
> \d posts
> alter table posts rename to komaposts;
> \dt
> drop table komaposts;
> \dt
> \q
$ nano db.sql
...
create table posts (title varchar(255), content text);
...
$ psql komablog
> \i db.sql
> \dt
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
