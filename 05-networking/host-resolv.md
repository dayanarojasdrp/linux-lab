# Resolución local y DNS en Linux (`/etc/hosts` y `/etc/resolv.conf`)

## Archivo /etc/hosts
Linux consulta primero este archivo antes de preguntar a un DNS. Permite resolver nombres de forma local.

### Formato
IP  nombre  alias

### Ejemplo
127.0.0.1 miweb.local

### Probar resolución
ping miweb.local

## Archivo /etc/resolv.conf
Define los servidores DNS que el sistema usará.

### Campos importantes
- **nameserver**: dirección IP del DNS.
- **search**: sufijos de dominio que se añaden automáticamente.
- **domain**: dominio por defecto.

### Ver configuración actual
cat /etc/resolv.conf

### Cambiar DNS temporalmente
sudo nano /etc/resolv.conf nameserver 8.8.8.8

## Práctica
1. Crear un dominio local en `/etc/hosts`.
2. Probarlo con `ping`.
3. Cambiar DNS en `resolv.conf`.
4. Verificar con `nslookup` o `dig`.
