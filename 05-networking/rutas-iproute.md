# Rutas y enrutamiento con iproute2

## Ver tabla de rutas
ip route

## Añadir ruta
sudo ip route add 10.10.10.0/24 via 192.168.1.1

## Eliminar ruta
sudo ip route del 10.10.10.0/24

## Ver interfaces
ip addr

## Campos importantes de ip route
- default via: puerta de enlace por defecto
- dev: interfaz usada
- metric: prioridad
- proto: origen de la ruta

