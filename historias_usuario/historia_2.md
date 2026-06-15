# Historia de Usuario 2: Alertas de Stock Mínimo (Reabastecimiento)

### Descripción
**Como** Emprendedor Local,  
**Quiero** recibir una alerta visual automática cuando la cantidad de un artículo sea igual o menor a su límite configurado,  
**Para** evitar la pérdida de ventas por desabastecimiento de productos populares.

---

### Criterios de Aceptación (Enfoque SQA)

#### Escenario 1: Activación visual de la alerta por stock bajo.
* **Dado que** un producto llamado "Camiseta Negra" tiene un stock mínimo configurado de 5 unidades,
* **Cuando** se registra una venta que reduce el stock actual de 6 unidades a 4 unidades,
* **Entonces** el sistema debe cambiar el estado del producto a "Bajo Stock", pintando la fila o el indicador del producto en color de advertencia, y añadirlo al panel principal de "Alertas Pendientes".

#### Escenario 2: Desactivación de la alerta tras reabastecimiento.
* **Dado que** un producto se encuentra con la alerta activa de "Bajo Stock",
* **Cuando** el emprendedor edita el producto e incrementa el inventario superando el límite de stock mínimo establecido,
* **Entonces** la alerta visual debe desaparecer automáticamente y el estado del producto debe cambiar a "Abastecido".