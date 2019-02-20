# VMSetup
VM Setup

vpn_centos.sh

因为centos7下默认实用的是firewall作为防火墙，但是脚本中还是使用iptables，所以在脚本设置pptpd开机启动之后应该顺便设置iptables开机启动，不然重启服务器之后iptables不生效。chkconfig iptables on

sudo vi /etc/ppp/chap-secrets

