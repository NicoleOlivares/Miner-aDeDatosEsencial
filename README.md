# MineriaDeDatosEsencial

# Conceptos:

## Estructura de minería de datos: "Tipos de datos"
- Si cambia el tipo de dato se debe volver a procesar la estructura de minería y también se debe volver a procesar todos los modelos.

- Algunos algoritmos solo funcionan con tipo de datos continuos. 

- Cada tipo de datos admite uno o más tipos de contenido. Que puede utilizar para describir el compartamiento de datos que contiene la columna. 

- Hay que asegurarse que los datos sean continuos o discretos. 

- Una misma estructura de datos puede admitir varios modelos de minería que comparten el mismo dominio.

- Algunos tipos de datos que existen en minería de datos son: text, long, boolean, double y date. 

### Columna discreta:
- Contiene un número finito de valores, ya sea, porque la entrada númerica se ha limitado a un conjunto determinado de valores o es un texto. El texto siempre se trata como valor discreto. 

- Los datos no están ordenados.

- Los valores no se pueden fraccionar.

- Compatible con todos los otros datos. 

### Columna continua:
- Incluye valores fraccionales infinitos.

- Siempre contiene datos númericos. Contiene datos medidas. 

- Es compatible con los tipos de datos: date, double y long.

### Columna discretizada:

Una columna ha sido discretizada cuando la columana contiene valores que representan grupos o despósitos de valores que se deriban de una columna continua. Los depósitos se tratan como valores ordenados y discretos.
Es compatible con: date, double, long y text.

### Columna tipo llave o clave:
- Identifica una fila de forma única.
- En una tabla de casos tiene un identificador númerico o de texto. 
- Se usa para el seguimiento de los registros. 
- Es compatible con: date, double, long y text.

Las tablas anidadas también tiene clave:
- Es el atributo analizable en tablas anidades.
- Los valores deben ser únicos para cada caso.
- Puede haber duplicados en todo el conjunto de casos.

### Columna Clave de secuencia:
- Los valores representan una secuencia de eventos.
- Ordenados y sin necesitar separación equivalente. 
- Es compatible con: date, double, long y text.

### Columna clave de tiempo:
- Valores ordenados y en una escala de tiempo.
- Es compatible con los tipos de datos: date, double y long.

### Columna tipo ordenado:
- Valores que definen un conjunto ordenado.
- Discretas en términos de tipo de contenido.
- Compatibles con todos los tipos de datos.

### Columna Cíclica:
- Conjunto ordenado cíclico, por ejemplo, los días de la semana. 
- ordenadas y discretas en términos de tipo de contenido. 
- Son compatibles con todos los tipos de datos.

### Columna tipo tabla:
- Contiene una table de datos anidada, con una o más columnas y una o más filas. 
- Pueden existir varias columnas de tabla anidada en una tabla de casos.
- Para cada fila de la tabla de casos la tabla anidada puede contener varios valores todos ellos relacionados con el registro de caso primario.
- El tipo de datos de esta columna siempre es table.

Esto es impoirtante para saber que utilizar para los algoritmos. 
Cuando se crea un modelo de minería de datos, la ambigûedad en los datos puede generar errores o impedir que se utilicen algunos algoritmos. 

## Pasos para crear un modelo:
- Crear la estructura de minería de datos.
- Seleccionar el algoritmo más adecuado.
- Elegir las columnas de estructuras que se van a usar en el modelo.
- Definir las propiedades de las columnas, especificar.
- Establecer parámetros.
- Procesar la estructura y el modelo. 

### Propiedades de los modelos de minería:
- Nombre.
- Descripción.
- Fecha de último procesado.
- Permiso.
- Filtros.
- Propiedades derivadas.

Propiedades especiales: algoritmos y uso

Una vez procesado el modelo de minería este almacena información sobre los datos y patrones. Incluyendo estadísticas, reglas y fórmulas de regresión.

## Algoritmos de minería de datos:

### Algoritmos de clasificación:
Predicen una o más variables discretas basándose en los demás atributos del conjunto de datos.

- Árbol de decisión: columna de una sola clave, no están permitidas las claves compuestas. Una columna de predicción. Pueden ser de tipos diferentes. Columnas de entrada discreta o continuas. Mientras más columnas, más se demora. 

- Red neuronal.
Predecir un resultado, comercialización y promoción, procesos industriales y de producción, etc. Depende del número de estados de las columnas de entrada. Depende del número de columnas de predicción y del número de estados de las columnas de predicción.

- Naive Bayes.
técnicas bayesianas. Probabilidad de cada estado de cada columna de entrada.
Con este algoritmo un departamento de comercialización puede predecir el resultado de un perfil de cliente concreto. 
No están permitadas las claves compuestas. 
Variables independientes y las de entrada también. 

### Algoritmos de regresión:
Predicen una o más variables númericas continuas como pérdidas o ganancias. basándose en otros atributos del conjunto de datos.
- Series temporales. 
No necesita columnas adicionales de entrada.
Predice tendencias basadas en los datos originales.
Se pueden agregar datos. 

Serie: Combinación de los datos de origen y los datos de la predicción.

El modelo de serie temporal utiliza una mezcla de dos algoritmos. 

Ocupa dos modelos, un modelo ocupa el algoritmo ARTXP y obtiene mejores resultados en las predicciones a corto plazo.
Y el otro modelo utiliza el algoritmo ARIMA utilizado para la predicción a largo plazo.

Combina los resultados de los dos modelos para obtener la mejor predicción sobre un número variable de intervalos de tiempo. 

Una columna key time con valores continuos.
una columna predecible
una columna de clave de serie opcional

- Regrasión lineal.
Ayuda a calcular una relación lineal entre una variable independiente y otra dependiente. 
Utiliza esa relación para la predicción. 

La relación toma la forma de una ecuación para la línea que mejor represente una serie de datos.
Es un método útil y conocido para modelar una respuesta a un cambio de algún factor subyacente. 

Se calculan y se prueban automaticamente todas las posibles relaciones entre las variables.
La regresión lineal podría simplificar el exceso de relaciones en escenarios en los que varios factores afectan al resultado.

Datos númericos continuos. Esta denso, estudiar más. También se puede crear un árbol de desición para regresión.

- Regresión logística. 
Modelo resultados binarios.
Método estadístico donde la curva de los datos se comprime mediante una transformación logística para minimizar el efecto de los valores extremos.

Columna númerica o de texto, clave unica, una columna de entrada o más. Al menos necesita una columna de predicción. No se admiten tablas anidadas en la columna de predicción, pero si de entrada. 

riesgo de enfermedad, demografico, que los clientes vuelvan o clasificar objetos con muchos atributos.

### Algoritmos de segmentación o clústering:
Que dividen los datos en grupos de elementos que tienen propiedades similares. 
- Tipo de segmentación.
- Divide los datos en grupos o clústures de elementos que tienen propiedades similares. Que no se podrían deribar lógicamente a través de la observación casual.
- Se utiliza para identificar agrupamientos naturales de casos basados en un conjunto de atributos.

La agrupación en clústeers es una tarea de minería de datos no supervisada. Todos los atributos de entrada son tratados por igual.

La mayoria de los algoritmo de clústering construyen a través de una serie de iteraciones y se detienen cuando el modelo converge, es decir, cuando los límites de estos segmentos están estabilizados.
Entrena el modelo de forma estricta a partir de las relaciones que existen en los datos y de los clústeres que identifique el algoritmo. 

Nota: investigar más. 

### Algoritmos de asociación:
Que buscan correlaciones entre diferentes atributos de un conjunto de datos para la creación de reglas de asociación.
- Algoritmo de asociación.

### Algoritmos de análisis de secuencias:
Que crean un resumen de las secuencias frecuentes o episodios en los datos como una serie de clicks en un sitio web.
- Clústers de secuencias.

Para seleccionar el tipo de algoritmo adecuado hay que enfocarse en el tipo de tarea a realizar. 

