# Подключение репозитория и установка nginx
```
sudo apt update
sudo apt install -y curl gnupg2 ca-certificates lsb-release ubuntu-keyring
curl https://nginx.org/keys/nginx_signing.key | gpg --dearmor | sudo tee /usr/share/keyrings/nginx-archive-keyring.gpg >/dev/null
echo "deb [signed-by=/usr/share/keyrings/nginx-archive-keyring.gpg] http://nginx.org/packages/ubuntu $(lsb_release -cs) nginx" | sudo tee /etc/apt/sources.list.d/nginx.list
sudo apt update
sudo apt install -y nginx
```
# Удаление nginx
``` sudo dpkg --purge nginx ```

# Установка пакета с использованием snap
``` sudo snap install htop ```

# Создание файла test.txt
```nano test.txt```

# Настройка автоматического бэкапа с использованием cron
```crontab -e```

# Добавил строку: */10 * * * * cp /home/nik/test.txt /home/nik/test.txt.bak