---
title: MySQL 为日期增加一个时间间隔
---


``` bash
set @dt = now();  
select date_add(@dt, interval 1 day);   - 加1天  
select date_add(@dt, interval 1 hour);   -加1小时  
select date_add(@dt, interval 1 minute);    - 加1分钟  
select date_add(@dt, interval 1 second); -加1秒  
select date_add(@dt, interval 1 microsecond);-加1毫秒  
select date_add(@dt, interval 1 week);-加1周  
select date_add(@dt, interval 1 month);-加1月  
select date_add(@dt, interval 1 quarter);-加1季  
select date_add(@dt, interval 1 year);-加1年 
```

More info: [更多](https://blog.csdn.net/mr_linjw/article/details/49849691)