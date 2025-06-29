# T02_03_Grupo01_RomeroAndre
Proyecto grupal para la materia ingeniera de software
# Sistema de Gestión de Minimercado - SGM

Este proyecto corresponde al desarrollo de un sistema backend para la gestión de un minimercado, cumpliendo con los requerimientos de las Tareas T02_01 y T02_02.

El sistema fue construido utilizando **Spring Boot**, siguiendo una arquitectura modelo/repositorio/servicio/controlador, e incluye documentación automática de los servicios mediante **Swagger/OpenAPI**.

## 🧑‍💻 Miembros del grupo

- Andre Alessandro Romero Martínez  
- Katherine Leonor Moran Zavala  
- Luis Daniel Montaleza Ortiz  

---

## 📦 Contenido del Proyecto

Este backend proporciona la gestión de las siguientes entidades principales:

- **Usuarios y Roles**: Control de acceso básico por rol (estructura lista, sin seguridad implementada aún).
- **Clientes**: Registro y gestión de clientes.
- **Proveedores**: Registro y gestión de proveedores.
- **Categorías**: Clasificación de productos.
- **Productos**: Inventario de productos.
- **Órdenes de Compra**: Registro de compras a proveedores.
- **Ventas y Detalle de Venta**: Registro de ventas a clientes.
- **Caja**: Control básico de apertura y cierre de caja.

Cada entidad dispone de un CRUD completo expuesto como servicios REST, documentados en Swagger.

---

## ⚙️ Tecnologías Utilizadas

- Java 17  
- Spring Boot 3.x  
- Spring Data JPA  
- MySQL  
- Springdoc OpenAPI (Swagger)  
- Maven  

---

## 🚀 Instrucciones para ejecutar el proyecto

### Requisitos Previos:

- Tener instalado **Java 17** o superior.  
- Tener instalado **MySQL Server**.  
- Crear la base de datos ejecutando en MySQL:

```sql
CREATE DATABASE minimercado;
# Configuración

## Instalación

### 1. Clona el repositorio:
```bash
git clone https://github.com/tu-usuario/sgm.git
cd sgm
```

### 2. Configura tus credenciales de MySQL en el archivo:
```
src/main/resources/application.properties
```

**Ejemplo de configuración:**
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/minimercado?useSSL=false&allowPublicKeyRetrieval=true&serverTimezone=UTC (puerto usado 3307)
spring.datasource.username=root (admin)
spring.datasource.password=tu_contraseña (12345)
```

### 3. Compila e instala dependencias:
```bash
./mvnw clean install -DskipTests
```

### 4. Ejecuta el proyecto:
```bash
./mvnw spring-boot:run
```

## 🧩 Acceso a la Documentación y Pruebas

Una vez en funcionamiento, accede a:
```
http://localhost:8080/swagger-ui/index.html
```

Desde Swagger podrás visualizar, probar y consumir todos los servicios REST implementados.

## 🗄️ Base de Datos

- El sistema crea automáticamente las tablas al iniciar, gracias a Hibernate.
- Los datos se almacenan de forma persistente en la base de datos `minimercado`.

## ⚠️ Notas Finales

- Actualmente, el sistema no tiene autenticación implementada.
- Para un entorno productivo, se recomienda agregar seguridad (encriptación de contraseñas, control de acceso).

## ✔️ Estado Actual

- ✅ Entidades principales listas
- ✅ CRUD funcional para cada módulo
- ✅ Documentación Swagger disponible
- ✅ Persistencia en MySQL configurada
