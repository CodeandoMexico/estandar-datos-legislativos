# Congreso Baja California

https://www.congresobc.gob.mx/

## Legislativo

### Asistencias del pleno (ordinarias)

Listado de sesiones (HTML)
https://www.congresobc.gob.mx/Contenido/Actividades_Legislativas/Actas_Sesion/Actas.aspx

En el listado de sesiones hay una columna con enlace a un PDF con la lista de asistencia (PDF)
https://www.congresobc.gob.mx/Documentos/Parlamentarias/ListaDeAsistencia/Lista_Asistencia_1152.pdf

En el Acta de Sesión viene la lista de asistencia (PDF)
Ejemplo: https://www.congresobc.gob.mx/Documentos/Parlamentarias/Acta/20211105ae.pdf

Datos
- Diputado: Diputado
- Asistencia: String | PRESENTE, JUSTIFICADO

### Cabilderos

???

## Códigos

Listado de Códigos (HTML)
https://www.congresobc.gob.mx/Contenido/Actividades_Legislativas/Leyes_Codigos.aspx

Datos
- Nombre: String
- Documento Original: URL
- Fecha: Date
- Estatus: String | VIGENTE
- Tomo: String

## Comisiones

El listado de comisiones está en el menú (HTML)

Detalle de Comisión (HTML)
https://www.congresobc.gob.mx/Contenido/Comisiones/index.aspx?com=15

Datos
- Nombre: String
- Presidente: Diputado
- Secretario: Diputado
- Vocales: Array(Diputado)

## Decretos

Listado de Decretos (HTML)

https://www.congresobc.gob.mx/Contenido/Actividades_Legislativas/Decretos.aspx

Detalle del Decreto (PDF escaneado)

En el listado de decretos hay algunos datos del decreto y se puede descargar un PDF que contiene el documento completo decreto.

Datos
- Número: Number
- Descripción: String
- Documento Original: URL
- Presentación Pleno: Date
- Recepción Ejecutivo: Date
- Fecha Publicación: Date
- Comisión: Comision
- Dictamen: Dictamen

## Dictamen

Listado de Dictámenes (HTML)
https://www.congresobc.gob.mx/Contenido/Actividades_Legislativas/Dictamenes.aspx

Detall del Dictamen (PDF escaneado)

En el listado de decretos se puede descargar un PDF escaneado que contiene el documento del dictamen asociado al decreto.

## Diputados

Listado de diputados (HTML)
https://www.congresobc.gob.mx/Contenido/Legislatura/Diputados/index.aspx

Detalle de un diputado (HTML)
https://www.congresobc.gob.mx/Contenido/Legislatura/Diputados/Perfil_Diputado.aspx?dip=92

Datos
- Nombre: String
- Apellido Paterno: String
- Apellido Materno: String
- Fotografía: URL
- Distrito Electoral: DistritoElectoral
- Teléfono: String
- Correo Electrónico: String
- CV: ?
- Enlaces externos: Array(URL) p.ej: redes sociales
- Comisiones: Array(Comision)

## Distritos

No pude encontrarlos en la web.

Listado de Distritos (HTML)
https://es.wikipedia.org/wiki/Distritos_Electorales_Estatales_de_Baja_California

Datos:
- Código de Municipio: 001: Ensenada, 002: Mexicali, 003: Tecate, 004: Tijuana, 005: Playas de Rosarito
- Número de Distrito

## Iniciativas

Listado de Iniciativas (HTML)
https://www.congresobc.gob.mx/Contenido/Actividades_Legislativas/Iniciativas.aspx

Detalle de Iniciativa (PDF escaneado)
Ej: https://www.congresobc.gob.mx/Documentos/ProcesoParlamentario/Iniciativas/20211130_INFORME_MOLINA.PDF

Datos
- Tipo: String | ACUERDO, INFORME, INIACTIVA DE REFORMA, INICIATIVA DE ADICIÓN, INICIATIVA DE LEY, POSICIONAMIENTO, DECLARATORIA
- No. Documento: String
- Fecha: Date
- Título: String
- Contenido de la iniciativa: String
- Enlace a documento original: URL
- Legislatura: Legislatura
- Comisión: Comision
- Sesión: Sesion
- Grupo parlamentario: GrupoParlamentario

## Legislaturas (histórico)

No pude encontrar la información. Sin embargo cuando buscar inciativas, sesiones, etc, puedes hacer busquedas en el tiempo, y aparece la legislatura asociada a una iniciativa.

Datos
- Numero: Number
- Numero Romano: String
- Fecha Inicio: Date
- Fecha Fin: Date

## Listado de leyes

Lista de Leyes (HTML)
https://www.congresobc.gob.mx/Contenido/Actividades_Legislativas/Leyes_Codigos.aspx

Datos:
- Nombre: String
- Enlace al documento original: URL
- Fecha: Date
- Estatus: String | VIGENTE
- Tomo: String | ej. TOMO_VII

## Ordenes

???

## Partidos, Grupos Parlamentarios, Fracciones

Lista de Partidos (HTML)
https://www.congresobc.gob.mx/Contenido/Legislatura/Partidos/index.aspx

Lista de Diputados de un Grupo Parlamentario (HTML)
Ej: https://www.congresobc.gob.mx/Contenido/Legislatura/Diputados/index.aspx?partido=PES

Datos
- Partido: Partido
- Diputados: Array(Diputado)
- Coordinador: Diputado

## Periodos

???

## Puestos

Mesa Directiva (HTML)
https://www.congresobc.gob.mx/Contenido/Legislatura/Mesa_Directiva/index.aspx

En cada comisión aparecen los puestos (HTML)
https://www.congresobc.gob.mx/Contenido/Comisiones/index.aspx?com=15

## Revisiones

???

## Secciones

???

## Directorio del Congreso

Directorio (HTML)
https://www.congresobc.gob.mx/Contenido/Informacion/Directorio/index.aspx?opcion=1

## Votaciones

???
