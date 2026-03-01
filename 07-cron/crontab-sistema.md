# Crontab del sistema (/etc/crontab)

## Ubicación
/etc/crontab

## Diferencia con crontab de usuario
Incluye un campo adicional para el usuario que ejecuta el comando.

## Formato
MIN HORA DIA-MES MES DIA-SEMANA USUARIO comando

## Ejemplo
# Ejecutar como root todos los días a las 2 AM
0 2 * * * root /usr/local/bin/script.sh
