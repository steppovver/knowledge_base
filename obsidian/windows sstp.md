1. Open the Settings, click on "Network & Internet" and then click on "VPN".
2. Click on "Add VPN".
3. ![[Pasted image 20250203094150.png]]
4. Press the Windows key and letter R. Type `ncpa.cpl` and press "OK".
5. Open properties of recently created VPN.
6. ![[Pasted image 20250203094629.png]]
7. ![[Pasted image 20250203094803.png]]
8. На данном этапе уже все должно работать как через exe установщик
9. Далее переходим к настройке маршрутов
10. 
11. Отключаем Default Gateway![[Pasted image 20250203094946.png]]
12. Далее в `PowerShell` вводим
```
Add-VpnConnectionRoute -ConnectionName "STC VPN" -DestinationPrefix 192.168.222.0/23 –PassThru
Add-VpnConnectionRoute -ConnectionName "STC VPN" -DestinationPrefix 172.16.0.0/15 –PassThru
Add-VpnConnectionRoute -ConnectionName "STC VPN" -DestinationPrefix 172.22.0.0/16 –PassThru
Add-VpnConnectionRoute -ConnectionName "STC VPN" -DestinationPrefix 172.26.34.0/23 –PassThru
```
13. Вуаля. Теперь работает и интернет и стцшные штучки дрючки

