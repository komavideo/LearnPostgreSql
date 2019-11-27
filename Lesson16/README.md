使用事务
==========

数据库事务(Database Transaction) ，是指作为单个逻辑工作单元执行的一系列操作，要么完全地执行，要么完全地不执行。 事务处理可以确保除非事务性单元内的所有操作都成功完成，否则不会永久更新面向数据的资源。通过将一组相关操作组合为一个要么全部成功要么全部失败的单元，可以简化错误恢复并使应用程序更加可靠。一个逻辑工作单元要成为事务，必须满足所谓的ACID（原子性、一致性、隔离性和持久性）属性。事务是数据库运行中的逻辑工作单位，由DBMS中的事务管理子系统负责事务的处理。

## 知识点

* PostgreSql数据库事务使用
  + begin
  + commit
  + rollback

## 实战演习

~~~sql
> select * from users;
> begin;
> update users set score = 50 where player = '库里';
> update users set score = 60 where player = '哈登';
> commit;
> select * from users;
> begin;
> update users set score = 0 where player = '库里';
> update users set score = 0 where player = '哈登';
> rollback;
> select * from users;
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
