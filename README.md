# UNIVERSIDAD TÉCNICA ESTATAL DE QUEVEDO

**TEMA:**
INFORME DE EXPOSICIONES SOBRE FRAMEWORK

**PRESENTADO POR:**
PANAMA MURILLO MOISES ANTONIO

**DOCENTE:**
DR. GLEISTON CICERÓN GUERRERO ULLOA, PH.D.

**CURSO:**
5TO SOFTWARE A

**FECHA:**
VIERNES, 30 DE JULIO DEL 2026

---

## GRUPO SVELTE

**Fred Beltrán:** Presenta Svelte y el consumo de APIs, explicando cómo se iba a desarrollar la exposición y las demostraciones. Habla de la historia y características de Svelte y SvelteKit, comparándolo con React en temas de latencia, rendimiento y librerías pesadas. Explica que el virtual DOM se usa en tiempo de construcción y que SvelteKit da versatilidad full stack en los endpoints. Muestra la estructura minimalista del proyecto (main.js) y el consumo de la API con métodos GET, POST, DELETE, etc. Explica que Svelte es un framework de frontend, con código limpio y directo, usando como ejemplo su pfc BIOPET de veterinaria, donde Svelte no tiene relación con el backend. Explica el login, el uso de JWT y Spring Boot, y en la demo muestra el frontend sin GET/POST configurados aún. Concluye con ventajas (reactividad, curva de aprendizaje sencilla) y desventajas (poca info, poco uso en Ecuador, ecosistema pequeño frente a React).

**Alison Zambrano:** Explica que Svelte trabaja con backend y frontend separados, no como una estructura unificada tipo Laravel, y que es apto para proyectos grandes. Pone de ejemplo un sistema de biblioteca, donde el usuario solo ve el frontend, no el código. Explica el flujo: el usuario registra correo y contraseña, el fetch actúa como intermediario que envía esos datos por POST al backend, y si son correctos se entrega un token que se guarda. En la demo muestra cómo se levanta primero el backend y luego el frontend, que es lo que finalmente ve el cliente.

## GRUPO ALPINE.JS

**Marlon Loor:** Explica que antes su ejemplo era solo frontend, y que ahora incluye backend y persistencia de datos con SQLite y la librería de Alpine.js. Explica que usa fetch con Express.js como backend y SQLite como base de datos embebida y ligera, que funciona sin internet. Muestra el index.html, cómo se importa la librería para usar x-data, y los scripts para hacer el CRUD. Explica que todo se maneja en un server.js sin controladores separados, levantado en el puerto 3000. Muestra también un ejemplo en Spring Boot en el puerto 8080 con los endpoints de autenticación. Explica el proyecto ARTISYNC, con el formulario de login y registro usando x-model, fetch y funciones asíncronas. Concluye con las ventajas de Alpine (curva de aprendizaje corta, pocos atributos y métodos) y la desventaja de que se limita mucho para proyectos más complejos.

## GRUPO NEXT.JS

**Alejandro Pallo:** Explica que su ejemplo se basa en React y consume una API desde el frontend. En la demo crea el proyecto con npm create next, configurándolo manualmente sin TypeScript ni compilador extra, usando CSS plano. Explica que los datos vienen del backend en Spring Boot, de un sistema de gestión para una escuela deportiva. Explica el archivo de configuración que conecta con el backend, la función de login y el GET para traer los datos de estudiantes. Explica cómo se cierra sesión, invalidando el estado guardado, y cómo se define la estructura HTML de cada página. Finalmente levanta el backend de su pfc y muestra los datos ya cargados en el frontend.

## GRUPO ASTRO

**Irvin Cajas:** Presenta el acceso a datos vía API REST y explica que Astro se lanzó en 2021 como proyecto open source, buscando reducir lo que se envía al navegador. Explica su arquitectura de islas, donde por defecto se manda HTML estático y no JS, y que define rutas sin enrutador, usando fetch para consumir APIs. En la demo muestra su pfc de gestión de biblioteca, explicando el GET y el POST con JWT para proteger la base de datos. Presenta una tabla comparativa entre Astro, Express, Laravel y Django según curva de aprendizaje y uso de ORM.

**Jaime Mariscal:** Con un ejemplo de veterinaria, explica cómo el listado de mascotas se obtiene por GET desde la base de datos a través del ORM. En la demo explica cómo Astro se conecta con Spring Boot y PostgreSQL usando Docker, inicia sesión como administrador y consulta los endpoints protegidos. Explica el manejo del token del usuario autenticado y cómo el GET solo lee registros sin modificarlos. Muestra las mascotas guardadas a través de la API. Menciona un caso real de una empresa en Brasil que usa Astro más allá de lo educativo, y comenta que en Ecuador no se usa mucho, pero sí en Colombia y Brasil.

**Maria Escudero:** Explica la estructura de un proyecto en Astro (public, components, layouts, pages, config, package.json, etc.) antes de pasar a la práctica. En la demo muestra su pfc consumiendo GET y POST, con backend y frontend ya inicializados, y explica cómo el backend devuelve un token que se guarda para usarlo después. Muestra el login y el registro de conductores. Explica ventajas (buen rendimiento, poco JS, se adapta a distintas tecnologías) y desventajas (no es backend tradicional, no trae ORM). Concluye que Astro es más una interfaz rápida que un framework backend.

## GRUPO QWIK CITY

**Kevin Castro:** Presenta el tema y explica la historia de Qwik, además de la estructura de la exposición. Explica la instalación de Qwik City y los comandos necesarios (npm create qwik@latest, drivers, drizzle, etc.), y cómo se verifica todo con qwik build. Recomienda Qwik con una valoración de 50/50, señalando que requiere esfuerzo aprenderlo bien.

**Romero:** Explica, con su pfc, cómo Qwik City usa routeAction$ para consumir una API existente y enviar datos. Explica que Qwik no tiene ORM propio, sino que depende del backend que expone la API, y menciona el uso de variables de entorno. Como ventaja destaca que envía menos JS al navegador; como desventaja, que su comunidad aún es pequeña y con poca documentación.

**Zaida Taipe:** Explica quién usa Qwik y menciona ejemplos de empresas ecuatorianas que lo documentan en sus proyectos, comparándolo con Next.js y Laravel. Explica su pfc, donde la API REST ya existe en Spring Boot y solo se muestra el consumo. Explica el árbol de carpetas, el archivo .env, el sufijo .server.ts para que el código no se exponga al cliente, y las funciones CRUD. Explica cómo routeLoader, routeAction, routeAction, routeAction y Zod trabajan juntos para traer y validar los datos. Hace una demo agregando, editando y eliminando una mascota desde el sistema.

## GRUPO SOLID.JS / SOLIDSTART

**Tejada:** Explica la historia de Solid y cómo se formó SolidStart como proyecto open source. Explica la estructura del proyecto (carpeta src, .env, package.json) y muestra su pfc de una cooperativa de transporte, con el módulo de conductores y sus endpoints usando Drizzle ORM. Explica en Postman un GET y un POST para consultar y agregar conductores. Concluye que no recomienda Solid para proyectos de fin de curso por ser muy reciente y con poca documentación, aunque destaca que no usa virtual DOM y es rápido para proyectos pequeños.

**Moncayo:** Explica el proceso de aprendizaje del framework y presenta la práctica de su pfc. Explica que SOLID es un acrónimo de los principios de diseño, relacionando cada carpeta de su proyecto (validación, notificaciones, tribunal, roles, actas) con una de las letras. Muestra el proyecto levantado en el puerto 8080, con las interfaces de docente, estudiante y titular, además del módulo de tribunal y acta generada.

## GRUPO REACT

**Ricardo Vélez:** Explica cómo nació React en Meta y conceptos como el virtual DOM y useEffect. Presenta su pfc con JWT, explicando el archivo api.js, el interceptor que agrega el token automáticamente, y el authService con la función de login y el refresh token. Explica que el login maneja credenciales, errores y estado de carga. Explica app.js como guardián que verifica el token para proteger las rutas, y cómo al cerrar sesión se elimina el token y se borra el historial para no poder volver atrás.

**Arcalle:** Explica cómo consumir la API de estudiantes a través de varios servicios (categorías, personas, estudiantes) con GET paginado y funciones para crear, actualizar y eliminar. Explica cómo la página de estudiantes usa useState y useEffect para manejar los datos, y un patrón de limpieza para evitar condiciones de carrera al cambiar de página. Explica handleOpenModal y handleChange, y muestra el formulario para editar, crear y eliminar estudiantes.

**Fajardo:** Explica la estructura de su proyecto en React (app.jsx, useState, useEffect), siendo su pfc un asistente de tareas. Explica el fetch que trae los datos del backend y el uso de await res.json() para redibujar la lista. Explica la entidad Tarea mapeada a PostgreSQL y el controlador con @GetMapping. Muestra cómo la página hace GET y POST directamente al backend, apoyándose en Spring Boot.
