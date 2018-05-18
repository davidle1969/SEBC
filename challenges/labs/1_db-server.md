[root@ip-172-31-10-51 ~]# hostname -f
ip-172-31-10-51.ap-southeast-1.compute.internal


[root@ip-172-31-10-51 ~]#  mysql -u hive -p -h `hostname -f` -e "status;"
Enter password:
--------------
mysql  Ver 15.1 Distrib 5.5.56-MariaDB, for Linux (x86_64) using readline 5.1

Connection id:          585
Current database:
Current user:           hive@ip-172-31-10-51.ap-southeast-1.compute.internal
SSL:                    Not in use
Current pager:          stdout
Using outfile:          ''
Using delimiter:        ;
Server:                 MariaDB
Server version:         5.5.56-MariaDB MariaDB Server
Protocol version:       10
Connection:             ip-172-31-10-51.ap-southeast-1.compute.internal via TCP/IP
Server characterset:    latin1
Db     characterset:    latin1
Client characterset:    utf8
Conn.  characterset:    utf8
TCP port:               3306
Uptime:                 2 hours 32 min 51 sec

Threads: 31  Questions: 196315  Slow queries: 0  Opens: 1512  Flush tables: 2  Open tables: 246  Queries per second avg: 21.406
--------------

[root@ip-172-31-10-51 ~]#  mysql -u hive -p -h `hostname -f` -e "show databases;"
Enter password:
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive_metastore     |
| test               |
+--------------------+

