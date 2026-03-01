# Resolución de nombres: /etc/hosts y /etc/resolv.conf

## /etc/hosts
Archivo de resolución local. Se consulta antes que DNS.

### Formato
IP  nombre  alias

### Ejemplo
127.0.0.1   miweb.local

## /etc/resolv.conf
Define los servidores DNS del sistema.

### Campos
- nameserver: IP del DNS
- search: sufijos de dominio
- domain: dominio por defecto

### Ver configuración
cat /etc/resolv.conf


