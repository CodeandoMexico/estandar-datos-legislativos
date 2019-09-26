Actor:
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

Revision:
  * creada (fecha)
  * aceptado (sí/no)
  * diff (hash)

Puesto:
  * nombre (del puesto)
  * comisión (a la que pertenece)

Link:
  * servicio (qué red social es)
  * url
  * actor (a la que pertenece)

Inasistencia:
  * actor (a la que pertenece)
  * total
  * sesiones
  * periodos (hash)


Votaciones:
  * actor (a la que pertenece)
  * total
  * a favor
  * en contra
  * abstención
  * ausente
  * periodos (hash)

Comisión:
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

Distrito:
  * tipo
  * entidad
  * secciones

Sección:
  * entidad
  * municipio
  * (id) marco geográfico nacional
  * sección
  * tipo
  * coordenadas

Teléfono:
  * número
  * extensión
