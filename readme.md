# INTRODUCCIÓN
### Nuestro segundo proyecto está basado en datos de la emprea de telecomunicaciones ENACOM en Argentina,  y el análisis exploratorio de los mismos, el cual debemos entregar en este informe. He extraído de la web de ENACOM, diferentes archivos csv, de los cuales he elegido algunos para luego poder desarrollar mi Dashboard y crear los 3 kpi's solicitados. 
### He seleccionado tamabién un csv externo con los datos de latitud y longitud de las distintas provincias.
### En este informe solo nos enfocarems en contar los EDA realizados.

# ANALISIS EXPLORATORIO DE LOS DATOS
### En este proyecto realizaré un análisis basado en la industria de la telecomunicaciones principalmente el acceso a internet, tanto del tipo de tecnología, como la velocidad media de bajada contratada, como analizar el internet fijo cada 100 hogares y los  ingresos de este servicio a nivel nacional.

## Elección de la fuente de datos
### Nuestra fuenta de datos está dentro de la página web de ENACOM. He intentado por intermedio de su API descargar los csv, pero al tener muchos errores, los cuales he intentado de solucionar, decidí descargarlos manualmente (por falta de tiempo y que no me alcanzara el mismo para todo el proceso).

### Luego de analizar todos los csv, he decido seleccionar algunos de ellos para mi análisis y futuras conclusiones. 

## Fuente de datos
### [DATASETS](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/)
### [DATASETS EXTERNO](https://datos.gob.ar/ar/dataset/jgm-servicio-normalizacion-datos-geograficos/archivo/jgm_8.9)
### He descargado los datos manualmente, debido a que por intermedio de la api he tenido algunos inconvenientes. Luego de estudiar los archivos he escogido los siguientes:  

### * Penetración de Internet fijo (accesos por cada 100 hogares) en provincia(trimestral),esta elección has sido para valorar a nivel de provincias la realidad en cada una de ella por cada 100 hogares que es un histórico del 2014 hasta el tercer trimestre del 2022.    


### * Acceso a Internet fijo por tecnología y provincia(trimestral)
### El histórico de esta tabla nos da información de todas las tecnologías en las diferentes provincias y el acceso a las mimas por parte de la población.

### * Velocidad media de bajada de Internet fijo por provincia (trimestral)
### En este csv nos dan la velocidad de descarga que tienen cada provincia, o sea el timpo de descarga que tarda en llegar la información en llegar a los horgares desde internet.


### * Internet Ingresos (trimestral, anual), por otro lado tenemos los ingresos por trimestre, lo cual intentaré ver el crecimiento en los diferentes trimestres.

## Análisis de los datos  

#### He realizado el análisis de mis datos con pandas,comenzando en todos con una análisis de las primeras filas, para luego ver los datos que tengo en cada uno de los csv, para modificarlos en caso necesario. Luego de transformar los datos:  
### - Reemplacé los puntos por vacíos
### - Eliminé caracteres no numéricos en algunas columnas
### - Corroboré duplicados y vacíos

### Hice un primer análisis  estadístico descriptivo de todos las tablas.
  
### Luego realicé un análisis de outliers creando un gráfico de cajas y posteriormente hice los histogramas correpondientes para ver su comportamiento en el gráfico.   
### Por útlimo cree una tabla pivot para analizar mejor los datos (comentarios en el EDA) y con esta tabla hice unos gráficos.  
### Con los csv ya preparados, los subiré a Power Bi para poder crear  un Dashboard con la creación de los kpi's

## PRIMERA CONCLUSIONES  
### Luego de explorar los datos y analizarlos, vemos que Buenos Aires en el total de accesos por tecnologías es que que tiene el mayor valor, seguido por Capital Federal. Que al realizar la gráfica de los totales con respecto a las provincias y los totales del último año, vemos que no hay grandes cambios.
### También he podido ver que cuando analizamos el acceso por cada 100 hogares, vemos que aparece en primer lugar Capital Federal. Para poder evaluar mejor estas diferencias en los datos, primero sabemos que la población en la provincia de Buenos Aires es mucho mayor que la de Capital Federal, y a pesar de tener  un acceso por cada 100 hogares más bajo, el total de acceso puede seguir siendo mayor en Buenos Aires debido a su mayor población total. 
### También puede haber una distribución de las distintas tecnologías.
### Aquí habría que tener otros factores en cuenta la infraestructua existente, la disponibilidad de servicios, la densidad de la población y las características socio-económicas.
### También debemos tener en cuenta que estas métricas total de accesos y accesos por cada 100 hogares son diferentes y dan diferentes perspectivas sobre el acceso a las tecnologías.
