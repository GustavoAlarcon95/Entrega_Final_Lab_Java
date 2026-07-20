# E-commerce API - Proyecto Final Back-End Java

## Descripción del proyecto

Este proyecto corresponde a la entrega del Proyecto Final del curso **Back-End en Java**.

Consiste en una API REST desarrollada con **Spring Boot** que permite gestionar un sistema básico de e-commerce. La aplicación incluye la administración de productos, categorías y carrito de compras, utilizando **MySQL** como base de datos y aplicando una arquitectura por capas (Controller, Service, Repository y Model).

---

## Instrucciones para ejecutar la aplicación

### Requisitos

* Java 17 o superior.
* Maven.
* MySQL.
* Visual Studio Code (con las extensiones de Java y Spring Boot).

### Pasos

1. Clonar el repositorio.
2. Crear la base de datos en MySQL.
3. Configurar las credenciales de la base de datos en el archivo `application.properties`.
4. Abrir el proyecto en Visual Studio Code.
5. Esperar a que Maven descargue las dependencias del proyecto.
6. Ejecutar la clase principal `EcommerceApplication`.
7. La API quedará disponible en `http://localhost:8080`.
8. Probar los endpoints utilizando Thunder Client o Postman.


---

## Ejemplos de uso / Datos de prueba

Una vez iniciada la aplicación pueden probarse los principales endpoints utilizando Postman o Thunder Client.

### Obtener todos los productos

```http
GET /productos
```

### Obtener todas las categorías

```http
GET /categorias
```

### Crear un carrito

```http
POST /carritos
```

### Agregar un producto al carrito

```http
POST /carritos/{idCarrito}/productos/{idProducto}
```

El proyecto incluye datos de prueba iniciales para facilitar la verificación del funcionamiento de la API.
