# Documentación Técnica — Tarjeta de Presentación Digital

Este documento describe la estructura semántica y las decisiones técnicas tomadas
en el desarrollo de la **Tarjeta de Presentación Digital**, creada como parte del
**Módulo 4: Código Desorganizado vs. Estructurado**.

El objetivo principal del archivo HTML es demostrar el uso correcto de **HTML5 semántico**,
manteniendo un código limpio, accesible y comprensible sin depender de estilos visuales.

---

## Decisiones Semánticas

A continuación se explica el motivo de uso de cada etiqueta principal:

### `<html lang="es">`
Se declaró el idioma del documento para que los navegadores, buscadores y lectores
de pantalla identifiquen correctamente el idioma del contenido.

### `<head>`
Contiene metadatos esenciales:
- `<meta charset="UTF-8">` asegura la correcta visualización de tildes y caracteres especiales.
- `<meta name="viewport">` permite una correcta visualización en dispositivos móviles.
- `<title>` y `<meta description>` mejoran la accesibilidad y el SEO.

### `<header>`
Se utilizó para agrupar la información principal de identidad:
- Nombre completo
- Rol o descripción
- Navegación principal del documento

Representa la introducción del sitio.

### `<nav>`
Se empleó para organizar los enlaces internos de la tarjeta.
Incluye `aria-label` para mejorar la accesibilidad y permitir que lectores de pantalla
comprendan la función del bloque.

### `<main>`
Contiene el contenido central del documento.
Su uso es clave para que buscadores y tecnologías de asistencia identifiquen
el contenido principal de la página.

### `<section>`
Se usó para dividir el contenido en bloques temáticos claros:
- Perfil profesional
- Habilidades
- Formación académica

Cada sección tiene un encabezado (`<h2>`) que describe su propósito.

### `<article>`
Se utilizó dentro de la formación académica para representar una unidad de contenido
independiente y reutilizable (un curso específico).

### `<time>`
Se empleó para representar fechas de forma legible tanto para humanos como para máquinas.

### `<aside>`
Contiene información complementaria relacionada con el contenido principal,
en este caso, los datos de contacto.

### `<address>`
Se utilizó correctamente para representar información de contacto personal.

### `<footer>`
Incluye información legal y contextual, como derechos de autor y el propósito educativo
del documento.

---

## Árbol DOM (Representación Visual)

Estructura jerárquica del documento HTML:

html
├── head
│   ├── meta (charset)
│   ├── meta (viewport)
│   ├── title
│   └── meta (description)
└── body
├── header
│   ├── h1
│   ├── p
│   └── nav
│       └── ul
│           ├── li → a
│           ├── li → a
│           └── li → a
├── main
│   ├── section (Perfil)
│   │   ├── h2
│   │   └── p
│   ├── section (Habilidades)
│   │   ├── h2
│   │   └── ul
│   │       ├── li
│   │       ├── li
│   │       ├── li
│   │       └── li
│   └── section (Formación)
│       ├── h2
│       └── article
│           ├── header
│           │   ├── h3
│           │   └── time
│           └── p
├── aside
│   └── section
│       ├── h2
│       └── address
│           ├── p
│           └── p
└── footer
└── small


---

## Conclusión

El archivo demuestra cómo una estructura semántica correcta permite que el código sea:
- Legible sin necesidad de estilos CSS
- Accesible para tecnologías de asistencia
- Fácil de mantener y comprender
- Compatible con estándares modernos de la web

Esta práctica evidencia que la verdadera diferencia entre un código desorganizado
y uno estructurado no está en lo visual, sino en el significado que el código comunica.
