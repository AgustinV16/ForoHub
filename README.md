# ForoHub

ForoHub es una aplicación web desarrollada con Spring Boot, JPA, Flyway y MySQL, diseñada para facilitar la creación y gestión de foros temáticos. Incluye autenticación segura con JWT, relaciones entre usuarios y roles, migraciones automatizadas, y una arquitectura limpia orientada a buenas prácticas.


## Funcionalidades principales

-  Autenticación con JWT y protección de endpoints.
-  Gestión de usuarios con roles (`ROLE_USER`, `ROLE_ADMIN`) mediante relación ManyToMany.
-  Creación, edición y visualización de publicaciones en foros.
-  Migraciones automáticas con Flyway para mantener el esquema alineado con las entidades.
-  Pruebas de endpoints con Insomnia/Postman.
-  Documentación clara y trazabilidad técnica.


## Tecnologías utilizadas

- Java 17
- Spring Boot 3
- Spring Security 6 + JWT
- Spring Data JPA (Hibernate)
- MySQL / H2 (dependiendo del perfil)
- Swagger / OpenAPI 3
- Maven como gestor de dependencias

## Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/BrianSilenT/ForoHub.git
   cd ForoHub

   
2. Configurar base de datos: 
   ```bash
   spring.datasource.url=jdbc:mysql://localhost:3306/forohub
   spring.datasource.username=tu_usuario
   spring.datasource.password=tu_contraseña
   spring.jpa.hibernate.ddl-auto=none
   spring.flyway.enabled=true

3. Compilar y Ejecutar:
   ```bash
   mvn clean install
   mvn spring-boot:run
