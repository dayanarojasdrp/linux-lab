# Permisos para /var/www en servidores web

## Usuario típico del servidor web
www-data

## Cambiar propietario del proyecto
sudo chown -R www-data:www-data /var/www/proyecto

## Permisos recomendados
sudo chmod -R 755 /var/www/proyecto

## Dar permisos de escritura solo a www-data
sudo chmod -R 775 /var/www/proyecto
sudo chown -R www-data:$(whoami) /var/www/proyecto

## Verificar permisos
ls -l /var/www
