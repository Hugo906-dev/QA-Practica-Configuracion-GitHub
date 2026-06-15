# Historia de Usuario 1: Registro y Control de Productos en el Catálogo

### Descripción
**Como** Emprendedor Local,  
**Quiero** registrar un nuevo producto con su nombre, categoría, stock inicial y nivel mínimo permitido,  
**Para** mantener mi catálogo digital actualizado y organizado.

---

### Criterios de Aceptación (Enfoque SQA)

#### Escenario 1: Registro exitoso de un producto con datos válidos.
* **Dado que** el usuario se encuentra en el formulario de "Agregar Producto",
* **Cuando** ingresa un nombre válido, selecciona una categoría, define un stock inicial mayor a cero y un precio de venta válido,
* **Y** presiona el botón "Guardar Producto",
* **Entonces** el sistema debe registrar el producto en la base de datos, mostrar un mensaje de éxito "Producto registrado correctamente" y reflejarlo inmediatamente en la tabla del catálogo.

#### Escenario 2: Intento de registro con campos obligatorios vacíos o datos inválidos.
* **Dado que** el usuario está en el formulario de "Agregar Producto",
* **Cuando** deja el campo "Nombre del Producto" vacío o introduce un valor de stock negativo,
* **Y** presiona el botón "Guardar Producto",
* **Entonces** el sistema debe impedir el envío, resaltar los campos erróneos en rojo y mostrar un mensaje de error específico.