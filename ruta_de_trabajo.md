# Aterrizando la ruta de trabajo

- Terminemos el [schema.md](https://github.com/CodeandoMexico/representantes-patito-2/blob/master/schema.md)
- Empecemos el frontend

## Cómo finalizar el schema.md

**Definición:** 
El schema es el documento que detalla la estructura de las tablas en una base de datos y el formato de los datos que rellenarán esas tablas, así como las relaciones entre las mismas (Ej: Una bancada tiene a muchos diputados y un diputado pertenece a una bancada). Terminar el schema significa que terminaremos una propuesta de un estándar de datos, y le permitirá a los desarrolladores que hacen el API a diseñarla.

**Contexto de esta tarea:**
En [schema.md](https://github.com/CodeandoMexico/representantes-patito-2/blob/master/schema.md) se encuentra la propuesta inicial de Representantes Patito para modelar los datos. El Congreso del estado de Guanajuato tiene una propuesta más avanzada de software que maneja la actividad legislativa. Tenemos una lista de endpoints (ligas de consulta de la base de datos) que tiran la estructura pública de la base de datos en formato JSON. Podemos nutrir la propuesta original de schema con los datos del API de Congreso de Guanajuato.

**¿Cómo estructuramos esta tarea?:**

**Objetivo:** Actualizar el [schema.md](https://github.com/CodeandoMexico/representantes-patito-2/blob/master/schema.md) con las tablas de GTO

1. Tarea: Validar con GTO qué tablas faltan
2. Tarea: Llenar en Github cada tarea de validar las tablas de GTO y sus campos con el schema (una tarea por tabla)
3. Propuesta: Proponer una fecha y una dinámica de definición de tablas externa para que otros puedan participar - **pospuesto**
4. Propuesta: Proponer una fecha y dinámica de definición de tablas interna (al interior de la comunidad de Codeando) para que otros puedan participar


### Endpoints GTO



- Listado de Leyes:
`GET http://www.congresogto.gob.mx/leyes.json`

- Listdo de Códigos:
`GET http://www.congresogto.gob.mx/codigos.json`

- Listado de Reglamentos:
`GET http://www.congresogto.gob.mx/reglamentos.json`

- Listado de Iniciativas a Consulta:
`GET http://www.congresogto.gob.mx/iniciativas/a_consulta.json`

- Listado de Iniciativas No Dictaminadas:
`GET http://www.congresogto.gob.mx/iniciativas/no_dictaminadas.json`

- Listado de Dictamenes en Pleno:
`GET http://www.congresogto.gob.mx/dictamenes/dictamenes_api.json`

- Listado de todas la Iniciativas:
`GET http://www.congresogto.gob.mx/iniciativas/iniciativas_api.json`

- Listado de Ordenes:
`GET http://www.congresogto.gob.mx/ordenes/ordenes_api.json`

- Detalle de la Orden/Reunion:
`GET http://www.congresogto.gob.mx/ordenes/780/orden_api.json`

- Listado de Dictamenes en comisiones:
`GET http://www.congresogto.gob.mx/dictamenes_comisiones/dictamenes_comisiones_api.json`

- Listado de Decretos:
`GET https://www.congresogto.gob.mx/decretos.json`

- Listado de Comisiones de la Legislatura Actual:
`GET https://www.congresogto.gob.mx/comisiones/comisiones_api.json`

- Cabilderos Personas Fisicas:
`GET http://www.congresogto.gob.mx/cabildero_fisicas/personas_fisicas_api.json`

- Cabilderos Personas Morales:
`GET http://www.congresogto.gob.mx/cabildero_morales/personas_morales_api.json`



## Frontend

**Contexto:**  
Como está descrito en el README, uno de los productos que salen de este proyecto es una forma de visualizar los datos. A esta parte le llamamos __Front-end__ es una página web que consume el API y despliega los datos de forma intuitiva.

**Problema:**
El fin de este proyecto es acercar el trabajo legislativo a la sociedad, por tanto, es crucial crear herramientas amigables que ayuden a buscar fácilmente la información requerida.
El Front-end debe cumplir con ser:
- Intuitivo (user-experience)
- Consistente (componentizable)
- Accesible (toma en cuenta las necesidades especiales del usuario)


- **Tarea:** Definir una dinámica para hacer un sprint de diseño de donde salgan todas las historias de usuario para esta aplicación.

## Preguntas en general

#### Contexto

En esta sección formularemos las preguntas e inquietudes generales en relación al proyecto; desde una perspectiva sobre los detalles de información legislativa a obtener y desplegar, hasta detalles técnicos sobre la estructura del proyecto y su desarrollo.

#### Q&A:

- **¿Los campos especificados a través del los endpoints del congreso de Gto. son suficientes?**
  No. Puede ser un primer saque pero necesitamos validaciones de otros estados y/o federal.
  
- **¿Quién será el usuario final de la aplicación?**
  X.
