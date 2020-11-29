# Sismos en Ecuador

Practicar sus conocimientos en representación cartográfica con datos de puntos.

### Requisitos

Crear un cuenta en ArcGIS Online de tipo Desarrollador y acceder a su espacio en www.arcgis.com. Tenga en cuenta de crear una carpeta en su espacio de contenido bajo el nombre **EJERCICIOS**.

## Resumen

ArcGIS online permite crear una vista de mapas en línea con qué interactuar y componer capas temáticas. En este ejercicio creará un mapa que muestre los sismos registrados en Ecuador en el año 2016. Se podrá visualizar la ubicación de los mismos con una simbología simple y además en otro mapa clasificar de acuerdo a la magnitud del evento. Adicionalmente se habilitara la opción de filtro por tiempo. Finalmente se compartirá el mapa como una aplicación web simple para que otros usuarios puedan explorarlo. 

### Guía de pasos

- [Crear capa alojada](#crear-capa-alojada)
- [Crear mapa de ubicación](#crear-mapa-de-ubicación)
- [Crear mapa de magnitud](#crear-mapa-de-magnitud)
- [Publicar aplicación web](#publicar-aplicación-web)

## Crear capa alojada

El primer paso de nuestro ejercicio consiste en crear un capa alojada a partir de un archivo Excel. Una capa alojada es un *servicio* que permite publicar información geográfica de tipo punto, línea y polígono. Para este ejercicio utilizaremos la siguiente información:

![sismos_excel](img\sismos_excel.png)

El enlace para descargar los datos se encuentra en el siguiente enlace: https://arcg.is/qGGLT 

La capa de puntos depende las columnas de la tabla denominadas **latitude** y **longitude** que serán utilizadas para suministrar la localización de los sismos. Otro campo importante es la **mag** (magnitud) y **time** (fecha).

En ArcGIS Online proceda a utilizar el botón *AGREGAR ELEMENTO* y elija la opción *DESDE EL EQUIPO*. Utiliza un dialogo como se muestra en la figura.

![sismos_add_layer](img\sismos_add_layer.png)

Los datos más importantes de este formulario son:

- Archivo: el excel Sismos.xlsx a utilizar como fuente de información.
- Título: nombre de la capa. Ej. Sismos 2016
- Etiquetas: datos adicionales para buscar información acerca del tema.
- Publicar este archivo como capa alojada: Tildar esta opción
- Localizar entidades por: Coordenadas
- En Campos de ubicación elegir X e Y como columnas para Longitud y Latitud.

Una vez completado confirmar con el botón AGREGAR ELEMENTO. Debe tener en cuenta que puede tardar unos segundos para crear el contenido en la plataforma. El resultado obtenido será una nueva capa de puntos creada.

![sismos_new_layer](img\sismos_new_layer.png)

### Examinar datos 

Cada vez crea una capa alojada se accede directo a la página de la misma. También se puede acceder desde CONTENIDO y luego accede al enlace sobre el nombre de la capa alojada para tener la siguiente vista.

<img src="img\sismos_layer.png" alt="sismos_layer" style="zoom:67%;" />

Puede acceder a los datos en forma tabular en la pestaña de DATOS y en la vista geográfica en VISUALIZACIÓN. Examine la información recientemente creada.

### Habilitar filtro de tiempo

Para habilitar la opción de tiempo puede utilizar el campo **Fecha** para este propósito. En el mapa esto puede utilizarse como filtro para poder interactivamente visualizar sismos en función al tiempo. En la sección de CAPAS elija la capa de puntos *Sismos_0* y luego en la parte inferior derecha presionar la opción HABILITAR con la siguiente configuración.

<img src="img\sismos_layer_time.png" alt="sismos_layer_time " style="zoom:67%;" />

## Crear mapa de ubicación



## Crear mapa de magnitud



## Publicar aplicación web