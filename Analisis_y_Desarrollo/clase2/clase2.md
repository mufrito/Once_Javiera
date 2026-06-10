#  Resumen de Aprendizajes: Ingeniería de Requerimientos (Nivel 2)

## 1. Concepto Profesional de Requerimiento

### Definición

Un requerimiento es una propiedad **documentada y verificable** que un sistema debe cumplir para resolver un problema o alcanzar un objetivo.

### Aprendizajes Clave

- Los requerimientos surgen de necesidades de usuarios, clientes, leyes, normas y sistemas externos.
- El trabajo del analista consiste en transformar necesidades informales en especificaciones claras, medibles y verificables.
- Todo requerimiento debe poder documentarse y comprobarse.

### Características de un Buen Requerimiento

-  Necesario
-  No ambiguo
-  Verificable
-  Consistente
-  Completo
-  Atómico (una sola idea)
-  Trazable

---

## 2. Requerimientos Funcionales (RF)

### Definición

Los requerimientos funcionales describen **qué hace el sistema**.

### Cómo Identificarlos

- Contienen verbos de acción.
- Describen entradas, procesos y salidas.
- Definen reglas de negocio o decisiones.
- Especifican acciones para distintos roles de usuario.

### Categorías Comunes

| Categoría | Ejemplos |
|------------|------------|
| Autenticación | Inicio de sesión, registro, recuperación de contraseña |
| Cálculos | Promedios, estadísticas, operaciones matemáticas |
| Persistencia | Crear, leer, actualizar y eliminar datos (CRUD) |
| Comunicación | Correos, SMS, notificaciones |
| Reportes | Exportación de información |
| Validaciones | Restricciones y reglas de negocio |

### Buenas Prácticas

- Utilizar una estructura uniforme.
- Expresar una sola funcionalidad por requerimiento.
- Ser claros, específicos y verificables.

---

## 3. Requerimientos No Funcionales (RNF)

### Definición

Los requerimientos no funcionales describen **cómo debe comportarse el sistema** y qué nivel de calidad debe alcanzar.

### Categorías Principales

-  Rendimiento
-  Seguridad
-  Usabilidad
-  Confiabilidad
-  Escalabilidad
-  Mantenibilidad
-  Compatibilidad y Portabilidad
-  Cumplimiento Legal

### Aprendizajes Clave

- Todo RNF debe ser medible.
- Debe incluir métricas y umbrales específicos.
- Debe existir una forma objetiva de verificar su cumplimiento.
- Los RNF impactan directamente la calidad y aceptación del sistema.

### Trade-offs Comunes

| Atributo 1 | Atributo 2 |
|------------|------------|
| Seguridad | Usabilidad |
| Rendimiento | Mantenibilidad |
| Escalabilidad | Costos |

> Mejorar un atributo puede afectar negativamente otro, por lo que es necesario encontrar un equilibrio.

---

## 4. Atributos de Calidad (ISO/IEC 25010)

### Definición

Los atributos de calidad representan las características generales que determinan qué tan bueno es un software.

### Los 8 Atributos Principales

1.  Adecuación funcional
2.  Eficiencia de desempeño
3.  Compatibilidad
4.  Usabilidad
5.  Confiabilidad
6.  Seguridad
7.  Mantenibilidad
8.  Portabilidad

### Relación entre Atributos y RNF

| Atributo de Calidad | RNF |
|---------------------|-----|
| Concepto general | Aplicación específica y medible |
| Ejemplo: Seguridad | Ejemplo: Bloquear acceso tras 5 intentos fallidos |

---

## 5. Análisis de Necesidades

### Stakeholders

Son todas las personas o entidades interesadas en el sistema.

### Ejemplos de Stakeholders

- Usuarios finales
- Clientes
- Administradores
- Organismos reguladores

### Técnicas de Elicitación

-  Entrevistas
-  Encuestas
-  Observación
-  Talleres
-  Prototipos
-  Revisión documental

### Aprendizajes Principales

- Cada stakeholder aporta necesidades distintas.
- Las técnicas deben seleccionarse según el contexto.
- El objetivo es convertir necesidades informales en requerimientos claros y verificables.

---

## 6. Historias de Usuario

### Definición

Las historias de usuario son descripciones breves de funcionalidades desde la perspectiva del usuario.

### Formato Estándar

```text
Como [usuario],
quiero [funcionalidad],
para [beneficio].
````

### Beneficios

* Centran el desarrollo en el valor para el usuario.
* Facilitan la comunicación entre clientes y desarrolladores.
* Son ampliamente utilizadas en metodologías ágiles.

---

## 7. Modelo INVEST

Una buena historia de usuario debe cumplir con INVEST:

| Letra | Significado                 |
| ----- | --------------------------- |
| **I** | Independent (Independiente) |
| **N** | Negotiable (Negociable)     |
| **V** | Valuable (Valiosa)          |
| **E** | Estimable (Estimable)       |
| **S** | Small (Pequeña)             |
| **T** | Testable (Testeable)        |

### Aprendizaje Clave

Una historia de usuario debe aportar valor, ser pequeña, comprobable y suficientemente clara para estimar su implementación.

---

## 8. Criterios de Aceptación

### Propósito

Definen cuándo una historia de usuario puede considerarse completada.

### Formato Recomendado

```text
Dado una condición inicial,
Cuando ocurre una acción,
Entonces debe producirse un resultado esperado.
```

### Importancia

* Permiten validar el cumplimiento de los requerimientos.
* Reducen ambigüedades.
* Facilitan las pruebas.
* Sirven como base para la aceptación del producto.

---

#  Conclusiones Generales

* Los requerimientos son el puente entre las necesidades del usuario y la implementación del software.
* Los RF describen **qué hace** el sistema.
* Los RNF describen **cómo debe comportarse** el sistema.
* La calidad del software depende en gran medida de los RNF y de los atributos de calidad.
* La identificación correcta de stakeholders es fundamental para descubrir necesidades reales.
* Las técnicas de elicitación permiten obtener información de manera efectiva.
* Las historias de usuario facilitan la comunicación y el desarrollo ágil.
* Los criterios de aceptación garantizan que los requerimientos puedan verificarse objetivamente.
* Un analista profesional debe ser capaz de capturar, documentar, clasificar y validar requerimientos de forma clara, medible y trazable.

---

##  Resumen Rápido

| Concepto                | Idea Principal                         |
| ----------------------- | -------------------------------------- |
| Requerimiento           | Debe ser documentado y verificable     |
| RF                      | Describe qué hace el sistema           |
| RNF                     | Describe cómo debe comportarse         |
| ISO 25010               | Define los atributos de calidad        |
| Stakeholders            | Personas interesadas en el sistema     |
| Elicitación             | Técnicas para descubrir requerimientos |
| Historia de Usuario     | Como..., quiero..., para...            |
| INVEST                  | Criterios para una buena historia      |
| Criterios de Aceptación | Dado..., Cuando..., Entonces...        |

```
```
