# mail
Скрипт автоматической настройки почтового сервера на Debian 10 Buster

Использование:
1. Запустите mailserver-setup.sh, укажите короткое имя хоста почтового сервера Specity, имя домена и локальный IP-адрес. Когда скрипт завершит работу, скопируйте пароль postgres и замените его строкой PASSWORD в mailuser-addnew.sh и mailuser-setpass.sh.
2. Заменить master.cf в / etc / postfix
3. Сгенерируйте SSL и DKIM, добавьте запись DKIM в /etc/rspamd/dkim_selectors.map.
4. Перезагрузите сервер.
5. Используйте mailuser-addnew.sh для создания нового почтового пользователя, используя mailuser-setpass.sh для изменения паролей для существующих пользователей. 
