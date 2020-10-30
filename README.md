For CentOS：
yum install -y wget curl cronie

For Debian 8+：
apt install -y wget curl cron

For Ubuntu/Debian 7：
apt-get install -y wget curl cron
然后下载AliDDNS脚本到你的服务器上：

wget -O /usr/sbin/AliDDNS-v2.0.sh https://ilemonrain.com/download/shell/AliDDNSv2.sh
下载地址请参考上面的 更新记录 & 下载地址 一节！
为脚本文件加上可执行属性：

chmod +x /usr/sbin/AliDDNS-v2.0.sh
执行脚本，开始配置：

/usr/sbin/AliDDNS-v2.0.sh
