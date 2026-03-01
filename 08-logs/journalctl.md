# Journalctl (logs de systemd)

## Ver logs de un servicio
journalctl -u nombre-del-servicio

## Últimas líneas
journalctl -u nombre-del-servicio -n 50

## Logs en tiempo real
journalctl -u nombre-del-servicio -f

## Logs desde el último arranque
journalctl -u nombre-del-servicio -b

## Filtrar por fecha
journalctl --since "2024-01-01" --until "2024-01-02"

## Ver todo el journal
journalctl
