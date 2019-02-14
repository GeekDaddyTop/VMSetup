# VMSetup
VM Setup

使用 vpn_centos.sh，另一个一过期.

因为centos7下默认实用的是firewall作为防火墙，但是脚本中还是使用iptables，所以在脚本设置pptpd开机启动之后应该顺便设置iptables开机启动，不然重启服务器之后iptables不生效。chkconfig iptables on

添加新用户：
sudo vi /etc/ppp/chap-secrets

