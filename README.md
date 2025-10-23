<span style="color: #2917f3ff;">**EDA: RELACIÓN DE LOS PRINCIPALES ÍNDICES ECONÓMICOS**</span>


<span style="color: #a11056ff;">*EL VALOR DE BITCOIN ESTÁ MÁS LIGADO A LA M2 QUE OTROS ÍNDICES COMO EL SP500 O EL ORO*</span>






/img/corr6.jpg




El archivo principal.ipynb es un cuaderno de Jupyter que realiza un análisis exploratorio de datos (EDA) sobre series financieras clave: el índice S&P 500, el precio del oro, el precio del Bitcoin y la oferta monetaria M2 de EE. UU. El análisis abarca desde octubre de 2014 hasta agosto de 2025, utilizando datos mensuales. El objetivo principal es comparar el crecimiento relativo de estos activos y la masa monetaria a lo largo del tiempo, normalizando los datos para que todas las series comiencen desde el mismo punto (octubre de 2014) y así facilitar la comparación visual de su rendimiento.

Preparación y Normalización de Datos
El análisis comienza con la carga y limpieza de los datos de cada serie. Los datos se normalizan restando el valor inicial de cada serie, lo que permite que todas comiencen en cero en el gráfico. Esto se hace para visualizar el crecimiento porcentual desde el punto de partida común. El código utiliza bibliotecas como pandas para la manipulación de datos y matplotlib o plotly para la visualización. Un paso clave es la creación de una columna combinada (dfunido) que almacena todos los datos normalizados, aunque se encontró un error en el código al intentar acceder a una columna llamada m2 Billions pct, lo que sugiere un problema en el cálculo del porcentaje de crecimiento para la oferta monetaria M2.

Visualización de Resultados
El cuaderno genera múltiples gráficos para representar los datos. El gráfico principal superpone las cuatro series (M2, S&P 500, Oro, Bitcoin) en una sola figura, con el eje Y normalizado. Esto permite ver claramente que Bitcoin ha tenido el mayor crecimiento, seguido por el S&P 500, el oro y, finalmente, la oferta monetaria M2. También se crea un gráfico con plotly que utiliza un segundo eje Y para representar el precio del Bitcoin, que tiene una escala mucho mayor, lo que evita que las otras series sean invisibles. El fondo del gráfico se establece en un color verde claro (D7F3ED) para mejorar la estética.
