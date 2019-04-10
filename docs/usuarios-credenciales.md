# Crear Usuario
`eg users create`
# Asignar credencial al usuario
`eg credentials create -c rasec -t key-auth -q`

> type ket-auth ---> debe agregarse la cabecera    Authorization > *apikey asjdlkasjd:asdkjaslkdjaskdl*

# REDIS
https://guiadev.com/curso-basico-redis-parte-02/
https://tecadmin.net/install-redis-on-debian-9-stretch/
## configuracion
https://www.solvetic.com/tutoriales/article/3763-como-instalar-configurar-redis-ubuntu-17-10/

## instalacion DEBIAN 9 
sudo aptitude install redis-server redis-tools redis-sentinel node-node-redis

## iniciar servicios en fedora
sudo systemctl start redis

## instalar redis connection en elproyecto
npm i connect-redis --save



## saber version de redis

redis-server --version

## CLIENTE de redis
redis-cli

## comprobar conexxion
> ping
(resultado bueno) > PONG
## Redis guarda su respaldo :
/var/lib/redis

## aseginar clave y valor
`set miclave mivalor`
## obtener valor
`get miclave`

## listar todas las KEYS
> redis-cli --scan --pattern *
> redis-cli KEYS *

## OPERACIONES DE LECURA
Here are the commands to retrieve key value:

> if value is of type string -> GET <key>
> if value is of type hash -> HGETALL <key>
> if value is of type lists -> lrange <key> <start> <end>
> if value is of type sets -> smembers <key>
> if value is of type sorted sets -> ZRANGEBYSCORE <key> <min> <max>
command to check the type of value a key mapping to:
> type <key>



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



https://github.com/techyugadi/egcompose

