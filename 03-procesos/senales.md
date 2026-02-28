# Señales en Linux 

## Objetivo
Comprender qué son las señales, cómo funcionan y cómo usarlas para controlar procesos en ejecución.

## Qué es una señal
Una señal es un mensaje que el kernel envía a un proceso para indicarle que debe hacer algo: terminar, pausar, continuar, recargar configuración, etc.

## Señales más importantes

### SIGTERM (15)
- Solicita terminar el proceso de forma **limpia**.
- El proceso puede atraparla y cerrar correctamente.
- Es la señal recomendada.

```bash
kill -15 <PID>
kill <PID>        # por defecto envía SIGTERM
