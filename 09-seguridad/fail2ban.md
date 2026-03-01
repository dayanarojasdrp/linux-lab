# Fail2ban

## Instalar Fail2ban
sudo apt install fail2ban

## Archivo principal de configuración
/etc/fail2ban/jail.conf

## Archivo recomendado para personalizar
/etc/fail2ban/jail.local

## Servicio
sudo systemctl start fail2ban
sudo systemctl enable fail2ban
sudo systemctl status fail2ban

## Ver jails activos
sudo fail2ban-client status

## Ver IPs bloqueadas en sshd
sudo fail2ban-client status sshd
