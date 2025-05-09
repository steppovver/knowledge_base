https://askubuntu.com/questions/57339/connect-disconnect-from-vpn-from-the-command-line


sudo nmcli connection up id STC-SSTP


```
nmcli connection modify stc-vpn-sstp +vpn.data "connection-type = password"
```

https://gitlab.gnome.org/GNOME/network-manager-sstp/-/issues/50