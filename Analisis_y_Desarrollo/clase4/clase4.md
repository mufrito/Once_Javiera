#  Clase 4: Documentación de Requerimientos

##  Objetivo

Aprender a documentar requerimientos de forma profesional utilizando:

- Casos de uso.
- Estándar IEEE 830.
- Documento SRS (Software Requirements Specification).
- Revisión cruzada.

---

# 1. ¿Por qué documentar?

La documentación permite convertir el conocimiento del analista en información permanente, compartida y verificable.

## Beneficios

-  Sirve como acuerdo entre cliente y equipo.
-  Guía a los desarrolladores.
-  Permite verificar que el sistema cumple lo solicitado.
-  Conserva el conocimiento del proyecto.
-  Funciona como evidencia legal y de auditoría.

## Riesgos de no documentar

- Pérdida de información.
- Dependencia de una sola persona.
- Malentendidos con el cliente.
- Problemas durante auditorías.
- Incremento de costos de mantenimiento.

## Regla general

> A mayor riesgo e impacto del proyecto, mayor documentación se necesita.

---

# 2. Estándar IEEE 830

## ¿Qué es?

Es un estándar internacional para elaborar documentos de especificación de requerimientos de software (**SRS**).

**SRS = Software Requirements Specification**

Su objetivo es que cualquier profesional pueda entender claramente los requerimientos del sistema.

## Beneficios

- Estructura organizada.
- Comunicación uniforme.
- Facilita auditorías.
- Reduce errores y omisiones.

## Estructura principal del SRS

### 1. Introducción
- Propósito.
- Alcance.
- Definiciones.
- Referencias.
- Visión general.

### 2. Descripción General
- Perspectiva del producto.
- Funciones principales.
- Características de usuarios.
- Restricciones.
- Dependencias.

### 3. Requisitos Específicos
- Requerimientos funcionales.
- Requerimientos no funcionales.
- Interfaces externas.
- Casos de uso.

### 4. Apéndices
- Diagramas.
- Glosarios.
- Trazabilidad.
- Documentación adicional.

## Características de un buen SRS

1. Correcto.
2. No ambiguo.
3. Completo.
4. Consistente.
5. Priorizado.
6. Verificable.
7. Modificable.
8. Trazable.

---

# 3. Casos de Uso

## Definición

Un caso de uso describe paso a paso cómo un usuario interactúa con el sistema para alcanzar un objetivo.

## Diferencia entre requerimiento y caso de uso

### Requerimiento

Describe **qué** debe hacer el sistema.

Ejemplo:

> El sistema deberá permitir reservar libros.

### Caso de Uso

Describe **cómo** ocurre el proceso.

Ejemplo:

1. Usuario inicia sesión.
2. Busca un libro.
3. Selecciona el libro.
4. Confirma la reserva.
5. El sistema registra la reserva.

## Componentes

###  Actor
Persona o sistema que interactúa con el software.

###  Sistema
Aplicación que responde a las acciones del actor.

###  Objetivo
Meta que busca alcanzar el actor.

###  Escenario
Secuencia de pasos para lograr el objetivo.

## Relaciones UML

### <<include>>

Un caso de uso siempre necesita otro.

Ejemplo:

```
Reservar libro
    <<include>>
Iniciar sesión
```

### <<extend>>

Agrega comportamiento opcional.

Ejemplo:

```
Pagar multa
    <<extend>>
Reservar libro
```

---

# 4. Plantilla Profesional de Caso de Uso

## Estructura

###  ID
Identificador único.

Ejemplo:

```
CU-001
```

###  Nombre

Verbo + objeto.

Ejemplo:

```
Reservar libro
```

###  Actor principal

Usuario principal que ejecuta el proceso.

###  Descripción

Resumen breve del objetivo.

###  Precondiciones

Condiciones necesarias antes de iniciar.

###  Postcondiciones

Resultado esperado al finalizar.

###  Flujo principal

Pasos del escenario exitoso.

###  Flujos alternos

Variaciones válidas del flujo principal.

###  Excepciones

Situaciones de error.

###  Reglas de negocio

Restricciones aplicables.

###  Frecuencia

Cantidad estimada de uso.

###  Prioridad

- Alta
- Media
- Baja

## Buenas prácticas

- Separar acciones del actor y del sistema.
- Incluir excepciones.
- Mantener detalle intermedio.
- Usar verbos claros.

---

# 5. Construcción de Casos de Uso

Un caso de uso completo debe incluir:

- Objetivo.
- Actor.
- Precondiciones.
- Postcondiciones.
- Flujo principal.
- Excepciones.
- Reglas de negocio.

## Recomendaciones

- Cada paso debe iniciar con un verbo.
- Diferenciar claramente actor y sistema.
- Si tiene más de 15 pasos, considerar dividirlo.
- Pensar siempre en:

> ¿Qué pasa si algo falla?

---

# 6. Plantilla SRS IEEE 830

## Sección 1: Introducción

Incluye:

- Propósito.
- Alcance.
- Definiciones.
- Referencias.
- Visión general.

---

## Sección 2: Descripción General

Incluye:

### Perspectiva del producto

Relación con otros sistemas.

### Funciones principales

Capacidades generales.

### Características de usuarios

Tipos de usuarios y nivel técnico.

### Restricciones

Ejemplos:

- Presupuesto.
- Tiempo.
- Tecnología.

### Dependencias

Factores externos necesarios.

---

## Sección 3: Requisitos Específicos

### Requerimientos Funcionales (RF)

Definen funciones del sistema.

Ejemplos:

```text
RF-001 Buscar libros.
RF-002 Reservar libros.
RF-003 Registrar préstamos.
```

### Requerimientos No Funcionales (RNF)

Definen calidad y restricciones.

Ejemplos:

```text
RNF-001 Tiempo de respuesta menor a 2 segundos.
RNF-002 Disponibilidad del 99%.
RNF-003 Contraseñas cifradas.
```

### Interfaces Externas

Integraciones con otros sistemas.

Ejemplos:

- API REST.
- SMTP.
- Aplicaciones móviles.

---

## Sección 4: Apéndices

Incluye:

- Casos de uso.
- Diagramas UML.
- Bocetos.
- Glosario.
- Matriz de trazabilidad.

---

## Importancia de los IDs

Ejemplos:

```text
RF-001
RNF-002
CU-003
```

Permiten:

- Referenciar elementos.
- Mantener trazabilidad.
- Facilitar pruebas.
- Organizar documentación.

---

# 7. Revisión Cruzada

## Definición

Proceso donde otra persona revisa el documento para encontrar errores o mejoras.

## Aspectos a revisar

###  Ambigüedades

Palabras como:

- rápido
- fácil
- moderno
- amigable

###  Contradicciones

Requerimientos que se contradicen.

###  Faltantes

Casos no contemplados.

###  Falta de métricas

Requisitos imposibles de medir.

###  Dependencias ocultas

Requerimientos relacionados no documentados.

###  No atómicos

Más de una idea en un mismo requerimiento.

###  Jerga técnica innecesaria

Lenguaje difícil para el cliente.

###  Sin posibilidad de verificación

No se puede probar objetivamente.

---

## Proceso recomendado

### 1. Leer cuidadosamente

Sin prisa.

### 2. Marcar hallazgos

- 🔴 Error crítico.
- 🟡 Duda.
- 🟢 Correcto.

### 3. Reunirse con el autor

Discutir hallazgos.

### 4. Verificar correcciones

Realizar una segunda revisión.

---

#  Conclusión

La documentación profesional transforma los requerimientos descubiertos durante el análisis en documentos claros, verificables y mantenibles.

Al finalizar la clase se domina:

-  Estándar IEEE 830.
-  Elaboración de documentos SRS.
-  Casos de uso y UML.
-  Revisión cruzada.
-  Trazabilidad de requerimientos.

## Idea clave

> Documentar bien significa garantizar que cualquier persona pueda entender, desarrollar, probar y mantener el sistema incluso años después de haber sido diseñado.