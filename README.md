## SWARM CON SERVICIOS SOAP Y REST

## PASO 1 Crear las imagenes

## Entrar en la carpeta apiRest y ejecutar el siguiente comando
`docker build . -t examen/restapi`
## Entrar en la carpeta en apiSoap y ejecutar el siguiente comando
`docker build . -t examen/soapapi`
## Entrar en la carpeta en client y ejecutar el siguiente comando
`docker build . -t examen/client`
## Entrar en la carpeta en mysql y ejecutar el siguiente comando
`docker build . -t examen/mysql`

## PASO 2 Desplegar los servicios con swarm

`docker swarm init`

`docker stack deploy -c docker-compose.yml servicios`

## Aclaraciones

Se creo el servidor SOAP en el puerto 4000

El servidor web se encuentra alojado en localhost:8080