Análisis de Prueba A/B para Optimización de Interfaz en Comercio Electrónico

Descripción del Proyecto
Este proyecto consistió en el análisis de una prueba A/B realizada por una tienda en línea internacional, con el objetivo de evaluar la efectividad de una nueva interfaz que incluía un sistema de recomendaciones. Aunque la prueba fue abandonada parcialmente, se nos proporcionaron los datos para realizar una evaluación completa de su impacto. El análisis cubrió el periodo del 7 de diciembre de 2020 al 1 de enero de 2021.

Objetivos
    * Verificar la calidad e integridad de los datos: duplicados, nulos y tipos de datos.
    * Evaluar la equidad entre los grupos de prueba y control.
    * Analizar el comportamiento de los usuarios en las diferentes etapas del embudo de conversión.
    * Comparar la conversión entre la interfaz original y la interfaz con recomendaciones.
    * Aplicar una prueba estadística (prueba Z) para determinar si las diferencias observadas son significativas.

Metodología
Utilicé Python y librerías como pandas, numpy, seaborn, plotly, scipy y statsmodels para realizar un análisis exploratorio y evaluar la validez de la prueba A/B. El trabajo incluyó:

    - Limpieza de datos: conversión de fechas, detección de valores nulos y duplicados, y depuración de usuarios presentes en ambos grupos.
    - Creación de embudos de conversión para visualizar el comportamiento en cada etapa: login, vista de producto, carrito y compra.
    - Cálculo de métricas clave (tasa de conversión, coeficientes de variación).
    - Comparación gráfica de los grupos A y B.
    - Aplicación de una prueba Z para contrastar las conversiones entre interfaces.

Conclusiones
    * Distribución desigual de usuarios y eventos: El grupo A tenía una participación significativamente mayor en la prueba de recomendaciones (14215 eventos frente a 3979 en grupo B).

    * Conversión más alta con la interfaz tradicional:

        * En el grupo de control, la interfaz tradicional superó a la interfaz con recomendaciones en la conversión en todas las etapas clave (hasta 7.23% más en “purchase”).
        * En el grupo de prueba, la interfaz tradicional también mostró mejores resultados (hasta 12.39% más en “product_page”).

    * No se encontró una diferencia estadísticamente significativa entre los grupos, según la prueba Z (valor p = 0.099), por lo que no se rechaza la hipótesis nula.

    * Recomendación: No continuar con la implementación del sistema de recomendaciones, ya que no demostró mejoras en la conversión y puede resultar contraproducente.

Lenguajes y herramientas principales
    - Python (pandas, numpy, matplotlib, seaborn, plotly, scipy, statsmodels)
    - Jupyter Notebook para documentación del análisis
    - Prueba Z de proporciones para validación estadística

Este análisis proporcionó una evaluación robusta de una prueba A/B incompleta, ayudando a tomar decisiones informadas sobre la dirección del producto y estrategias de optimización en el sitio web.