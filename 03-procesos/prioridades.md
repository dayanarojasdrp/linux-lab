# Prioridades de Procesos: nice y renice 

## Objetivo
Controlar la prioridad de CPU de un proceso para que consuma más o menos recursos según la necesidad.

## Qué es nice
Es un valor que indica qué tan “amable” es un proceso con los demás.

- Rango: de -20 a 19
- Mientras más **alto** el número → menos prioridad
- Mientras más **bajo** el número → más prioridad

Valores típicos:
- Procesos normales: 0
- Procesos que deben ser suaves: 10–19
- Procesos que necesitan prioridad: -5 a -20 (requiere sudo)

---

## Crear un proceso con nice

### Prioridad baja (menos CPU)
```bash
nice -n 10 comando
