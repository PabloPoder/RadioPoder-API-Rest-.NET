# RadioPoder - API .NET 6

[![GitHub Last Commit](https://img.shields.io/github/last-commit/PabloPoder/RadioPoder-Api.Net6?logo=github)](https://github.com/PabloPoder/RadioPoder-Api.Net6/commits/main)
[![GitHub Repo Size](https://img.shields.io/github/repo-size/PabloPoder/RadioPoder-Api.Net6?logo=github)](https://github.com/PabloPoder/RadioPoder-Api.Net6)

## ⚙️ API Rest desarrollada con .NET Core

Esta es la API Restful desarrollada con .NET Core que proporciona los servicios de backend para la aplicación móvil [Radio Poder desarrollada en Flutter](https://github.com/PabloPoder/RadioPoder-Flutter). Permite la gestión de noticias, comentarios, usuarios, sorteos y participaciones, facilitando la interacción dinámica de datos en la aplicación móvil.

## 📱 Repositorio de la Aplicación Móvil Flutter:
[![Enlace al Repositorio de Flutter](https://img.shields.io/badge/Ver%20App%20Flutter-1769FF?style=for-the-badge&logo=flutter)](https://github.com/PabloPoder/RadioPoder-Flutter)

## 🏗️ Modelo UML
![Diagrama UML de la API Radio Poder](https://user-images.githubusercontent.com/50326883/203380289-fb42008b-753a-42b9-a46a-027a48de4b1f.png)

Este diagrama UML representa la estructura y las relaciones principales de los modelos de datos utilizados en la API.

## Endpoints de la API ⚡

A continuación, se describen los endpoints principales de la API y las operaciones que soportan:

### Comentarios
* **GET** `/api/Comentarios/{id}`: Obtiene un comentario específico por su ID.
* **GET** `/api/Comentarios`: Obtiene todos los comentarios.
* **PUT** `/api/Comentarios/{id}`: Actualiza un comentario existente.
* **DELETE** `/api/Comentarios/{id}`: Elimina lógicamente un comentario (puede que no se borre de la base de datos).

### Noticias
* **GET** `/api/Noticias/{id}`: Obtiene una noticia específica por su ID.
* **GET** `/api/Noticias`: Obtiene todas las noticias.
* **POST** `/api/Noticias`: Crea una nueva noticia.
* **GET** `/api/Noticias/{id}/TiempoDeLectura`: Obtiene el tiempo estimado de lectura para una noticia específica.

### Usuarios
* **GET** `/api/Usuarios/{id}`: Obtiene un usuario específico por su ID.
* **GET** `/api/Usuarios`: Obtiene todos los usuarios.
* **GET** `/api/Usuarios/Email/{email}`: Obtiene un usuario específico por su dirección de correo electrónico.
* **POST** `/api/Usuarios/Login`: Permite a un usuario iniciar sesión.
* **POST** `/api/Usuarios/Register`: Permite a un nuevo usuario registrarse.
* **GET** `/api/Usuarios/Logeado`: Obtiene la información del usuario actualmente autenticado.
* **PUT** `/api/Usuarios/Editar`: Permite editar la información del usuario autenticado.
* **PUT** `/api/Usuarios/EditarGoogle`: Permite editar la información del usuario autenticado a través de Google.

### Sorteos
* **GET** `/api/Sorteos/{id}`: Obtiene un sorteo específico por su ID.
* **GET** `/api/Sorteos`: Obtiene todos los sorteos.
* **GET** `/api/Sorteos/{id}/Ganador`: Obtiene el ganador de un sorteo específico.
* **POST** `/api/Sorteos`: Crea un nuevo sorteo.

### Participaciones
* **GET** `/api/Participaciones/{id}`: Obtiene una participación específica por su ID.
* **GET** `/api/Participaciones`: Obtiene todas las participaciones.
* **POST** `/api/Participaciones`: Crea una nueva participación.
* **DELETE** `/api/Participaciones/{id}`: Elimina una participación específica.

## 🛠️ Tecnologías Utilizadas
* [.NET Core](https://dotnet.microsoft.com/en-us/learn/aspnet/what-is-aspnet-core) - Framework para construir la API Rest.
* C# - Lenguaje de programación utilizado en .NET Core.
* RESTful API - Arquitectura de la interfaz de comunicación entre la app y el servidor.

## 🤝 Contribución
Si deseas contribuir a este proyecto, ¡eres bienvenido! Puedes hacerlo de las siguientes maneras:

* Reportar errores o problemas (Issues).
* Proponer mejoras o nuevas funcionalidades (Pull Requests).
* Mejorar la documentación de la API.
