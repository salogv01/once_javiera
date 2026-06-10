# Resumen: Requerimientos, Calidad de Software e Historias de Usuario

## ¿Qué es un requerimiento?

Un requerimiento es una propiedad o característica que un sistema debe poseer para resolver un problema o alcanzar un objetivo. Según el estándar IEEE 830, un requerimiento debe estar documentado y ser verificable. Esto significa que debe poder escribirse claramente y comprobarse posteriormente si se cumple o no.

Los requerimientos pueden provenir de diversas fuentes, como los usuarios finales, los clientes o patrocinadores, las leyes y regulaciones aplicables, y otros sistemas con los que se debe integrar la solución.

Para que un requerimiento sea considerado de calidad, debe cumplir varias características: ser necesario, no ambiguo, verificable, consistente, completo, atómico y trazable.

---

## Requerimientos Funcionales

Los requerimientos funcionales describen qué debe hacer el sistema. Representan las acciones, tareas, procesos o servicios que la aplicación debe ofrecer a sus usuarios.

Generalmente se identifican mediante verbos de acción como registrar, mostrar, calcular, validar, modificar, generar o enviar. También suelen describir entradas, salidas, decisiones y acciones asociadas a diferentes roles del sistema.

Una estructura común para redactarlos es:

> El sistema deberá + acción + objeto + condiciones.

Los requerimientos funcionales pueden clasificarse en distintas categorías, entre ellas autenticación, cálculos, persistencia de datos, comunicación, generación de reportes y validación de información.

---

## Requerimientos No Funcionales

Los requerimientos no funcionales describen cómo debe comportarse el sistema. A diferencia de los requerimientos funcionales, no se enfocan en las tareas que realiza el software, sino en la calidad con la que dichas tareas deben ejecutarse.

Un sistema puede cumplir perfectamente sus funciones y aun así fracasar si presenta problemas de rendimiento, seguridad o usabilidad. Por ello, los requerimientos no funcionales son fundamentales para el éxito de una aplicación.

Las principales categorías de requerimientos no funcionales son:

- Rendimiento.
- Seguridad.
- Usabilidad.
- Confiabilidad.
- Escalabilidad.
- Mantenibilidad.
- Compatibilidad y portabilidad.
- Cumplimiento legal y normativo.

Una regla fundamental es que todo requerimiento no funcional debe ser medible. Expresiones como "el sistema debe ser rápido" o "el sistema debe ser seguro" son demasiado ambiguas. En cambio, deben especificarse métricas concretas, umbrales aceptables y formas de verificación.

También es importante comprender que algunos requerimientos no funcionales pueden entrar en conflicto entre sí. Por ejemplo, aumentar la seguridad suele reducir la facilidad de uso, mientras que incrementar la escalabilidad normalmente implica mayores costos de infraestructura.

---

## Atributos de Calidad del Software

Los atributos de calidad son características generales que permiten evaluar qué tan bueno es un software. Constituyen conceptos abstractos que posteriormente se convierten en requerimientos no funcionales concretos y medibles.

La norma internacional ISO/IEC 25010 define ocho atributos principales de calidad:

### Adecuación funcional

Evalúa si el sistema realiza correctamente las funciones para las cuales fue diseñado.

### Eficiencia de desempeño

Mide la velocidad de respuesta y el uso eficiente de recursos como memoria, procesamiento y almacenamiento.

### Compatibilidad

Determina la capacidad del sistema para coexistir e intercambiar información con otros sistemas.

### Usabilidad

Evalúa la facilidad con la que los usuarios pueden aprender, comprender y utilizar la aplicación.

### Confiabilidad

Mide la capacidad del sistema para funcionar de manera estable y consistente sin fallos frecuentes.

### Seguridad

Analiza la protección de la información y de los usuarios frente a accesos no autorizados o amenazas.

### Mantenibilidad

Se refiere a la facilidad para corregir errores, realizar mejoras o incorporar nuevas funcionalidades.

### Portabilidad

Evalúa la capacidad del software para ejecutarse en distintos entornos, dispositivos o plataformas.


---

## Historias de Usuario

Las historias de usuario son una técnica utilizada en metodologías ágiles para expresar requerimientos desde la perspectiva de quien utilizará el sistema. Su objetivo es centrarse en el valor que recibe el usuario más que en los detalles técnicos.

Su estructura básica es:

> Como [tipo de usuario], quiero [funcionalidad], para [beneficio].

Las historias de usuario no sustituyen los requerimientos funcionales formales, sino que ofrecen una manera más sencilla y cercana de capturar necesidades.

---

## Principio INVEST

Una buena historia de usuario debe cumplir los criterios INVEST:

- **Independent (Independiente):** puede desarrollarse sin depender de otras historias.
- **Negotiable (Negociable):** puede discutirse y ajustarse durante el proyecto.
- **Valuable (Valiosa):** aporta valor real al usuario.
- **Estimable (Estimable):** permite calcular esfuerzo y tiempo de desarrollo.
- **Small (Pequeña):** puede completarse dentro de un sprint corto.
- **Testable (Testeable):** puede verificarse objetivamente.

---

## Criterios de Aceptación

Los criterios de aceptación definen las condiciones necesarias para considerar una historia de usuario como completada. Permiten validar que el sistema cumple exactamente con las expectativas planteadas.

Normalmente se redactan utilizando la estructura:

**Dado** una condición inicial,  
**Cuando** ocurre una acción,  
**Entonces** debe producirse un resultado esperado.

Por ejemplo:

- Dado que el estudiante está autenticado.
- Cuando abre la aplicación.
- Entonces puede visualizar el menú del día.

Los criterios de aceptación transforman una necesidad general en comportamientos concretos que pueden probarse y validarse durante el desarrollo.

