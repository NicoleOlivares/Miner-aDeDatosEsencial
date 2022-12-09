# MineriaDeDatosEsencial

# Conceptos:

## Estructura de minería de datos: "Tipos de datos"
- Si cambia el tipo de dato se debe volver a procesar la estructura de minería y también se debe volver a procesar todos los modelos.

- Algunos algoritmos solo funcionan con tipo de datos continuos. 

- Cada tipo de datos admite uno o más tipos de contenido. Que puede utilizar para describir el compartamiento de datos que contiene la columna. 

- Hay que asegurarse que los datos sean continuos o discretos. 

## Columna discreta:
- Contiene un número finito de valores, ya sea, porque la entrada númerica se ha limitado a un conjunto determinado de valores o es un texto. El texto siempre se trata como valor discreto. 

- Los datos no están ordenados.

- Los valores no se pueden fraccionar.

- Compatible con todos los otros datos. 

## Columna continua:
- Incluye valores fraccionales infinitos.

- Siempre contiene datos númericos. Contiene datos medidas. 

- Es compatible con los tipos de datos: date, double y long.

## Columna discretizada:

Una columna ha sido discretizada cuando la columana contiene valores que representan grupos o despósitos de valores que se deriban de una columna continua. Los depósitos se tratan como valores ordenados y discretos.
Es compatible con: date, double, long y text.

## Columna tipo llave o clave:
- Identifica una fila de forma única.
- En una tabla de casos tiene un identificador númerico o de texto. 
- Se usa para el seguimiento de los registros. 
- Es compatible con: date, double, long y text.

Las tablas anidadas también tiene clave:
- Es el atributo analizable en tablas anidades.
- Los valores deben ser únicos para cada caso.
- Puede haber duplicados en todo el conjunto de casos.

## Columna Clave de secuencia:
- Los valores representan una secuencia de eventos.
- Ordenados y sin necesitar separación equivalente. 
- Es compatible con: date, double, long y text.

## Columna clave de tiempo:
- Valores ordenados y en una escala de tiempo.
- Es compatible con los tipos de datos: date, double y long.

## Columna tipo ordenado:
- Valores que definen un conjunto ordenado.
- Discretas en términos de tipo de contenido.
- Compatibles con todos los tipos de datos.

## Columna Cíclica:
- Conjunto ordenado cíclico, por ejemplo, los días de la semana. 
- ordenadas y discretas en términos de tipo de contenido. 
- Son compatibles con todos los tipos de datos.

## Columna tipo tabla:
- Contiene una table de datos anidada, con una o más columnas y una o más filas. 
- Pueden existir varias columnas de tabla anidada en una tabla de casos.
- Para cada fila de la tabla de casos la tabla anidada puede contener varios valores todos ellos relacionados con el registro de caso primario.
- El tipo de datos de esta columna siempre es table.

Esto es impoirtante para saber que utilizar para los algoritmos. 
Cuando se crea un modelo de minería de datos, la ambigûedad en los datos puede generar errores o impedir que se utilicen algunos algoritmos. 



