# Ganancia real acciones
Lo que se busca con este proyecto es poder consumir una api que nos devuelve el valor del dolar (CCL en este caso) y ver la ganancia real de nuestros activos reflejada en dolares.

## Descripción
Para este proyecto se utilizaron las siguientes librerias:
* Pandas.
* yfinance
* request
* datetime
* plotly

Lo que hace el código básicamente es con una función consumir la api y devolver el valor del dolar al día de hoy. Luego se crea un dataframe manualmente donde se colocan nuestros tickers, su cantidad y el precio promedio de compra. Con este df hacemos la descarga de los activos con yfinance y luego hacemos los cálculos correspondientes agregandolos en columnas para saber lo total invertido y nuestras ganancias netas tanto en dolares como en pesos.
Luego con toda esta data, utilizamos la librería plotly, trayendo únicamente plotly.express y plotly.graph_objs para realizar gráficos ineractivos y visualmente atractivos. Los gráficos que se seleccionaron para el análisis fueron el gráfico circular para mostrar la participación de cada activo, y un gráfico de barras para mostrar la cantidad invertida vs la cantidad de ganancia neta de cada ticker. A continuación se adjunta una imagen de ambos gráficos.

![pie](https://github.com/Franco2411/ganancia-real-acciones/assets/70663058/7acfc31b-93f2-4092-bb0b-4a7dfa513fea)

![bar](https://github.com/Franco2411/ganancia-real-acciones/assets/70663058/113f45ab-1cc6-474e-bf24-4d4eb66c7252)

