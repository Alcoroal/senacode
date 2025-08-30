🎓 Senacode - Estrategia didáctica para aprender a programar en entornos virtuales
Descripción del Proyecto
Senacode es una plataforma virtual del SENA creada para facilitar el aprendizaje de la programación mediante una estrategia didáctica innovadora. Su enfoque combina contenidos interactivos, retos prácticos y metodologías activas que promueven el aprendizaje autónomo, la creatividad y la resolución de problemas.

El proyecto busca fortalecer la formación en competencias digitales, ampliar el acceso a la educación tecnológica y preparar a los aprendices para los desafíos del mundo digital.

Stack Tecnológico
Backend
Python - Lenguaje principal
FastAPI - Framework web moderno
PostgreSQL - Base de datos relacional
Docker - Contenedores para despliegue y desarrollo local
Frontend
TypeScript - Lenguaje con tipado estático
CSS Modules - Estilos que solo afectan al componente donde se usan, evitando choques con otros.
SASS - Una versión mejorada de CSS que permite usar variables y organizar mejor los estilos.
Mobile
iOS: Swift + SwiftUI
Android: Kotlin + Jetpack Compose
Arquitectura
Frontend (TypeScript)     Mobile Apps (Swift/Kotlin)
        │                           │
        └─────────┬─────────────────┘
                  │
            Backend API (FastAPI)
                  │
            Database (PostgreSQL)
Entidades del Sistema
Course (Curso)
ID único → Un número o código que identifica cada curso (como una cédula para el curso).
Nombre del curso → El título del curso, por ejemplo: “Introducción a Python”.
Descripción → Un pequeño resumen de qué trata el curso.
Thumbnail (imagen) → La imagen de portada del curso (como la carátula de un libro).
Slug para URLs → Una versión corta del nombre para usar en el enlace web, ej: introduccion-python.
Profesores asignados → Lista de los profes que dictan ese curso.
Timestamps de gestión → Fechas de creación y última actualización del curso (útil para saber cuándo fue creado o editado).
Class (Clase)
ID único → Identificador propio de cada clase dentro de un curso.
Pertenece a un curso → Cada clase está dentro de un curso específico.
Nombre de la clase → El título de la clase, ej: “Variables en Python”.
Descripción → Texto corto que explica qué se verá en esa clase.
Slug para URLs → Nombre simplificado para el enlace web de la clase.
URL del video → El enlace del video de la clase (YouTube, Vimeo, o servidor propio).
Timestamps de gestión → Fechas de creación y última actualización de la clase.
Teacher (Profesor)
ID único → Identificador único para cada profesor.
Nombre completo → El nombre real del profesor.
Email de contacto → Correo electrónico del profe (para contacto o gestión).
Timestamps de gestión → Fechas de creación y última actualización del registro del profesor.
El objetivo es conservar el sistema simple y centrado en lo esencial, evitando funciones extra innecesarias.# senacode
