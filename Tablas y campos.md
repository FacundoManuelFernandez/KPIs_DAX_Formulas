A continuación se detallan los tablas, sus relaciones y las columnas utilizadas en las fórmulas.

TablaTransacciones:
- ID Transaccion: código que identifica unívocamente cada transacción
- Tipo de Transaccion: Venta/Devolución

TablaDescuentos:
- ID Transaccion: código que identifica unívocamente cada transacción
- Tipo de Transaccion: Venta/Devolución
- Estado de descuento: Aplicado/Anulado
- Nombre de descuento: Nombre correspondiente al descuento otorgado.
- '$DescuentoOtorgado': Monto de descuento otorgado (en $)

TablaClasificacionDescuentos:
- Tipo de aplicacion: Automático/Especial
- Tipo de descuento: Club de Beneficios (entre otros).

TablaPagos:
- ID Transaccion: código que identifica unívocamente cada transacción
- Estado de pago: Realizado/Anulado
- '$PagoNeto': Monto pagado (en $)
- Cantidad de cuotas: Cantidad de cuotas en las que se realizó el pago (de acuerdo a la codificación del sistema, que puede no coincidir con la cantidad de cuotas real).

TablaClasificacionCuotas:
- Cuotas Reales: Cantidad de cuotas en las que se pagó realmente.
- Cuotas S/Clasificacion Sistema: Cantidad de cuotas en las que se realizó el pago de acuerdo a la codificación del sistema.

Relaciones entre tablas:

- TablaDescuentos * <-- 1 TablaClasificacionDescuentos [a partir de 'Nombre Descuento']
- TablaDescuentos * <-- 1 TablaTransacciones [a partir de 'ID Transaccion']
- TablaPagos * <-- 1 TablaClasificacionCuotas [a partir de 'Cantidad de Cuotas' y 'Cuotas S/Clasificacion Sistema']
- TablaPagos * <-- 1 TablaTransacciones [a partir de 'ID Transaccion']


