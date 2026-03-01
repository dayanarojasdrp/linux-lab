# Logrotate

## Archivo principal
/etc/logrotate.conf

## Directorio de configuraciones por servicio
/etc/logrotate.d/

## Opciones comunes
- weekly: rotar semanalmente
- daily: rotar diariamente
- rotate N: mantener N archivos
- compress: comprimir logs viejos
- create: crear un nuevo log vacío
- missingok: no mostrar error si el log no existe
- notifempty: no rotar si está vacío

## Forzar rotación manual
sudo logrotate -f /etc/logrotate.conf
