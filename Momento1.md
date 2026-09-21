InicioCosteoPrecios
//ENTRADA
definir nombreProducto caracter;
definir costoBase decimal;
definir porcentajeGanancias decimal;
definir ganancias decimal;
definir cons IVA <- 0.19;
definir subtotal decimal;
definir precioFinal decimal;
definir valorImpuesto decimal;
//PROCESO
escribir "ingrese el nombre del producto"
leer nombreProducto;
escribir "ingrese el costo base"
leer costoBase;
escribir "ingrese el Porcentaje de ganancias deseadas"
leer porcentajeGanancias;

ganancias <- costoBase * (porcentajeGanancias / 100);
subtotal <- costoBase + ganancias;
valorImpuesto <- subtotal * IVA;
precioFinal <- subtotal + valorImpuesto;
//SALIDA
escribir "Recibo de venta";
escribir "el costo base del producto" + nombreProducto + "es:" + costoBase;
escribir "tus ganancias del producto" + nombreProducto + "es:" + ganancias;
escribir "el precio subtotal de" + nombreProducto + "es:" + subtotal;
escribir "Precio del IVA es:" + valorImpuesto;
escribir "El valor Final del producto" + nombreProducto + "es:" + precioFinal;

FinCosteoPrecios