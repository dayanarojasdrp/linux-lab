# Rutas y tablas de enrutamiento con iproute2

## Ver la tabla de rutas
ip route

## Conceptos clave
- **default via**: puerta de enlace por defecto.
- **dev**: interfaz usada.
- **metric**: prioridad de la ruta.
- **proto**: quién creó la ruta.

## Añadir una ruta
sudo ip route add 10.10.10.0/24 via 192.168.1.1

## Eliminar una ruta
sudo ip route del 10.10.10.0/24

## Ver interfaces
ip addr

## Práctica
1. Ver tu default gateway.
2. Añadir una ruta falsa.
3. Confirmarla con `ip route`.
4. Borrarla.
