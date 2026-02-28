# Crear Servicios con systemd 

## Objetivo
Aprender a crear, habilitar, iniciar y depurar servicios personalizados usando systemd, como lo haría un administrador Junior+ en un servidor Linux.

---

## ¿Qué es un servicio systemd?
Un servicio es un proceso gestionado por systemd que puede iniciarse automáticamente al arrancar el sistema, reiniciarse si falla y generar logs propios.

Los servicios se definen en archivos `.service` ubicados en: /etc/systemd/system/

---

## Estructura de un archivo .service

Ejemplo típico:
[Unit]
Description=Mi servicio personalizado
After=network.target

[Service]
ExecStart=/usr/local/bin/mi_script.sh
Restart=on-failure
User=dayana

[Install]
WantedBy=multi-user.target

### Explicación
- **[Unit]**
  - `Description`: descripción del servicio.
  - `After`: indica que debe iniciarse después de la red.

- **[Service]**
  - `ExecStart`: comando principal del servicio.
  - `Restart`: reinicio automático si falla.
  - `User`: usuario con el que corre el servicio.

- **[Install]**
  - `WantedBy`: define en qué modo del sistema se habilita.

---

## Crear un servicio paso a paso

### 1. Crear el archivo del servicio
```bash
sudo nano /etc/systemd/system/mi_servicio.service

