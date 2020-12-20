# otus-systemd

Не смог понять, почему  timer принципиально отказывался запускать service. То есть перезапускать раз в 30 секунд - timer перезапускает, но вот без отдельного старта watchlog.service - ничего не работает. 

systemctl start watchlog.timer

systemctl start watchlog.service

