# SSH Hardening

## Archivo de configuración
/etc/ssh/sshd_config

## Deshabilitar login de root
PermitRootLogin no

## Cambiar puerto SSH
Port 2222

## Deshabilitar autenticación por contraseña
PasswordAuthentication no

## Reiniciar servicio SSH
sudo systemctl restart ssh

## Ver estado
sudo systemctl status ssh
