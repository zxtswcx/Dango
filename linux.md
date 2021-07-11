````
## 查看防火墙状态

firewall-cmd --state

## 停止firewall

systemctl stop firewalld.service

service network restart

firewall-cmd --zone=public --add-port=8039/tcp --permanent
firewall-cmd --reload

````



