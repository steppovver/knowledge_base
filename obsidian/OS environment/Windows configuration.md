Основано но
[Диджитализируй](https://github.com/alexey-goloburdin/knowledge-base/blob/main/%D0%A1%D1%86%D0%B5%D0%BD%D0%B0%D1%80%D0%B8%D0%B9.%20%D0%9F%D0%BE%D0%BB%D0%BD%D0%B0%D1%8F%20%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0%20Windows%2C%20WSL%20%D0%B8%20%D0%B8%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D0%B2%20%D0%B4%D0%BB%D1%8F%20%D1%80%D0%B0%D0%B7%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%87%D0%B8%D0%BA%D0%B0.md#%D1%81%D0%BA%D1%80%D1%8B%D1%82%D1%8C-%D0%B8%D0%BA%D0%BE%D0%BD%D0%BA%D1%83-%D1%81-%D1%80%D0%B0%D0%B1%D0%BE%D1%87%D0%B5%D0%B3%D0%BE-%D1%81%D1%82%D0%BE%D0%BB%D0%B0)
# Скрыть иконку с рабочего стола

Надо в реестре в разделе `HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\HideDesktopIcons\NewStartPanel` добавить запись с именем `{2cc5ca98-6485-489a-920e-b3e88a6ccce3}` и значением `1`.
# WSL

Ставим WSL (команды выполняем в Powershell или командной строке Windows):
```bash
wsl --install -d Debian
wsl --set-default-version 2
```
# Настройка Git в WSL

```bash
sudo apt update
sudo apt install -y git

# чтобы кириллические имена файлов нормально выводились
git config --global core.quotepath
```


[[Windows]]