[root@ip-172-31-7-188 centos]# uptime
 04:06:10 up 32 min,  1 user,  load average: 0.00, 0.01, 0.05
 [root@ip-172-31-8-163 centos]# uptime
 04:06:20 up 32 min,  1 user,  load average: 0.00, 0.01, 0.01
[root@ip-172-31-15-157 centos]# uptime
 04:06:28 up 33 min,  1 user,  load average: 0.00, 0.01, 0.04
[root@ip-172-31-5-225 centos]# uptime
 04:06:24 up 32 min,  1 user,  load average: 0.00, 0.01, 0.01
[root@ip-172-31-15-61 centos]# uptime
 04:06:17 up 32 min,  1 user,  load average: 0.00, 0.01, 0.02

AWS

ec2-13-229-233-1.ap-southeast-1.compute.amazonaws.com
13.229.233.1

ec2-54-169-190-203.ap-southeast-1.compute.amazonaws.com
54.169.190.203

ec2-13-250-42-168.ap-southeast-1.compute.amazonaws.com
13.250.42.168

ec2-54-255-141-68.ap-southeast-1.compute.amazonaws.com
54.255.141.68

ec2-13-250-100-108.ap-southeast-1.compute.amazonaws.com
13.250.100.108

[root@ip-172-31-7-188 centos]# uname -a
Linux ip-172-31-7-188.ap-southeast-1.compute.internal 3.10.0-862.2.3.el7.x86_64 #1 SMP Wed May 9 18:05:47 UTC 2018 x86_64 x86_64 x86_64 GNU/Linux
[root@ip-172-31-7-188 centos]# cat /proc/version
Linux version 3.10.0-862.2.3.el7.x86_64 (builder@kbuilder.dev.centos.org) (gcc version 4.8.5 20150623 (Red Hat 4.8.5-28) (GCC) ) #1 SMP Wed May 9 18:05:47 UTC 2018

[root@ip-172-31-7-188 centos]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       50G  3.0G   47G   6% /
devtmpfs        7.8G     0  7.8G   0% /dev
tmpfs           7.8G     0  7.8G   0% /dev/shm
tmpfs           7.8G   17M  7.8G   1% /run
tmpfs           7.8G     0  7.8G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000
tmpfs           1.6G     0  1.6G   0% /run/user/0


[root@ip-172-31-7-188 centos]# yum repolist enabled
Loaded plugins: fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirror.qoxy.com
 * extras: mirror.qoxy.com
 * updates: mirror.qoxy.com
repo id                             repo name                             status
base/7/x86_64                       CentOS-7 - Base                       9,911
extras/7/x86_64                     CentOS-7 - Extras                       258
updates/7/x86_64                    CentOS-7 - Updates                      151
repolist: 10,320

[root@ip-172-31-7-188 centos]# cat /etc/passwd | grep hulk
hulk:x:2600:2600::/home/hulk:/bin/bash
[root@ip-172-31-7-188 centos]# cat /etc/passwd | grep thanos
thanos:x:2500:2500::/home/thanos:/bin/bash
[root@ip-172-31-7-188 centos]# cat /etc/passwd | grep groot
groot:x:2700:2700::/home/groot:/bin/bash


[root@ip-172-31-7-188 centos]# cat /etc/group | grep groot
groot:x:2700:
avengers:x:2702:hulk,groot
[root@ip-172-31-7-188 centos]# cat /etc/group | grep hulk
hulk:x:2600:
avengers:x:2702:hulk,groot
[root@ip-172-31-7-188 centos]# cat /etc/group | grep thanos
thanos:x:2500:
blackorder:x:2701:thanos




