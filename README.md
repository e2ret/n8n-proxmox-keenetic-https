n8n

Установка
bash -c "$(wget -qLO - https://github.com/tteck/Proxmox/raw/main/ct/n8n.sh)"

Ручная установка
Смена пароля root
Разрешить SSH

Создание домена в keenetic


Настройка Telegram
WEBHOOK_URL

/etc/systemd/system
Файл n8n.service

[Unit]
Description=n8n

[Service]
Type=simple
Environment="N8N_SECURE_COOKIE=false"
ExecStart=n8n start
Environment="WEBHOOK_URL=https://n8n.edhome.keenetic.pro/"
[Install]
WantedBy=multi-user.target
