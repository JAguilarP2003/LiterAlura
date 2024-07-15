
---

# LiterAlura

**LiterAlura** es una aplicación Java/Spring Boot diseñada para gestionar libros y autores utilizando la API de Gutendex y una base de datos PostgreSQL.

## Características

- **Buscar libro por título:** Permite buscar libros por su título utilizando la API de Gutendex.
- **Registro de libros y autores:** Permite registrar libros y autores obtenidos de la API.
- **Consultas y listados:** Ofrece varias consultas como listar todos los libros registrados, listar autores registrados, listar autores vivos en un determinado año, y listar libros por idioma.
- **Interfaz de línea de comandos (CLI):** Implementa un menú interactivo para ejecutar las diferentes funcionalidades.

## Tecnologías Utilizadas

- Java 11
- Spring Boot 2.5.0
- PostgreSQL
- Hibernate
- Jackson JSON

## Configuración

Para configurar la aplicación, asegúrate de tener configuradas las siguientes propiedades en tu archivo `application.properties`:

```properties
spring.application.name=literAlura
spring.datasource.url=jdbc:postgresql://${DB_HOST}/literalura
spring.datasource.username=${DB_USER}
spring.datasource.password=${DB_PASSWORD}
spring.datasource.driver-class-name=org.postgresql.Driver
hibernate.dialect=org.hibernate.dialect.HSQDialect

spring.jpa.hibernate.ddl-auto=update

spring.jpa.show-sql=true
spring.jpa.format-sql=true
```

Reemplaza `${DB_HOST}`, `${DB_USER}` y `${DB_PASSWORD}` con los valores correspondientes de tu entorno.

## Ejecución

Para ejecutar la aplicación, puedes utilizar Maven desde la línea de comandos:

```bash
mvn spring-boot:run
```

Esto iniciará la aplicación y mostrará el menú interactivo en la consola.

## Contribuciones

Las contribuciones son bienvenidas. Si deseas contribuir a este proyecto, por favor crea un *pull request* detallando tus cambios propuestos.

## Autor

[JAguilarP2003](https://github.com/JAguilarP2003)

---

