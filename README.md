HENRY’S LABS
Roberto Pedro DATA-12
PROYECTO INDIVIDUAL 02 --Data Analyst


## Análisis del Sector de Telecomunicaciones en Argentina

### Descripción del Problema

El proyecto tiene como objetivo realizar un análisis completo del sector de las telecomunicaciones en Argentina, específicamente en el acceso a internet fijo y otros servicios de comunicación en Argentina. Se busca entender el comportamiento del sector, identificar oportunidades de crecimiento y mejorar la calidad de los servicios ofrecidos.

### EDA (Exploratory Data Analysis)

Se realizó un análisis exploratorio de los datos utilizando las librerías Numpy, Pandas y se generaron visualizaciones con ProfileReport, Matplotlib y Seaborn


### Dashboard

Se implementó un dashboard funcional y coherente con el storytelling. El dashboard incluye filtros interactivos que permiten explorar los datos en detalle. Se enfocó en presentar de manera clara y estética la información relevante sobre el sector de telecomunicaciones.

### KPIs (Indicadores Clave de Desempeño)

Se sugirieron 3 KPIs relacionados con la historia del análisis. Estos indicadores se muestran en el dashboard y se explicó su funcionalidad en la presentación.
kPI1: Aumentar el volumen de facturación de internet fijo en un 20% anual respecto al año anterior.

KPI2: Aumento de velocidad de bajada un 15% anual.

KPI3: Aumento 20%de servicios de cablemodem  en un año. 



### Conclusiones de cada Dataset


 ####"I__baf1.ipynb"
Número total de accesos al servicio de Internet fijo por banda ancha y banda angosta .
_El acceso a internet fijo por banda ancha ha ido creciendo todos los años
_El acceso por dial up ha disminuido
_No se identificaron valores extremos en las columnas numéricas
_Banda ancha  el 75 % esta alrededor de 900.000
_Banda ancha, mediana esta alrededor de 8.000
_Dial up el 100% llega alrededor de 39.000
_Dial up, mediana esta alrededor de 23.000

#### int fijo_vel.
Número de accesos al servicio de Internet fijo por velocidad de bajada en cada provincia. 
_El servicio de velocidad mas usada es el de  hasta +30 kbps observado en grandes ciudades especialmente.
_Los valores maximos llegan alrededor de 1 millon aprox.
_No se observan valores nulos o faltantes en el dataset
_Hay valores extremos en las columnas numéricas
_Existe alta correlación entre ciertos rangos de velocidad
_Se registran datos desde el año 2014 hasta el 3er trimestre de 2022
_La velocidad  de acceso desde  menos de 512 MBps .hasta +30 Mbps


#### Int_Acses_x_tecnolog_
Número de accesos al servicio de Internet fijo por tipo de tecnología. Total nacional .
_No se observan columnas con valores nulos ni faltantes
_La columna ADSL(BANDA ANCHA) sesgada hacia la derecha
_Fibra optica tiene la mediana mas baja, comparada con las otras columnas
_ADSL hay una alta correlacion inversa con el resto de tipos de acseso a internet
_Cable Modem hay una alta correlacion  con el resto de tipos de acseso, exceptuando ADSL
_Se observan outliers en la columna Fibra óptica
_El 75% de	Cablemodem ronda en	5.1 millones
_El 75% de Fibra optica ronda 1.1 millones
_El 75% de	ADSL ronda en 3,7 millones Y 3,8 mill es su maximo
_wirelles sesgado hacia la izquierda
_Aumento de valores en cablemodem cada año


#### int_fijo_prov
Número de accesos al servicio de Internet fijo por banda ancha y banda angosta en cada provincia.
- No se observan valores nulos o faltantes en el dataset
- La columna ADSL (Banda Ancha) muestra un sesgo hacia la derecha
- Fibra Óptica tiene la media más baja en comparación con otras columnas
- El acceso ADSL tiene una alta correlación inversa con otros tipos de acceso a internet
- Se observan outliers en la columna Fibra Óptica
- El 75% de los accesos Cablemodem ronda en 5.1 millones y el 75% de Fibra Óptica ronda en 1.1 millones

#### Int_ingresos
Ingresos trimestrales por la prestación del servicio de Internet fijo.
- No se observan valores faltantes ni nulos en el dataset.
- El trimestre 4 tiene registros únicos nueve veces, excepto el 4 que tiene 8 registros únicos.
- Los ingresos aumentan sostenidamente cada año y el 3er trimestre destaca como el de mayor ingreso históricamente.
- No se observan outliers en los ingresos.

#### Int_penetracion
Accesos a banda ancha y banda angosta por provincia.
Serie trimestral de la penetración del Internet fijo en la métrica por cada 100 hogares y aceso Accesos por cada 100 hab
- No se observan valores faltantes ni nulos en el dataset.
- No se observan valores atípicos en ninguna de las columnas.
- La cantidad de hogares con internet aumenta anualmente.
- La columna "Acs_x_c_100_Hab" muestra un valor máximo cercano a 24.
- Se observa un aumento en la cantidad de accesos por cada 100 habitantes.
- No se observan valores atipicos
-Observamos que va aumentando la cantidad de acseso por cada 100 habitantes, observando el minimo  9 

#### Int_tipo_localidades
Listado de localidades con conectividad a internet, con detalle por tipo de conexión.
- Se detectaron filas duplicadas y se eliminaron
- El 25% del servicio corresponde a SATELITAL
- "Wireless" tiene una presencia del 48% en las localidades.
- El 50% de la conectividad es a través de telefonia fija.
- Existe una alta correlación entre "TELEFONIAFIJA" y "ADSL"
- Se observan datos de 24 provincias, 444 partidos y 3912 localidades
- Presencia del 50% de servicio telefonia fija
- TELEFONIAFIJA altamente correalacionada con ADSL
- El tipo de conectividad CABLEMODEM 20%
- El tipo de conectividad menos usado es WIRELESS DIALUP 9%

#### Int_vel_bajada.csv
Velocidad Media de bajada(descarga) de Internet fijo.
- No se observan valores faltantes ni nulos.
- La velocidad media de bajada se encuentra entre 4 y 60 Mbps aproximadamente.
- Existe una alta densidad entre 4 y 20 Mbps.
- No se observan outliers en los datos.
- El valor máximo de velocidad de bajada es de 62.46 Mbps.
- El 75% de la velocidad de bajada se encuentra entre 3 y 40 Mbps.
- Los registros muestran un aumento gradual en la velocidad de bajada desde el trimestre 1 de 2021 hasta el último registro, alcanzando su máximo de 62.46 Mbps.

### Observaciones Generales

Los datasets analizados proporcionan información relevante sobre el sector de las telecomunicaciones en Argentina, incluyendo ingresos, penetración de Internet, tipos de conectividad y velocidad de bajada.

Informcion extraida de ENACOM, LINK:https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/
