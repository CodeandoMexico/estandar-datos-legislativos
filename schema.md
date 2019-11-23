# Actor
  ### (Diputado o Diputada) :
` Belongs to` **[Partido](#Partidos)**
` Belongs to` **[Legislatura](#Legislaturas)**
` Has many` **[Comisiones](#Comisiones)**
` Has and belongs to` **[Asistencias](#Asistencias)**  
` Has and belongs to` **[Iniciativas](#Iniciativas)**

  * cámara (a la que pertenece) [local, federal, senado]
  * nombre
  * apellido
  * slug (nombre y apellido transliterado para búsquedas)
  * distrito (`/^d[lf]-[1-3]{,1}\d-(\d{1,2}|rp|c[1-5])$/`)
  * entidad (número)
  * género (0, 1 -- masculino/femenino)
  * partido
  * correo
  * imagen
  * suplente
  * elección [mayoría relativa, primera minoría, representación proporcional]
  * curul
  * cabecera
  * teléfonos
  * links (redes sociales, páginas)
  * puestos (de comisiones)
  * inasistencias
  * votaciones
  * revisiones

# Legislaturas
` Has many ` **[Diputados](#Actor)**
` Has many ` **[Iniciativas](#Iniciativas)**
  * Nombre
  * No. de Legislatura
  * No en romano

# Periodos
` Belongs to ` **[Legislatura](#Legislaturas)**
  * Legislatura
  * Legislatura Id
  * Actual

# Periodos
` Belongs to ` **[Legislatura](#Legislaturas)**
 * Legislatura
 * Legislatura Id
 * Actual

# Partidos
` Has many ` **[Diputados](#Actor)**
` Belongs to ` **[Legislatura](#Legislaturas)**
` Has and Belongs to ` **[Iniciativas](#Iniciativa)**
 * Nombre
 * Logo
 * Estatus
 * URL Web
 * Orden
 * Estatus

# Asistencias
` Has and belongs to many ` **[Diputados](#Actor)**
` Has and belongs to many ` **[Asistencias Diputados](#Asistencias-diputados)**
` Belongs to ` **[Comision](#Comisiones)**
` Belongs to ` **[Legislatura](#Legislaturas)**
  * Fecha
  * Comision
  * Legislatura
  * Periodo

# Asistencias-diputados
` Belongs to ` **[Diputado](#Actor)**
` Belongs to ` **[Asistencia](#Asistencias)**
  * Diputado Id
  * Asistencia Id
  * Tipo de Asistencia

# Dictamenes
` Has many ` **[Iniciativas](#Iniciativas)**
` Has many ` **[Votaciones](#Votaciones)**
` Belongs to ` **[Legislatura](#Legislaturas)**
  * Titulo
  * Fecha de presentacion
  * Archivo
  * Numero de publicacion (Periodico oficial)

# Revision:
  * creada (fecha)
  * aceptado (sí/no)
  * diff (hash)

# Puesto:
  * nombre (del puesto)
  * comisión (a la que pertenece)

# Link:
  * servicio (qué red social es)
  * url
  * actor (a la que pertenece)

# Inasistencia: (Revisar)
  * actor (a la que pertenece)
  * total
  * sesiones
  * periodos (hash)

# Votaciones:
` Belongs to ` **[Diputado](#Actor)**
` Belongs to ` **[Dictamen](#Dictamenes)**
  * actor (a la que pertenece)
  * total
  * a favor
  * en contra
  * abstención
  * ausente
  * periodos (hash)

# Comisiones:
` Has many ` **[Diputados](#Actor)**
` Has many ` **[Asistencias](#Asistencias)**
  * cámara
  * nombre
  * oficina
  * link
  * entidad (para cámaras locales)
  * teléfonos
  * integrates (actores que pertenecen)
    * cuáles son de presidencia
    * cuáles son de secretaría
    * cuáles son sólo integrantes

# Distrito:
  * tipo
  * entidad
  * secciones

# Sección:
  * entidad
  * municipio
  * (id) marco geográfico nacional
  * sección
  * tipo
  * coordenadas


# Teléfono:
  * número
  * extensión


# Cabilderos:
  * rfc
  * razon_social
  * domicilio
  * telefono
  * correo_electronico
  * personas_autorizadas (tratar como array)
  * estatus_cabildero
  * anexo_buno (tratar como text)
  * anexo_bdos (tratar como text)
  * numero_acreditacion
  * persona_fisica
  * numero_cabildero
  * fecha_acreditacion
  * organos_gobierno_comisiones
  * diputadas_diputados
  * diputados (arreglo con los datos de los diputados correspondientes)
  * comisiones
  * nombre
  * colonia

# Decretos
    ` Belongs to` **[Dictamen](#Dictamenes)**
    ` Belongs to` **[Iniciativa](#Iniciativas)**
    ` Belongs to` **[Legislatura](#Legislaturas)**
    ` Has many` **[Archivos](#Archivos)**
    * titulo
    * archivo
    * archivo_de_publicacion
    * descripcion
    * fecha_publicacion
    * no_publicacion

# Detalle-orden
 ` Belongs to` **[Orden](#Ordenes)**
 ` Belongs to` **[Iniciativa](#Iniciativas)**
   * archivo
   * descripcion
   * numero_romano
   * colocacion(orden)

# Ordenes
  ### Ordenes del día
` Belongs to` **[Comision](#Comisiones)**
` Belongs to` **[Legislatura](#Legislaturas)**
  * fecha
  * ejercicio
  * archivo_pdf
  * tipo_de_orden (reunion, sesión solemne, diputación permanente, junta preparatoria, sesión extraordinaria)

# Listado de todas la Iniciativas:
  * id
  * fecha
  * descripcion
  * fondo
  * subfondo
  * seccion
  * clave
  * lugar
  * fecha_radicacion
  * iniciante
  * tipo_documento
  * asunto
  * comisiones
      * comision
          * nombre
# Ley:

  * id [ numerico ]
  * categoria_id [ numerico ]
  * created_at [ datetime ]
  * updated_at [ datetime ]
  * titulo [ cadena ]
  * descripcion [ cadena ]
  * tipo [ numerico ]
  * variable_id [ numerico ]
  * epub_url [ cadena ] || epub: { url: [ cadena ] }
  * word_url [ cadena ] || alt: word: { url: [ cadena ] }
  * pdf_url [ cadena ] || pdf: { url: [ cadena ] }
  * publicacion_url [ cadena ]  || publicacion: { url: [ cadena ] }
  * publicacion_info [ cadena ]  
  * orden [ numerico ]

# Código

  * id [ numerico ]
  * titulo [ cadena ]
  * descripcion [ cadena ]
  * pdf_url [ cadena ] || pdf: { url: [ cadena ] }
  * word_url [ cadena ] || word: { url: [ cadena ] }
  * publicacion_url [ cadena ] || publicacion: { url: [ cadena ] }
  * publicacion_info [ cadena ]

