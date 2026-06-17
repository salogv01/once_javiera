# Documentacion de Requerimientos

## 1. Por que documentar?

La trampa mas comun del analista junior: pensar que tener la informacion "en la cabeza" es suficiente. Casi siempre termina en desastre.

| Mente | Papel |
|---|---|
| Se olvida en horas o dias | Permanece igual en el tiempo |
| Nadie mas accede a ella | Todo el equipo puede consultarla |
| Se pierde si te vas | Sobrevive a cambios de personal |
| Imposible auditar | Sirve de evidencia legal |

### Casos reales de no documentar
- **El programador estrella se va** sin documentacion, la empresa pago 45 millones para que un consultor entendiera el codigo.
- **"Eso no fue lo que dije"** sin acuerdo firmado, el cliente nego haber pedido algo y costo 6 meses extra.
- **La auditoria imposible** un banco no pudo probar cumplimiento legal y recibio una multa de 500 millones.

### Las 5 funciones de la documentacion
1. **Acuerdo** contrato entre cliente y equipo
2. **Guia** que construir, sin adivinar
3. **Verificacion** los testers prueban contra ella
4. **Conocimiento** memoria que sobrevive a las personas
5. **Legal** evidencia en disputas o auditorias

**Regla de oro**: a mas riesgo, mas documentacion (de historias en Trello hasta SRS completo con trazabilidad total).

---

## 2. El estandar IEEE 830

Estandar internacional del IEEE que define como escribir un **SRS** (Software Requirements Specification) — el documento maestro donde se escriben todos los requerimientos de un sistema.

### Beneficios vs criticas
| Beneficios | Criticas |
|---|---|
| Estructura clara y reconocida | Puede ser excesivo para proyectos pequenos |
| Facilita auditorias | Toma tiempo llenarlo |
| Cualquier programador lo entiende | Requiere disciplina mantenerlo |
| Mejora comunicacion con el cliente | No es agil por naturaleza |

### Estructura del SRS
1. Introduccion
2. Descripcion general
3. Requisitos especificos
4. Apendices

---

## 3. Casos de uso

Un caso de uso es una **descripcion narrativa paso a paso** de como un usuario interactua con el sistema para lograr un objetivo.

> Un requerimiento dice **que** pasa. Un caso de uso explica **como** pasa, paso a paso, incluyendo que ocurre si algo falla.

### Componentes
- **Actor** quien interactua (humano o sistema externo)
- **Sistema** el software que responde
- **Objetivo** lo que el actor quiere lograr
- **Escenario** la secuencia de pasos

### Diagrama UML
- Figura humana = actor
- Ovalos = casos de uso
- Rectangulo = limites del sistema
- Lineas = conexion actor-caso de uso

### Relaciones especiales
- **Include** un caso de uso siempre incluye otro (ej: "Reservar libro" incluye "Iniciar sesion")
- **Extend** comportamiento opcional bajo condicion (ej: "Pagar multa" extiende "Reservar libro")

---

## 4. Plantilla de caso de uso

Un caso de uso profesional tiene **12 secciones**:

| Seccion | Contenido |
|---|---|
| ID | Identificador unico (ej: CU-001) |
| Nombre | Verbo + objeto |
| Actores | Quien ejecuta el caso |
| Descripcion breve | Una frase con el objetivo |
| Precondiciones | Que debe ser cierto antes |
| Postcondiciones | Que debe ser cierto despues del exito |
| Flujo principal | Pasos del escenario ideal |
| Flujos alternos | Caminos validos distintos |
| Excepciones | Que pasa si algo falla |
| Reglas de negocio | Restricciones aplicables |
| Frecuencia de uso | Que tan seguido se ejecuta |
| Prioridad | Alta / Media / Baja |

### Errores comunes
- Confundir con un manual de usuario (describir botones e interfaz en vez de acciones)
- Mezclar pasos del actor con los del sistema
- Olvidar las excepciones, solo describir el caso feliz
- Ser demasiado abstracto o demasiado detallado

---

## 5. Revision cruzada

Otro analista lee tu documento buscando errores, ambiguedades o cosas faltantes. La primera defensa contra un mal SRS. Cuatro ojos ven mas que dos.

### Que buscar
- **Ambiguedades**  palabras vagas como "rapido" o "amigable"
- **Contradicciones**  requerimientos que chocan entre si
- **Faltantes**  casos no cubiertos
- **No medibles** RNF sin metrica clara
- **Dependencias**  requerimientos que dependen de otros sin decirlo
- **No atomicos**  dos ideas mezcladas en un requerimiento
- **Jerga tecnica innecesaria**  si el cliente no la entiende, hay que reescribir
- **Sin verificacion posible**  si no se puede probar, hay que reformular

### Proceso de revision
1. Leer con calma, idealmente en dos sesiones
2. Marcar con colores (rojo = critico, amarillo = duda, verde = OK)
3. Reunirse con el autor para conversar los hallazgos
4. Verificar correcciones despues de ajustar