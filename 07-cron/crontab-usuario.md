# Crontab de usuario

## Editar crontab del usuario actual
crontab -e

## Ver tareas del usuario
crontab -l

## Eliminar crontab del usuario
crontab -r

## Sintaxis
MIN HORA DIA-MES MES DIA-SEMANA comando

## Ejemplos
# Cada minuto
* * * * * comando

# Todos los días a las 3 AM
0 3 * * * comando

# Cada 5 minutos
*/5 * * * * comando
