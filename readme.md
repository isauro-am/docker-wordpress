# Docker Wordpress

Requisitos
- Docker
- Docker-compose

Previo a ejecutarlo, es recomendable configurar las contraseñas destinadas para la base de datos así como definir un nombre apropiado para nuestro usuario y nombre de la base de datos.

```yaml
    environment:
      MYSQL_ROOT_PASSWORD: mysqlRootPsswdDB
      MYSQL_DATABASE: wordpress
      MYSQL_USER: wP-userDB
      MYSQL_PASSWORD: wP-psswdDB

...

      WORDPRESS_DB_USER: wP-userDB
      WORDPRESS_DB_PASSWORD: wP-psswdDB
      WORDPRESS_DB_NAME: wordpress
```

Al ejecutar el servicio, quedara expuesto nuestro wordpress por el puerto 2000, siendo accedido mediante http://localhost:2000/

```bash
docker-compose up -d
```

