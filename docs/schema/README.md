# Schema

El `schema` es un conjunto de archivos que especifican la estructura de los datos dentro del **Estándar de Datos Abiertos Legislativos**. Para asegurar la calidad y usabilidad del estándar se ha utilizado el framework de [Frictionless Data](https://frictionlessdata.io/standards/#standards-toolkit), un conjunto de especificaciones creadas para estandarizar diferentes aspectos del trabajo con datos (vocabulario compartido, intercambio de datos y orientación).

La base de este esquema es:

- [Table Schema](https://specs.frictionlessdata.io/table-schema/) - Un formato simple para declarar un esquema para datos tabulares. El esquema está diseñado para expresarse en JSON.
- [Data Package](https://specs.frictionlessdata.io/data-package/) - Un formato de contenedor simple para describir una colección coherente de datos en un solo paquete.

## Estructura

**Paquete de datos**, el archivo `schema.json` contiene en su totalidad la descripción de todos los conjuntos de datos, así como los metadatos del estándar. Contiene lo siguiente:

- Nombre y descripción
- Esquemas
- Relaciones
- Versión
- Formatos
- Contribuidores
- Licencia

**Esquemas indivudales**, los archivos como `legislador.json` o `asiento.json` son las especificaciones independientes de cada entidad (concepto) dentro del estándar. Contienen lo siguiente:

- Descriptores para cada campo
    - Nombre
    - Título
    - Descripción
    - Ejemplo
    - Tipo de dato
    - Formato
    - Reestricciones
- Otras propiedades
    - Valores faltantes
    - Llave primaria
    - Llaves foráneas

## Herramientas

Ya que el estándar está basado en _Frictionless Data_, se puede hacer uso de las siguientes herramientas:

1. **Validador para conjuntos de datos tabulares** - [Goodtables.io](http://try.goodtables.io/) es un servicio en línea gratuito para la validación continua de datos. Comprueba un archivo de datos tabulares en busca de problemas estructurales, como filas en blanco y valida que los datos sigan determinado esquema creado con _Table Schema_ (como es el caso para este estándar).

2. **GitHub Action para la validación de datos** - [Frictionless Repository](https://repository.frictionlessdata.io/) es un servicio de gestión de datos para la validación continua de datos en un repositorio a través de Github Actions. Se manera automática valida continuamente los datos en busca de errores tabulares y proporciona un informe visual y te permite automatizar el proceso para publicar datos bajo el estándar.

3. **Data framework para Python** - [Frictionless Framework](https://framework.frictionlessdata.io/) es un marco de gestión de datos para que Python describa, extraiga, valide y transforme datos tabulares. Te permite utilizar Python para trabajar los conjuntos de datos y realizar las acciones necesarias para implementar el estándar.

4. **Visualizador de esquemas** - [Frictionless Components](https://components.frictionlessdata.io) es una librería que te permite visualizar los componentes de Framework de _Frictionless Data_ como los esquemas y paquetes através de una interfaz gráfica amigable. Te permite crear y editar varias estructuras de metadatos del estándar de manera visual.

5. **Presentación de datos** - [Livemark](https://livemark.frictionlessdata.io/) es un marco de presentación de datos para Python que genera sitios estáticos a partir de Markdown extendido con gráficos interactivos, tablas, scripts y otras características. Te permite publicar informes sobre datos publicados bajo el estándar.

6. **Otras librerías** - [Frictionless Libraries](https://libraries.frictionlessdata.io/) son un conjunto de bibliotecas de integración de datos para 10 lenguajes de programación que implementan conceptos de Frictionless Data a través de lenguajes de programación.