# otus-systemd

Не смог понять, почему  timer принципиально отказывался запускать service. То есть перезапускать раз в 30 секунд - timer перезапускает, но вот без отдельного старта watchlog.service - ничего не работает. 

systemctl start watchlog.timer

systemctl start watchlog.service

Все проверки - по методичке, т.е.:

1) tail -f /var/log/messages

2) systemctl status spawn-fcgi

3) ss -tnulp | grep httpd



