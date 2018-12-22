# MysqlCodeTree
Mysql核心源码阅读

<pre>
Mysql调优

      1.由于应用对mysql的并发操作较大 
        show processlist;
  
       大概有1000多的并发sql，积压，现在先解决sql挤压的问题
       将mysql的线程数调大，这个配置和cpu个数一样大小
       set global innodb_thread_concurrency=32

       观察一段时间，发现挤压情况减少，仍然有部分sql执行过慢

      2：锁超时，事务回滚
</pre>