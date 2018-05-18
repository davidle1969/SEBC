AWS
ec2-13-250-106-119.ap-southeast-1.compute.amazonaws.com
ec2-54-251-181-71.ap-southeast-1.compute.amazonaws.com
ec2-52-221-198-84.ap-southeast-1.compute.amazonaws.com
ec2-13-229-201-255.ap-southeast-1.compute.amazonaws.com
ec2-54-169-148-224.ap-southeast-1.compute.amazonaws.com

Red Hat 7.0

[centos@ip-172-31-10-51 ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       50G  894M   50G   2% /
devtmpfs        7.8G     0  7.8G   0% /dev
tmpfs           7.8G     0  7.8G   0% /dev/shm
tmpfs           7.8G   17M  7.8G   1% /run
tmpfs           7.8G     0  7.8G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000

[root@ip-172-31-10-51 ~]#  yum repolist enable
Loaded plugins: fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirror.qoxy.com
 * extras: mirror.qoxy.com
 * updates: mirror.qoxy.com
repolist: 0
[root@ip-172-31-10-51 ~]#


[root@ip-172-31-10-51 ~]# id jimenez
uid=2800(jimenez) gid=2800(jimenez) groups=2800(jimenez),2902(rangers)
[root@ip-172-31-10-51 ~]# id beltran
uid=2900(beltran) gid=2900(beltran) groups=2900(beltran),2901(astros)
[root@ip-172-31-10-51 ~]# grep jimenez /etc/passwd
jimenez:x:2800:2800::/home/jimenez:/bin/bash
[root@ip-172-31-10-51 ~]# grep beltran /etc/passwd
beltran:x:2900:2900::/home/beltran:/bin/bash
[root@ip-172-31-10-51 ~]# grep jimenez /etc/group
jimenez:x:2800:
rangers:x:2902:jimenez
[root@ip-172-31-10-51 ~]# grep beltran /etc/group
beltran:x:2900:
astros:x:2901:beltran



