更新和删除
==========

## 知识点

* update [table] set [field=newvalue,...] where ...
* delete from [table] where ...

## 实战演习

~~~sql
> update users set score = 29.1 where player = '阿詹';
> update users set score = score + 1 where team = '勇士';
> update users set score = score + 100 where team IN ('勇士', '骑士');
> delete from users where score > 30;
~~~

## 课程文件

https://gitee.com/komavideo/LearnPostgreSql

## 小马视频频道

http://komavideo.com
