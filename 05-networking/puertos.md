# Puertos y servicios en Linux

## Ver puertos abiertos
sudo ss -tulnp

## Ver proceso asociado a un puerto
sudo ss -tulnp | grep 80

## Escuchar un puerto (prueba)
nc -l 8080

## Probar conexión a un puerto remoto
nc -vz 192.168.1.10 22
