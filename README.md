For CentOS：
yum install -y wget curl cronie

For Debian 8+：
apt install -y wget curl cron

For Ubuntu/Debian 7：
apt-get install -y wget curl cron
然后下载AliDDNS脚本到你的服务器上：

wget -O /usr/sbin/AliDDNS-v2.0.sh https://raw.githubusercontent.com/sigle0724/aliddnsv2/main/AliDDNSv2.sh && chmod +x /usr/sbin/AliDDNS-v2.0.sh && /usr/sbin/AliDDNS-v2.0.sh

计划任务

*/1 * * * * /usr/sbin/AliDDNS-v2.0.sh run >/dev/null 2>&1 &

重启

CentOS:

service crond restart

Ubuntu/Debian：

service cron restart

并将Cron加入开机启动项：

CentOS：

chkconfig crond on

Ubuntu/Debian：

systemctl enable cron
