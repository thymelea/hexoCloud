---
title: 处理并发和同步
---

## 如何处理并发和同步：
### 1. 在程序中使用线程的锁机制完成并发控制，
### 2. 在利用数据库的锁机制，如：悲观锁和乐观锁
#### 悲观锁 ：就是在查询语句后面加上for update，查询时锁住表的字段不可更新操作，直到事务提交，才会释放锁，缺点：对于大量数据操作时，
	 资源浪费严重
#### 乐观锁：在表结构基础上添加一个版本冗余字段，没对数据库中数据操作一次该字段进行一次加1，只有比当前版本大的数据才可入库，对于大量数据
	的操作一般都是用乐观锁。
## 对于大量数据处理：
### 分表存储，如通过时间分，或者某些字段分
## 对于大量并发请：1.提高访问带宽，2.搭建负载均衡服务器，3.oracle分表机制，进行分表，4.不持续操作数据库，使用缓存技术，5，使用静态页面





More info: [更多](https://www.cnblogs.com/lr393993507/p/5909804.html)