SELECT语句
==========

## 知识点

* select 基本使用

## 实战演习

### init.sql

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
~~~

### SQL实战

~~~bash
$ psql komablog
> \i init.sql
> \dt
> \d users
> select * from users;
> \x
> select * from users;
> \x
> select * from users;
> select player, score from users;
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
