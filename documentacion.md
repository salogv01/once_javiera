# Decisiones semánticas

Para hacer mi tarjeta de presentación utilicé etiquetas semánticas de HTML5 con el objetivo de darle una estructura comprensible al código.

---

## Estructura general

### `<header>`
La utilicé para agrupar el título inicial, mi nombre y la frase. Esta es la introducción del contenido.

### `<main>`
Tiene el contenido principal de la página. Es donde se encuentra toda la información relevante.

### `<footer>`
Contiene la información de mi correo (contacto) y los derechos de autor. Es el cierre de mi tarjeta de presentación.

---

## Organización del contenido

### `<section>`
Lo puse para dividir el contenido en secciones:

- Sobre mí  
- Habilidades  
- Pasatiempos  
- Contacto  

### `<article>`
Lo utilicé dentro de la sección **"Pasatiempos"** para poner cada actividad en una lista.

---

## Encabezados

- `<h1>`: El título principal de la página.  
- `<h2>`: Algunos subtítulos de bloques principales.  
- `<h3>`: Subtítulos dentro de los artículos.  
- `<h4>`: Un subtítulo en el footer.  

---

## Etiquetas de texto

- `<p>`: Para los párrafos de texto.  
- `<strong>`: Para poner en negrita información relevante.  
- `<em>`: Para hacer énfasis o adquirir un tono reflexivo.  

---

## Etiquetas especializadas

### `<time>`
Lo utilicé para las fechas porque esto permite que las máquinas lo interpreten.

### `<ul>` y `<li>`
Para ordenar mis habilidades como una lista.

### `<address>`
Para la información de contacto y para indicar semánticamente que es la información de ubicación o de comunicación.

### `<a href="...">`
Permite que se envíen correos desde el enlace.

### `<small>`
Para poner texto menos relevante visualmente.

### `<hr>`
Para separar visualmente secciones importantes (header / main / footer).

---

## Árbol DOM

Esta es la estructura jerárquica de la página:

```plaintext
html
├── head
│   ├── meta (charset="UTF-8")
│   ├── meta (viewport)
│   └── title
│
└── body
    ├── header
    │   ├── h1
    │   ├── h2
    │   └── p
    │       └── em
    │
    ├── main
    │   ├── section (Sobre mi)
    │   │   ├── h2
    │   │   ├── p
    │   │   │   └── time
    │   │   └── p
    │   │
    │   ├── section (Habilidades)
    │   │   ├── h2
    │   │   └── ul
    │   │       ├── li
    │   │       ├── li
    │   │       └── li
    │   │
    │   ├── section (Pasatiempos)
    │       ├── h2
    │       ├── article
    │       │   ├── h3
    │       │   └── p
    │       ├── article
    │       │   ├── h3
    │       │   └── p
    │       └── article
    │           ├── h3
    │           └── p
    │   
    └── footer
        ├── section
        │   ├── h4
        │   └── address
        │       ├── p
        │       │   └── a
        │       └── p
        │
        └── p
            └── small
                └── time
```