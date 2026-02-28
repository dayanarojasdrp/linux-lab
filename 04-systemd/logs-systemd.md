
# Logs en systemd con journalctl 

## Objetivo
Aprender a ver, filtrar y depurar logs de servicios administrados por systemd usando `journalctl`.

---

## Ver logs de un servicio

### Logs completos
```bash
journalctl -u mi_servicio
