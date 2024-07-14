# Ganancia real acciones
Lo que se busca con este proyecto es poder consumir una api que nos devuelve el valor del dolar (CCL en este caso) y ver la ganancia real de nuestros activos reflejada en dolares.

## Descripción
Para este proyecto se utilizaron las siguientes librerias:
* Pandas.
* yfinance
* request
* datetime
* plotly
* google.cloud
* os

Lo que hace el código básicamente es con una función consumir la api de mercados de ambito y devolver el valor del dolar al día de hoy. Luego utilizando la libreria firestore de google.cloud, hacemos una conexión a la base para obtener nuestros tickers, su cantidad y el precio promedio de compra. Con este df hacemos la descarga de los activos usando la libreria de yfinance y luego hacemos los cálculos correspondientes agregandolos en columnas para saber lo total invertido y nuestras ganancias netas tanto en dolares como en pesos.
Se realiza también la descarga del dataframe en un archivo xlsx.
Luego con toda esta data, utilizamos la librería plotly, trayendo únicamente plotly.express y plotly.graph_objs para realizar gráficos ineractivos y visualmente atractivos. Los gráficos que se seleccionaron para el análisis fueron el gráfico circular para mostrar la participación de cada activo, y un gráfico de barras para mostrar la cantidad invertida vs la cantidad de ganancia neta de cada ticker. A continuación se adjunta una imagen de ambos gráficos.

![pie](https://github.com/user-attachments/assets/cba856cc-4c5d-4e8c-82ab-714e0880ef7c)

![bar](https://github.com/user-attachments/assets/5338a0cf-f7a3-4ed3-8d69-7fe8bfb2964e)


