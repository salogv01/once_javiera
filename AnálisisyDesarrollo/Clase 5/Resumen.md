# Introduccion al Diseno. Clase 5

## 1. Pensar antes de dibujar

El diseno no es decorar, **es decidir**. Cada linea, color y boton comunica algo si no lo decidiste tu, lo decidio el azar.

### La analogia del arquitecto
Antes de poner un solo ladrillo, un arquitecto hace preguntas incomodas (cuantas personas, cuantos banos, presupuesto). Un error en los planos se multiplica por cada ladrillo mal puesto. El software funciona igual: un error de diseno se multiplica por cada pantalla mal construida.

### Los 5 niveles del diseno
| Nivel | Descripcion |
|---|---|
| **Sketch** | Garabato rapido, 30 segundos, para tirar ideas |
| **Wireframe** | Cajas y lineas con proporciones, sin color |
| **Mockup** | Colores, tipografia, imagenes pero no se mueve |
| **Prototipo** | Interactivo, se puede hacer clic, casi real |
| **Producto final** | Codigo real, lento y caro de hacer |

**La trampa mortal**: saltar directo al mockup (nivel 3) sin pasar por sketch y wireframe se gastan horas en algo que va a cambiar varias veces.

### Las 3 preguntas obligatorias
1. **¿Quien lo va a usar?** una persona concreta, no "todo el mundo"
2. **¿Que intenta lograr?** la unica cosa que vino a hacer
3. **¿Que se lo impide?** que le molesta, que le da miedo, que lo confunde

### Costo de no disenar
- Una app de delivery con el boton de confirmar mal ubicado perdio 3 de cada 5 usuarios
- Un banco puso "Transferir" y "Eliminar cuenta" uno al lado del otro 8% de usuarios elimino su cuenta por error
- Una funcion de busqueda quedo tan escondida que nadie la encontro en 6 meses

---

## 2. Boceto en papel

Antes de tocar un mouse, toca un lapiz. El papel es rapido, barato y se rompe sin consecuencias.

### Por que papel y no pantalla
- **Velocidad** un boceto en servilleta toma 30 segundos
- **Permiso para fallar** nadie siente culpa de romper un papel
- **Lenguaje universal** cualquiera puede opinar sobre un garabato

### Tres tipos de boceto
| Tipo | Tiempo | Uso |
|---|---|---|
| **Thumbnail** | <30 segundos | Explorar muchas ideas antes de elegir |
| **Rough sketch** | 5-10 minutos | Refinar la idea elegida, mostrar al equipo |
| **Polished wireframe** | Mas detallado | Entregar a desarrolladores o testear |

**Truco caja-marco**: dibujar primero el rectangulo del celular antes de cualquier elemento evita que el boceto se "salga" del espacio real.

---

## 3. Herramientas digitales

El papel no se jubila, solo se le suman herramientas y solo despues de validar en papel.

### Las 4 herramientas que importan
- **Excalidraw** bocetos digitales rapidos y arquitectura de sistemas, estilo dibujado a mano
- **FigJam / Figma** mockups profesionales y prototipos interactivos, estandar de la industria
- **Whimsical** diagramas de flujo, mapas mentales, wireframes rapidos
- **Papel** para thumbnails y exploracion, nunca se abandona

**Regla de oro**: usa la herramienta mas simple que resuelva el problema.

---

## 4. Arquitectura y modelado
Antes de disenar la pantalla, disena el sistema. Una app no es solo lo que el usuario ve:  hay datos, servicios y reglas detras.

### Que muestra la arquitectura
- Donde se guardan los datos
- Que hace la app internamente al tocar un boton
- Con que otros sistemas se comunica
- Que partes son seguras y cuales no

### Los 4 diagramas clave
| Diagrama | Para que sirve |
|---|---|
| **Cajas y flechas** | El mas simple, explica la app a cualquier persona |
| **Flujo de datos** | Muestra como viaja la informacion |
| **Diagrama de clases** | Detalla las "cosas" del sistema, mas tecnico |
| **Diagrama de secuencia** | Cuenta la historia paso a paso |

**Regla de los 30 segundos**: si un diagrama tarda mas de 30 segundos en entenderse, divide en varios diagramas mas simples.

---

## 5. Prototipado rapido

Un prototipo es una simulacion interactiva sin codigo real. Cuenta una historia: el usuario hace esto, ve esto otro, llega a un resultado.

### Para que sirve
- Probar con usuarios reales antes de codificar
- Comunicar la vision al equipo y al cliente
- Iterar rapido cambiar una pantalla toma minutos, no dias

### Lo-fi vs Hi-fi
| | Lo-fi | Hi-fi |
|---|---|---|
| **Hecho en** | Papel o wireframes | Colores, tipografia, imagenes reales |
| **Ventaja** | Rapido de cambiar, ideal para explorar | Se siente terminado, bueno para presentar |
| **Desventaja** | Menos creible para el cliente | Tarda mas en cambiarse |

**Regla de los 3 clics**: si el usuario no llega a su objetivo en maximo 3 clics, el diseno tiene pantallas de mas o informacion oculta.

---

## Cierre

### 3 ideas para llevarte
1. **Disenar es decidir** cada linea, color y boton comunica algo
2. **Empieza en papel** es mas rapido, mas honesto y permite fallar sin culpa
3. **Un buen prototipo cabe en 3 clics** si el usuario se pierde, el problema es el diseno

Disenar bien no es un talento innato, **es una disciplina que se entrena**. Cada vez que te detienes a preguntar quien, que intenta y que lo impide, te acercas mas a crear algo que la gente realmente quiera usar.

**Siguiente paso**: Clase 6 Prototipado avanzado (componentes interactivos, animaciones, pruebas con usuarios reales).