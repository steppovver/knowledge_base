Нашел для убунты нормальное приложение для удаленного рабочего стола

На рабочем компе ставим сервак sudo apt install freerdp2-shadow-x11

На домашнем компе ставим клиента sudo apt install freerdp2-x11

  

Запускается сервак командой. В автозапуск пока хз можно ли добавить встроенными средствами

freerdp-shadow-cli /port:<port> -auth

Порт можно не указывать, будет использовать дефолтный. Но у меня он с чем-то конфликтует 

  

чтоб подключиться с домашнего компа:

xfreerdp /u:<имя пользователя> /p:<пароль> /v:<ip:port> /bpp:16

bpp - количетсво бит используемых для передачи цвета. 16 минимум и вроде его достаточно.

```
xfreerdp /u:prubens /p:0113 /w:1280 /h:720 /v:172.26.34.27:25566 /video /rfx /network:lan /gfx /dynamic-resolution /sound:sys:pulse
```

xfreerdp /u:prubens /p:0113 /v:192.168.222.27:25565 /network:wan /video /rfx /gfx /smart-sizing:1280x720