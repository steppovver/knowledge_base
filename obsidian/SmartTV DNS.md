https://dtf.ru/howto/3042960-obhod-zamedleniya-youtube-dlya-lyubyh-smart-tv-s-goodbyedpi-v2ray-maradns

Перенаправление всего трафика на прокси-сервер, запущенный на компьютере, путём ответов DNS на любой домен IP-адресом компьютера.Примитивный и не особо удобный, но простой и практически универсальный метод, подходящий для любых телевизоров, даже базовых и устаревших моделей. Работает только при включённом компьютере.

в своем [тг-канале](https://ttttt.me/+a77e9ybQ4bRhZTNi) я собрал самые актуальные способы обхода блокировки, можете выбрать любой способ, который вам больше всего подходит: Для Smart TV, ПК, телефона, Android, IOS и т.д.
![[Pasted image 20241003203752.png]]
## На компьютере с Windows:

- [Скачайте, настройте и запустите GoodbyeDPI 690](https://github.com/ValdikSS/GoodbyeDPI/releases/tag/0.2.3rc3), убедитесь, что он работает на компьютере
- Скачайте архив [v2ray-maradns.7z](https://ntc.party/uploads/short-url/gJuqsY5xacVbRKEQTd9ZHcGVcM5.7z) (7.8 MB), распакуйте
- Откройте файл maradns\zone-redirect-all.txt блокнотом, замените 192.168.69.128 на IP-адрес вашего компьютера (его можно посмотреть в настройках сетевого адаптера, либо командой ipconfig)
- Запуститеv2ray\v2ray-run.cmd, в появившемся окне разрешите сетевое взаимодействие программы, сверните окно
- Запустите maradns\mara-run.cmd, в появившемся окне разрешите сетевое взаимодействие программы, сверните окно

## На телевизоре:

- Найдите в настройках сети настройки DNS-сервера
- Укажите IP-адрес вашего компьютера (который вы вписали в maradns\zone-redirect-all.txt) в качестве DNS-сервера (и основного, и альтернативного, если телевизор требует два адреса).Некоторые модели не позволяют указать только DNS-сервер внучную: может потребоваться также задать настройки IP-адреса, маски подсети и шлюза
- Отключите IPv6, если такая возможность есть в телевизоре. Это следует сделать, даже если у вас нет IPv6-связности (роутер может выдавать DNS по IPv6 внутри локальной сети)
- Откройте браузер, убедитесь, что сайты открываются
- Откройте YouTube

Переходите в мой [тг-канал](https://ttttt.me/+a77e9ybQ4bRhZTNi), где я регулярно выкладываю полезные сервисы и приложения для жизни

[[VPN]]
