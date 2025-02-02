
isstp
usepeerdns require-mschap-v2 noauth noipdefault noccp refuse-eap refuse-pap refuse-mschap nodefaultroute

au.stc-spb.ru
rubensp
sstpc
4kQsH4fH


скрипт для запуска **sstp-client**
```
#!/bin/bash
sudo /opt/homebrew/Cellar/sstp-client/1.0.20/sbin/sstpc --log-level 4 --log-stdout --log-stderr --user rubensp --password <password> --cert-warn au.stc-spb.ru usepeerdns require-mschap-v2 noauth noipdefault refuse-eap refuse-pap refuse-mschap nodefaultroute
```

```
~ ❯ cat /etc/ppp/ip-up 
```

```
#!/bin/sh
now=`date +%Y-%m-%d_%Hh%Mm%Ss`
logfile=/var/log/ip-up.log

echo "$0 called at $now with following params:" >> $logfile
echo "The VPN interface (e.g. ppp0): $1" >> $logfile
echo "Unknown, was 0, in my case: $2" >> $logfile
echo "IP of the VPN server: $3" >> $logfile
echo "VPN gateway address: $4" >> $logfile
echo "Regular (non-vpn) gateway for your lan connections: $5" >> $logfile

# Add 192.168.0.0 to 192.168.0.255 range to routing table on VPN interface
# /sbin/route add -net 192.168.0.0/16 -interface $1 >> $logfile 2>&1

/sbin/route add 192.168.222.0/23 -interface $1 >> $logfile 2>&1
/sbin/route add 172.16.0.0/15 -interface $1 >> $logfile 2>&1
/sbin/route add 172.22.0.0/16 -interface $1 >> $logfile 2>&1
```

# Don't forget add chmod +x
```
sudo chmod +x /etc/ppp/ip-up
```


[[macos setup]]