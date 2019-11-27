变更表结构
==========

## 知识点

* alter table [tablename] ...
* create index ...
* drop index ...

## 实战演习

~~~sql
> \d users;
> alter table users add fullname varchar(255);
> \d users;
> alter table users drop fullname;
> \d users;
> alter table users rename player to nba_player;
> \d users;
> alter table users alter nba_player type varchar(100);
> \d users;
> create index nba_player_index on users(nba_player);
> \d users;
> drop index nba_player_index;
> \d users;
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
