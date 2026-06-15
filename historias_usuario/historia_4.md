# Historia de Usuario 4: Dashboard de Reportes Financieros y de Inventario

### Descripción
**Como** Emprendedor Local,  
**Quiero** visualizar un gráfico analítico con los ingresos totales del mes y el valor financiero de mi inventario actual,  
**Para** analizar la salud financiera de mi negocio y planificar mis inversiones de compra de suministros.

---

### Criterios de Aceptación (Enfoque SQA)

#### Escenario 1: Carga y consistencia de los datos del Dashboard.
* **Dado que** el usuario ingresa al módulo de "Reportes y Estadísticas",
* **Cuando** la página termina de cargar de forma completa,
* **Entonces** el sistema debe recuperar las ventas del periodo actual y mostrar de forma clara y dinámica:
  1. El gráfico de barras con los ingresos mensuales.
  2. El listado de los 3 productos más vendidos.
  3. El valor monetario totalizado del inventario en base a la fórmula: Costo Unitario * Cantidad Disponible.