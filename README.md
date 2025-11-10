Este repositorio contiene un conjunto de medidas (KPIs) formuladas en DAX para el análisis de ventas y descuentos. Los indicadores fueron diseñados a medida para analizar y evaluar requerimientos específicos de negocio.

Como criterio de selección se incluyeron métricas que representan distintas formas de medición (ratios, índices, tasas, etc.) sobre diferentes dimensiones (cantidades, montos, proporciones), priorizándose las fórmulas que aportan valor por su complejidad o por patrones de cálculo reutilizables. En ese sentido, para mantener la sobriedad del repositorio no se publicaron medidas redundantes o cuyo código no aportara información novedosa o sustancial. A los fines de facilitar la legibilidad del código, se procuró utilizar en la medida de la posible una cantidad reducida de campos/columnas (empleados bajo distinta lógica de cálculo según cada caso). Cada medida incluye comentarios explicativos que detallan su lógica paso a paso.

Como la construcción de los indicadores responde a necesidades de negocio específicas, su formulación puede variar según el contexto y el modelo de datos. 

Las medidas expuestas son las siguientes (dispuestas en orden alfabético):

1. **Beneficio Promedio por Aplicación Concretada de Club de Beneficios**: mide el monto promedio de beneficio otorgado por los descuentos concretados (aplicados y no anulados) correspondientes al Club de Beneficios.
2. **Cantidad de Ventas con Acumulación de Descuento Club de Beneficios + Otro Descuento**: mide la cantidad de ventas en las que se aplicó simultaneamente un descuento del Club de Beneficios junto con otro descuento distinto.
3. **Distribución interna de descuentos del Club de Beneficios (%)**: mide la proporción del monto total de descuentos del Club que corresponde a cada segmento dentro de este programa.
4. **Índice de rendimiento (monto/pagos concretados) sobre variable "x"**: mide el rendimiento de una variable determinada tomando como referencia la cantidad de pagos que tuvo y su participación sobre el monto total facturado. Un valor superior a 1 indica que, en promedio, los pagos asociados a esa variable tienen montos más altos que el promedio general.
5. **Promedio de Cuotas Concretadas**: mide la cantidad promedio de cuotas correspondiente a los pagos concretados.
6. **Proporción de Ventas con Descuento Automático (%)**: mide la proporción de ventas en las cuales se aplicó un descuento automático sobre el total de ventas registradas.
7. **Ratio de Descuentos Especiales (por c/100 Ventas)**: mide cuántos descuentos especiales se concretan por cada 100 ventas realizadas. 
8. **Tasa de descuentos especiales (sobre descuentos concretados)**: mide la proporción que representan los descuentos especiales sobre la totalidad de los descuentos concretados.

Dentro del repositorio encontrarán la carpeta que contiene las fórmulas de las medidas susodichas y un documento que detalla las tablas y columnas utilizadas junto con el modelo de datos.
