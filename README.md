# bad_ssh_ips
ssh attack package sent from thoses ips, drop them via iptables

## block via iptables in a simple loop
for ip in $(cat bad_ip_list.txt ); do iptables -I INPUT -s $ip -j DROP; done

## 恶意ssh地址 ip列表
