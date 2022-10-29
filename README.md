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

5. Reconstruir las bases de datos con la semilla

```
http://localhost:3000/api/v2/seed
```

## Stack Usado

- MongoDB
- Nest
