📚 Literalura

Autor: Cristian Vanegas

Literalura es un proyecto desarrollado en Java cuyo objetivo es consumir una API REST, procesar respuestas en JSON y persistir información utilizando SQL.
El proyecto se basa en la API pública Gutendex, que proporciona datos de libros del Proyecto Gutenberg.

Este proyecto fue creado con un enfoque educativo y práctico para fortalecer habilidades backend como integración de servicios externos, manejo de datos estructurados y persistencia en bases de datos.

🎯 Objetivo del Proyecto

Consumir una API REST externa

Procesar y mapear respuestas JSON a objetos Java

Organizar la lógica de negocio mediante servicios

Preparar la información para su almacenamiento y consulta usando SQL

Aplicar buenas prácticas de diseño y estructura de código

🛠 Tecnologías Utilizadas

Java 8

Maven

API REST (Gutendex)

JSON

SQL

IntelliJ IDEA

🌐 Uso de API REST

Literalura consume la API pública Gutendex, la cual expone información de libros en formato JSON.

El proyecto realiza:

Peticiones HTTP enviando parámetros de búsqueda (por ejemplo, el título del libro)

Recepción de respuestas JSON con estructuras anidadas

Procesamiento de listas de libros, autores, idiomas y métricas como número de descargas

Ejemplo de funcionalidad:

Búsqueda de libros por título usando el método searchBooks(String title)

📦 Manejo de JSON

Uno de los ejes principales del proyecto es el manejo de JSON.

Las respuestas JSON de la API son transformadas en objetos Java

Se utilizan clases modelo que reflejan la estructura del JSON

Se evita trabajar con datos sin procesar, facilitando validaciones y mantenimiento

Esto permite:

Mayor claridad en el código

Reutilización de datos

Escalabilidad del proyecto

🗄 Uso de SQL

El proyecto está preparado para trabajar con SQL con el fin de:

Almacenar libros y autores obtenidos desde la API

Evitar consultas repetidas a la API

Permitir búsquedas locales más rápidas

Mantener persistencia de la información

La integración con SQL permite manejar los datos de forma estructurada y aplicar principios básicos de persistencia y consulta de información.

🗂 Clases Principales
Author

Representa un autor obtenido desde la API.

Atributos principales:

Nombre

Año de nacimiento

Año de fallecimiento

Book

Representa un libro obtenido desde la API.

Atributos principales:

Título

Idioma

Número de descargas

Lista de autores

⚙ Arquitectura del Proyecto

Servicio dedicado para el consumo de la API (GutendexServiceImpl)

Separación entre lógica de negocio y modelos

Código organizado para facilitar mantenimiento y futuras mejoras

Preparado para escalar hacia una arquitectura más robusta

🚀 Instalación y Ejecución
Requisitos

Java 8 (JDK 8)

Maven

IntelliJ IDEA u otro IDE compatible

Instalación

Clonar el repositorio:

git clone https://github.com/tu-usuario/literalura.git


Ingresar al directorio:

cd literalura


Compilar el proyecto:

mvn clean install


Ejecutar desde el IDE.

📌 Aprendizajes Clave

Consumo de APIs REST en Java

Manejo y transformación de JSON

Modelado de datos con clases Java

Introducción a persistencia con SQL

Organización de proyectos con Maven
