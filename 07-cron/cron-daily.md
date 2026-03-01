# Cron.daily y tareas periódicas del sistema

## Ubicación
/etc/cron.daily/
/etc/cron.hourly/
/etc/cron.weekly/
/etc/cron.monthly/

## Funcionamiento
Los scripts dentro de estas carpetas se ejecutan automáticamente según su frecuencia.

## Permisos requeridos
Los scripts deben ser ejecutables:
chmod +x /etc/cron.daily/mi-script

## Ver logs de ejecución
cat /var/log/syslog | grep cron
