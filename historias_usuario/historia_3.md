# Historia de Usuario 3: Registro de Ventas y Descuento de Stock

### Descripción
**Como** Emprendedor Local,  
**Quiero** registrar una venta seleccionando múltiples productos del catálogo y procesando el total,  
**Para** automatizar el cobro al cliente y mantener el stock real al día sin hacer cálculos manuales.

---

### Criterios de Aceptación (Enfoque SQA)

#### Escenario 1: Procesamiento exitoso de una venta multiproducto.
* **Dado que** el usuario se encuentra en el módulo de "Nueva Venta",
* **Cuando** añade 2 unidades del "Producto A" y 1 unidad del "Producto B" al carrito de venta,
* **Y** presiona el botón "Concluir Venta",
* **Entonces** el sistema debe calcular el total sumando los precios unitarios por cantidad, generar un comprobante virtual con un número de transacción único y restar automáticamente las unidades vendidas del stock.

#### Escenario 2: Intento de venta que supera el stock disponible.
* **Dado que** el "Producto C" posee únicamente 3 unidades disponibles en inventario,
* **Cuando** el usuario intenta digitar o incrementar la cantidad a 5 unidades en el carrito de ventas,
* **Entonces** el sistema debe bloquear la acción, lanzar una alerta que diga "Cantidad solicitada supera el stock disponible (Máximo: 3)" e impedir que se complete la venta.