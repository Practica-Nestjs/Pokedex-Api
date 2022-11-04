<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Ejecutar en Desarrollo

1. Clonar el Repositorio
2. Ejecutar

```
$ npm install
```

3. Tener Nest CLI instalado

```
$ npm i -g @nestjs/cli
```

4. Levantar la base de datos (Verificar que Docker este ejecutando en segundo plano)

```
$ docker compose up -d
```

5. Clonar el archivo **.env.templeate** y renombrar la copia a **.env**

6. Llenar las variables de entorno definidas en el `.env`

7. Ejecutar la aplicacion en dev:

```
npm run start:dev
```

5. Reconstruir las bases de datos con la semilla

```
http://localhost:3000/api/v2/seed
```


## Stack Usado

- MongoDB
- Nest

# Production Build
1. Crear el archivo ```.env.prod``` 
2. Llenar las variables de entorno para productcion
3. Crear la nueva imagen 
```
$ docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```
4. Para cuando se requiera ejecutar la imagen nuevamente, se implementa
```
$ docker-compose -f docker-compose.prod.yaml --env-file .env.prod up -d
```