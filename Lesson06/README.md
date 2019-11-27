INSERT语句
==========

## 知识点

* insert into [tablename] (field, ...) values (value, ...)

## 实战演习

~~~sql
$ psql komablog
> \dt
> \d posts
~~~

### SQL部分

~~~sql
> insert into posts (title, content) values ('', '');
> insert into posts (title, content) values (NULL, '');
> insert into posts (title, content) values ('title1', 'content11');
> select * from posts;
> insert into posts (title, content) values ('title2', 'content22');
> insert into posts (title, content) values ('title3', 'content33');
> select * from posts;
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
