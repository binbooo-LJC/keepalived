# keepalived
keepalived 高可用lvs负载均衡集群
########
  keepalived.conf
###
1.keepalived.config 为DR1（前端主调度器）配置，将该keepalived.conf分别放置在DR1和DR2/etc/keepalived目录下。
2.修改DR2服务器下keepalived.conf文件。statue MASTER =>statue BACKUP,proirity 100=>prority 80(低于100即可)
#####

##### 
  realServer.sh
####
 分别将realServer.sh 放置RS1和RS2，sh realServer.sh start
### 


