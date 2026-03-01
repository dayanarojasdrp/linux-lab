# Compresión con gzip

## Comprimir un archivo
gzip archivo.log

## Descomprimir un archivo
gunzip archivo.log.gz

## Mantener el archivo original al comprimir
gzip -k archivo.log

## Ver ratio de compresión
gzip -l archivo.log.gz
