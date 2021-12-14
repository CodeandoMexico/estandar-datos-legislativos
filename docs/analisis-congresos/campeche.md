# Congreso Campeche

https://www.congresocam.gob.mx/

## Legislativo

### Asistencias del pleno (ordinarias)

Listado de asistencias (PDF)
https://www.congresocam.gob.mx/asistencia/

Tienen los datos de asistencias, aunque no dice si es Pleno o Comisión, en un PDF.

Datos
- Diputado: Diputado
- Fecha: Date
- Asistencia: String | ASISTENCIA, PERMISO, FALTA, SALIO_CON_PERMISO, SALIO_SIN_PERMISO, LICENCIA

### Cabilderos

???

### Códigos

Listado de leyes (HTML)
No me queda muy claro si las leyes son parecidas a los codigos.
http://legislacion.congresocam.gob.mx/


### Comisiones

Lstado de comisiones (HTML)
https://www.congresocam.gob.mx/comisiones/

Datos
- Nombre: String
- Presidente: Diputado
- Secretario: Diputado
- Vocales: Array(Diputado) (1er, 2do, 3er)

### Decretos

Listado de Decretos (HTML)
https://www.congresocam.gob.mx/decretos/

Detalle del Decreto (PDF)

Datos
- Número: Number
- Legislatura: Legislatura
- Descripción: String
- Texto: String
- Documento Original: URL
- Fecha Publicación: Date

### Dictamen

Listado de Dictámenes (HTML)
https://www.congresocam.gob.mx/dictamenes/

Detall del Dictamen (PDF)

Datos
- No. expediente: String
- Legislatura: Legislatura
- Asunto: String
- Texto: RichText (markdown?)
- Representante: Diputado (el que presenta?)
- Promovente: String
- Comisión/es: Array(Comision)

### Diputados

Listado de diputados (HTML)
https://www.congresocam.gob.mx/legislatura-lxiv/

Detalle de un diputado (HTML)
https://www.congresocam.gob.mx/ubicatudiputado/diputado.php?dip=afrggcggcecb

Datos
- Nombre: String
- Apellido Paterno: String
- Apellido Materno: String
- Fotografía: URL
- Distrito Electoral: DistritoElectoral
- Municipio: Municipio
- Reoresentación: TipoRepresentacion | MAYORIA_RELATIVA,
- Partido: PartidoPolitico
- Teléfono: String
- Correo Electrónico: String
- CV: ?
- Enlaces externos: Array(URL) p.ej: redes sociales

  - Comisiones: Array(Comision)
  - Iniciativas: Array(Iniciativa)
  - Asistencias Sesiones (pleno)
  - Asistencias Comisiones
  - Informes de actividades
  - Informes de viajes
  - Informes de comisiones

### Distritos Electorales

https://es.wikipedia.org/wiki/Distritos_electorales_federales_de_M%C3%A9xico#Campeche

Datos:
- Código de Municipio: 001: Ensenada, 002: Mexicali, 003: Tecate, 004: Tijuana, 005: Playas de Rosarito
- Número de Distrito

### Iniciativas

Listado de Iniciativas (HTML), el detalle (PDF)
https://www.congresocam.gob.mx/iniciativas/

Datos
???

### Legislaturas (histórico)

Algunas secciones (actas, ) se pueden buscar por legislatura, pero no hay un archivo de toda una lgislatura.

### Listado de leyes

Lista de Leyes
http://legislacion.congresocam.gob.mx/

Datos
- Nombre: String
- Tipo: String | ESTATALES, FEDERALES


### Ordenes

???

### Partidos, Grupos Parlamentarios, Fracciones

Coordinadores y representantes de partido
https://www.congresocam.gob.mx/coordinadores-y-representantes/

### Periodos

Esta información está repartida en otras páginas. p.ej: mesa directiva por periodo, en las actas de comisiones, etc.


### Puestos

Junta de Gobierno
https://www.congresocam.gob.mx/estructura-junta-gobierno-integracion/

Mesa directiva (PDF)
https://www.congresocam.gob.mx/estructura-mesadirectiva-integracion/

Secretario general
https://www.congresocam.gob.mx/secretaria-general/

Organo Interno de Control
https://www.congresocam.gob.mx/organo-interno-de-control/


### Revisiones

???

## Secciones

???

## Directorio del Congreso

https://www.congresocam.gob.mx/directorio/

Datos
- Nombre
- Direccion: Direccion
- Teléfonos: Array(Teléfono, Ext)
- Email: String (Email)

## Votaciones

???