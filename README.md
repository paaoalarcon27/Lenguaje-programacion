# Huellitas Pet Shop - Sistema de Facturación

## Objetivo

Huellitas Pet Shop es una tienda dedicada a la venta de alimentos y productos para perros y gatos.

El objetivo de este proyecto es desarrollar un sistema de facturación en Python que permita registrar las compras de los clientes, calcular subtotales, descuentos, IVA, costos de envío y generar una factura con un número consecutivo.

## Catálogo de productos

| Código | Producto | Precio | IVA |
|---|---|---:|---:|
| P-001 | Concentrado para perro 2 kg | $45.000 | 19% |
| P-002 | Arena para gato 5 kg | $32.000 | 19% |
| P-003 | Collar para perro | $25.000 | 19% |
| P-004 | Shampoo para mascotas | $18.000 | 19% |
| P-005 | Alimento húmedo para gato | $8.000 | 5% |
| P-006 | Medicamento veterinario | $20.000 | 0% |

## Reglas de negocio

### Regla 1: Descuento por valor de compra

Si el valor de la compra antes de IVA es mayor o igual a $100.000, se aplica automáticamente un descuento del 10%.

### Regla 2: Descuento por cantidad

Si el cliente compra 5 o más unidades del mismo producto, se aplica un descuento del 5% sobre ese producto.

### Regla 3: Costo de envío

Si el total de la compra después de aplicar los descuentos es mayor o igual a $150.000, el envío es gratis.

Si el total es menor a $150.000, se cobra un costo de envío de $8.000.

## Funcionamiento del sistema

El sistema permite:

1. Mostrar el catálogo de productos.
2. Buscar productos mediante su código.
3. Registrar las cantidades solicitadas por el cliente.
4. Informar cuando se introduce un código de producto inexistente.
5. Calcular el subtotal de la compra.
6. Aplicar los descuentos establecidos.
7. Calcular el IVA correspondiente a cada producto.
8. Calcular el costo de envío.
9. Generar una factura con número consecutivo.
10. Guardar cada factura como archivo `.txt`.

## Pruebas realizadas

Se realizaron las siguientes pruebas:

- Producto con IVA general del 19%.
- Producto exento de IVA.
- Compra de 5 o más unidades para comprobar el descuento por cantidad.
- Ingreso de un código de producto inexistente.
- Generación de una factura y su archivo `.txt`.
- Generación de dos facturas consecutivas para comprobar el aumento del número de factura.

Todas las pruebas realizadas funcionaron correctamente.

## Archivos del proyecto

- `sistema_facturacion.ipynb`: notebook con el código completo del sistema.
- `factura_1012.txt`: ejemplo de factura generada por el programa.
- `factura_1013.txt`: segundo ejemplo de factura generada por el programa.
- `README.md`: documentación del proyecto.
