# DHCP y NAT

## DHCP
Protocolo que asigna IP automáticamente.

### Renovar IP
sudo dhclient -r
sudo dhclient

## NAT
Traducción de IP privadas a públicas.

### Ver reglas NAT
sudo iptables -t nat -L -n -v

### Regla MASQUERADE (ejemplo)
sudo iptables -t nat -A POSTROUTING -o ens33 -j MASQUERADE
