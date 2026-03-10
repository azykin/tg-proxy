# tg-proxy

Установка
`bash <(curl -s "https://raw.githubusercontent.com/nolaxe/install-MTProxy/main/telemt-from-image.sh")`

Остановить все контейнеры
`docker stop $(docker ps -q)`

Очистка docker
`docker system prune -a --volumes`

Проверка открытых портов
`sudo ufw status verbose`

Добавление портов и включение фаервола
`sudo ufw allow 22/tcp
sudo ufw allow 443/tcp
sudo ufw allow 8443/tcp
sudo ufw enable   # если ещё не включён
`

Показать все занятые порты
`ss -tulpn`

Создание HEX секрета
`openssl rand -hex 16`
