操作多个表
==========

## 知识点

* 表结合查询的基础知识

## 实战演习

### renew.sql

~~~sql
create table users (
    id serial primary key,
    player varchar(255) not null,
    score real,
    team varchar(255)
);
insert into users (player, score, team) values
('库里', 28.3, '勇士'),
('哈登', 30.2, '火箭'),
('阿杜', 25.6, '勇士'),
('阿詹', 27.8, '骑士'),
('神龟', 31.3, '雷霆'),
('白边', 19.8, '热火');

create table twitters (
    id serial primary key,
    user_id integer,
    content varchar(255) not null
);
insert into twitters (user_id, content) values
(1, '今天又是大胜,克莱打的真好!'),
(2, '今晚我得了60分,哈哈!'),
(3, '获胜咱不怕,缺谁谁尴尬.'),
(4, '明年我也可能转会西部'),
(5, '我都双20+了，怎么球队就是不胜呢?'),
(1, '明年听说有条大鱼要来,谁呀?');
~~~

### SQL实行

~~~sql
$ dropdb komablog;
$ createdb komablog;
$ psql komablog;
> \i renew.sql
> select * from users;
> select * from twitters;
> select users.player, twitters.content from users, twitters where users.id = twitters.user_id;
> select u.player, t.content from users as u, twitters as t where u.id = t.user_id;
> select u.player, t.content from users as u, twitters as t where u.id = t.user_id and u.id = 1;
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
