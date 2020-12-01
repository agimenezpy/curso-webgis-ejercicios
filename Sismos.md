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
- [Compartir mapas web](#compartir-mapas-web)

## Crear capa alojada

El primer paso de nuestro ejercicio consiste en crear un capa alojada a partir de un archivo Excel. Una capa alojada es un *servicio* que permite publicar información geográfica de tipo punto, línea y polígono. Para este ejercicio utilizaremos la siguiente información:

![sismos_excel](img\sismos_excel.png)

El enlace para descargar los datos se encuentra en el siguiente enlace: https://arcg.is/qGGLT 

La capa de puntos depende las columnas de la tabla denominadas **latitude** y **longitude** que serán utilizadas para suministrar la localización de los sismos. Otro campo importante es la **mag** (magnitud) y **time** (fecha).

En ArcGIS Online proceda a utilizar el botón *AGREGAR ELEMENTO* y elija la opción *DESDE EL EQUIPO*. Utiliza un dialogo como se muestra en la figura.

![sismos_add_layer](img\sismos_add_layer.png)

Los datos más importantes de este formulario son:

- Archivo: el Excel **Sismos.xlsx** a utilizar como fuente de información.
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

Como parte del proyecto “Sismos en Ecuador” se crea un mapa web para desplegar la ubicación de los sismos con una simbología simple. A partir de la capa alojada "Sismos 2016" creada anteriormente se procede desde la sección CONTENIDO a acceder a la creación de un mapa nuevo por el botón ABRIR EN MAPVIEWER.

![sismos_new_map](img\sismos_new_map.png)

Asegurarse de crear un mapa nuevo, en caso del que el MapViewer abra un mapa anterior puede presionar el botón CREAR MAPA NUEVO. Una vez abierto el MapViewer se procede a GUARDAR el mapa con el título "Mapa de Sismos 2016", poner etiquetas correspondientes y guardar en la carpeta EJERCICIOS.

Luego se debe elegir el MAPA BASE de nombre TERRENO CON ETIQUETAS y después simbolizar con una configuración simple a través de la opción CAMBIAR ESTILO.

![sismos_style1](img\sismos_style1.png)

El estilo sería de mostrar ubicación por medio de un símbolo de circulo de color rojo. El mapa final quedaría como esta en la figura.

<img src="img\sismos_map1.png" alt="sismos_map1" style="zoom:67%;" />

El rango visible debe estar en PAIS y luego confirmar con ACEPTAR. Se debe GUARDAR el mapa antes de volver a CONTENIDO.

## Crear mapa de magnitud

Adicionalmente para el tema de “Sismos en Ecuador” se crea un mapa web para desplegar la magnitud de los sismos con una simbología de recuento y cantidades con una variante de color. A partir de la capa alojada "Sismos 2016" creada anteriormente se procede desde la sección CONTENIDO a acceder a la creación de un mapa nuevo por el botón AGREGAR AL MAPA NUEVO.

![image_new_map2](img\sismos_new_map2.png)

Una vez abierto el MapViewer se procede a GUARDAR el mapa con el título "Mapa de Sismos Magnitud 2016", poner etiquetas correspondientes y guardar en la carpeta EJERCICIOS.

Luego se debe elegir el MAPA BASE de nombre TERRENO CON ETIQUETAS y  simbolizar la capa con una configuración de recuentos y cantidades a través de la opción CAMBIAR ESTILO.

![sismos_style2](img\sismos_style2.png)

Se debe elegir el atributo MAGNITUD y realizar los cortes numéricos como se muestra en la figura por medio de una clasificación manual de 4 grupos.

<img src="img\sismos_map2.png" alt="sismos_map2" style="zoom:67%;" />

 El nivel de rango visible debe ser a nivel PAIS. Luego de realizar todos los cambios se procede ACEPTAR y finalmente GUARDAR el mapa. El nombre de la capa debe ser renombrada a "Sismos 2016" desde el menú adicional de opciones y además configurar la ventana emergente con los tres campos desplegados:

<img src="img\sismos_popup.png" alt="sismos_popup" style="zoom:67%;" />

La configuración de la ventana emergente debe ser correctamente asignado a los tres campo un valor legible en el "ALIAS", en el título de la ventana y la configuración de los campos numéricos de PROFUNDIDAD (0 decimales) y MAGNITUD (2 decimales).

![sismos_popup_det](img\sismos_popup_det.png)

Luego de realizar todos los cambios se procede ACEPTAR y finalmente GUARDAR el mapa. Al terminar se dirige a la sección de CONTENIDO.

## Compartir mapas web

Luego de finalizar la edición del mapa puede proceder a compartir los mapas desde CONTENIDO por el enlace rápido y elegir TODOS.

![sismos_share](img\sismos_share.png)

Para capturar un enlace de su mapa puede acceder al ABRIR EN MAPVIEWER el mapa y presionar el botón COMPARTIR para capturar la URL corta de su mapa web.

<img src="img\sismos_share_link.png" alt="sismos_share_link" style="zoom:70%;" /> 

