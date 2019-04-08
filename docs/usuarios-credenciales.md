# Crear Usuario
`eg users create`
# Asignar credencial al usuario
`eg credentials create -c rasec -t key-auth -q`

# REDIS
https://guiadev.com/curso-basico-redis-parte-02/

## iniciar servicios en fedora
sudo systemctl start redis

## saber version de redis

redis-server --version

## CLIENTE de redis
redis-cli
> redis no identifica la DB por nombre , si no por numero (0 - 15) solo 16 base de datos. para desplazarnos entre ellas :

select 1

> Para que veas de manera gráfica la cantidad de bases de datos

CONFIG GET databases

> Redis dispone de cinco estructuras de datos:
- “clave” es lo que utiliza Redis para identificar el conjunto de datos
    "key" "valor"
"key" puede ser cualquier  nombre
"valor" puede ser: 
Cadena de texto
Listas
Hashes
Conjunto
Conjunto ordenados

## aseginar clave y valor
`set miclave mivalor`
## obtener valor
`get miclave`

https://github.com/techyugadi/egcompose

