# Documentación General del Sistema Web de Indicadores# Descripción General
Este proyecto representa una interfaz web de gestión de indicadores desarrollada íntegramente en HTML y CSS. El enfoque principal del sistema es permitir al usuario iniciar sesión y, a partir de ahí, navegar entre distintas funcionalidades relacionadas con la gestión de datos: agregar, eliminar, visualizar y reportar indicadores, así como acceder a una sección de ayuda.

La interfaz utiliza un diseño estático con unidades relativas para asegurar un control total sobre la distribución visual en todas las pantallas. Esto proporciona precisión en la colocación de cada elemento, aunque sacrifica cierta flexibilidad en dispositivos con resoluciones diferentes.

# Estructura de Archivos
El sistema se compone de los siguientes archivos HTML:

[./index.html](index.html.)

[./logued.html](logued.html.)

[./add.html](add.html.)

[./delete.html](delete.html.)

[./report.html](report.html.)

[./help.html](help.html.)

# index.html
Esta página representa la puerta de entrada al sistema. Incluye dos campos principales para que el usuario ingrese sus credenciales:

Usuario

Contraseña

Tras llenar los campos, se hace clic en el botón de "Ingresar", el cual redirige directamente al logued.html, simulando una autenticación sin validación real. No se implementan scripts de validación o seguridad; el comportamiento es completamente estático.

# logued.html
Una vez que el usuario ha accedido, llega a la página principal. Este es el centro todas las opciones. La interfaz muestra una serie de íconos alineados horizontalmente que enlazan a diferentes funcionalidades:

# Acción	Archivo destino	Descripción
# Añadir	add.html	    Formulario para agregar un nuevo indicador.
# Refrescar	logued.html	    Recarga la misma página.
# Eliminar	delete.html	    Selección y eliminación de indicadores.
# Reportar	report.html	    Visualización tabular de indicadores y datos.
# Ayuda	    help.html	        Página de soporte o preguntas frecuentes.

# add.html
Esta página presenta una interfaz en la cual el usuario llenará la información requerida:

Nombre del indicador

Descripción

Categoría

Fecha de inicio y finalización

Método de medición

Frecuencia

Porcentaje de cumplimiento

Área responsable

Una vez diligenciada toda la información se presionará el botón de "añadir" se redigirá a la página principal.

# delete.html
Esta sección permite al usuario seleccionar uno o varios indicadores desde una lista para su posible eliminación. Cada fila contiene:

Una casilla de verificación

El botón "Eliminar" está presente al final y al presionarlo nos redirige a la página principal.

# report.html
Se trata de la página más informativa del sistema donde se listan múltiples indicadores con todos sus atributos relevantes. Utiliza un bloque de texto preformateado ("pre") para simular una tabla alineada. Cada fila incluye:

Nombre

Descripción

Categoría

Fechas de inicio y fin

Método de medición

Frecuencia

Porcentaje de cumplimiento

Área responsable

También se presentan casillas de verificación al lado derecho de cada fila.

# help.html
La sección de ayuda está pensada para mostrar orientación básica al usuario.
