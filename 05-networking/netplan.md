# Configuración de red con Netplan

## Archivos de configuración
/etc/netplan/*.yaml

## Aplicar cambios
sudo netplan apply

## Configuración estática (ejemplo)
network:
  version: 2
  ethernets:
    ens33:
      dhcp4: no
      addresses:
        - 192.168.1.50/24
      gateway4: 192.168.1.1
      nameservers:
        addresses: [8.8.8.8, 1.1.1.1]

## Configuración DHCP (ejemplo)
network:
  version: 2
  ethernets:
    ens33:
      dhcp4: yes

## Validar configuración
sudo netplan try
