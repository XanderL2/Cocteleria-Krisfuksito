# Documentación del Proyecto: Arquitectura Cliente-Servidor (Backend MVC)

![enter image description here](https://raw.githubusercontent.com/XanderL2/Cocktail-Making-Kris/refs/heads/main/docs/main.png)

## Justificación y motivación del proyecto

Este es el proyecto final de M12 hecho por Nil y Alex.

El proyecto es una Pagina interactiva sobre Va-11 Hall-a,
un juego de servir cocteles i emborrachar a los clientes.

Tanto los datos de la API como la tematica
estan basadas en el juego original,
con los cocteles del juego y un ambiente visual de estilo cyberpunk.

## Arquitectura
![](arquitectura.webp)

## Esquema de arquitectura

La arquitectura es de tipo cliente-servidor:
- **Frontend:** Desarrollado en JavaScript (Angular), HTML y CSS.
- **Backend:** Implementado en C# utilizando el framework .NET Core para exponer la API.
- **Base de datos:** SQLite para almacenamiento persistente.
- **Comunicación:** El cliente consume servicios web expuestos por el backend.

```
[Cliente (JS/HTML/CSS)] <----HTTP----> [Servidor .NET Core (C#)] <----> [SQLite]
```

## Tecnologías utilizadas
- **Lenguaje de programación:** C# (backend), JavaScript (frontend)
- **Lenguajes de marcado:** HTML, CSS
- **Framework backend:** .NET Core - API
- **Base de datos:** SQLite
- **Serialización:** Json.NET - Newtonsoft
- **Paradigma:** Programación Orientada a Objetos (POO)


### Características implementadas
- Múltiples rutas en los controladores para gestionar diferentes vistas y acciones.
- Modelos y vistas conectados para mostrar datos tanto de servicios web externos como de la base de datos.
- Serialización y deserialización de datos usando Json.NET (Newtonsoft).
- Maquetado cuidado y validación de accesibilidad (WAVE).
- Añadir autenticación y gestión de usuarios.

## Propuestas de mejora y nuevas funcionalidades
- Mejorar la internacionalización y accesibilidad.
- Implementar tests automatizados (unitarios y de integración).

## Tecnologías utilizadas
- **Lenguajes de programación:** C# (backend), TypeScript/JavaScript (frontend)
- **Lenguajes de marcado:** HTML, CSS
- **Framework frontend:** Angular
- **Framework backend:** .NET Core (API, MVC)
- **Base de datos:** SQLite
- **Serialización:** Json.NET - Newtonsoft
- **Paradigma:** Programación Orientada a Objetos (POO)

## Organización y estructura del código

### Frontend (Angular)
- **Componentes:** Estructuran la interfaz y gestionan la lógica de presentación.
- **Servicios:** Encapsulan la lógica de negocio del cliente y la comunicación con la API.
- **Módulos:** Permiten organizar el código por funcionalidades.
- **Rutas:** Definen la navegación entre vistas.
- **Buenas prácticas:** Uso de POO, separación de responsabilidades, reutilización de componentes, validación de formularios, accesibilidad.

### Backend (.NET Core MVC)
- **Modelos:** Clases que representan las entidades y gestionan la lógica de acceso a datos (ORM, consultas a SQLite).
- **Controladores:** Gestionan las rutas, procesan las peticiones HTTP, consumen servicios web y consultan la base de datos.
- **Vistas:** (En caso de usarlas) Razor/HTML/CSS para mostrar información, aunque en este proyecto la API es consumida por el frontend Angular.
- **Serialización:** Newtonsoft para transformar los datos entre JSON y objetos C#.
- **Buenas prácticas:** Separación de lógica, validación de datos, seguridad, documentación de endpoints.

## Características implementadas
- Múltiples rutas en los controladores y en el frontend para gestionar diferentes vistas y acciones.
- Modelos y vistas conectados para mostrar datos tanto de servicios web externos como de la base de datos.
- Serialización y deserialización de datos usando Json.NET (Newtonsoft).
- Maquetado cuidado y validación de accesibilidad (WAVE).
- Autenticación y gestión de usuarios.
- Ambientación visual cyberpunk y adaptación temática a Va-11 Hall-a.

## Propuestas de mejora y nuevas funcionalidades
- Mejorar la internacionalización y accesibilidad.
- Implementar tests automatizados (unitarios y de integración).
- Añadir un panel de administración para la gestión avanzada de datos.
- Optimizar el rendimiento y la escalabilidad.
- Mejorar la documentación y la cobertura de pruebas.

## Validación y buenas prácticas
- Se ha validado la accesibilidad y usabilidad con la herramienta WAVE.
- Se sigue el patrón MVC (Backend) y la POO y patrones en el Frontend, para garantizar un código limpio y mantenible.



