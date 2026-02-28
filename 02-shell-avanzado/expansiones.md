# Expansiones en Shell (Nivel Junior+)

## Objetivo
Dominar las expansiones del shell para automatizar tareas, generar listas, y manipular patrones sin escribir comandos repetitivos.

## Tipos de expansiones

### 1. Expansión de comodines (globbing)
- `*` — coincide con cero o más caracteres.
- `?` — coincide con un solo carácter.
- `[abc]` — coincide con cualquiera de esos caracteres.
- `[a-z]` — coincide con un rango.

#### Ejemplos
```bash
ls *.txt
ls archivo?.md
ls imagen[1-3].png
