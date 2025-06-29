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
