添加表约束
=========

## 知识点

* 表子段的约束条件

## 实战演习

### db.sql

~~~sql
create table posts (
    id serial primary key,
    title varchar(255) not null,
    content text check(length(content) > 8),
    is_draft boolean default TRUE,
    is_del boolean default FALSE,
    created_date timestamp default 'now'
);

-- 说明
/*
约束条件：

not null:不能为空
unique:在所有数据中值必须唯一
check:字段设置条件
default:字段默认值
primary key(not null, unique):主键，不能为空，且不能重复
*/
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
