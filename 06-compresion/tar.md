# Compresión y empaquetado con tar

## Crear un archivo .tar
tar -cvf archivo.tar carpeta/

## Extraer un archivo .tar
tar -xvf archivo.tar

## Crear un archivo .tar.gz (empaquetar + comprimir)
tar -czvf archivo.tar.gz carpeta/

## Extraer un archivo .tar.gz
tar -xzvf archivo.tar.gz

## Flags principales
- c: create
- x: extract
- v: verbose
- f: file
- z: gzip
