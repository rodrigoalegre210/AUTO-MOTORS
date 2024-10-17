<h1 align="center"> Servicio automotriz "Auto Motors" </h1>

Este proyecto es uno de los retos dentro de la página de [ID for Ideas](https://idforideas.com/), una comunidad que busca ayudar a personas juniors a ganar experiencia profesional dentro del mundo IT.

### Proyecto: Servicio Automotriz "Auto Motors"

"Empresa colombiana con franquicias. Ofrece servicios y productos como cambio de aceite, cambio de filtros, venta de cubiertas, llantas, entre otras."

### Descripción del proyecto.

"Contamos con datos internos de la empresa como ventas y empleados. Requieren analizar el impacto de la pandemia para evaluar si vender la empresa, si quiebra o si salir a buscar inversores para expansión hacia otros paises."

### Objetivo:

"El cliente necesita contar con toda la información ya analizada para tomar una decisión final."

### Indicadores básicos para empezar:

* Venta Total
* Cantidad de Elementos vendidos
* Ganancia Facturación Total de Servicios
* Cantidad de Servicios Ofrecidos
* Cantidad de Sedes o ubicaciones disponibles
* Ventas totales por Sede en cada Rubro o Familia y Servicios
* Ventas realizadas por sus empleados
* Ranking de Ventas / Servicios de Empleados

***Estos puntos son establecidos en el archivo "descripcion.pdf"***

---

### Trabajo Técnico.

#### Problemas con el archivo Ventas.csv

Para realizar el trabajo se usaron los datos Ventas y Empleados, pero los datos de "Ventas" dieron dos problemas:

1. El archivo tenía un total de **921320** valores faltantes.
2. La columna 'Ventas' nos daba un error de formato por las ',' y '.' dentro de Power BI.

Estos problemas se abarcaron dentro del archivo modelado.ipynb, en donde se eliminan las filas tienen valores faltantes en su totalidad y se pasan los valores de la columna 'Ventas' a números limpios.

#### Columnas creadas dentro de Power BI

**Ventas en USD**: Dentro del archivo descripcion.pdf se especifica que para el proyecto nos debemos manejar en dólares estadounidense (0,00023).

**VentasTotales**: Suma total de las ventas.

**GananciaServicios**: Ganancia total de los servicios.

**CantidadServicios**: Cantidad de servicios realizados.

**VentasServicios**: Ventas solo de servicios.

**CantidadSedes**: Suma de la cantidad de sedes.

**VentasPorEmpleados**: Suma de las ventas de empleados (mismo calculo que **'VentasTotales'**)

**RankingVentasEmpleados**: Ranking de las ventas de los empleados.

También se trabajó con la columna 'Fecha' para sacar los años y poder desglozar los gráficos en años.

---

<img src="Análisis de Ventas.jpg" alt="Análisis de Ventas">

**Datos Clave**:

* Ventas totales: $25.18 millones (en USD).
* Ventas por Sede: El mayor ingreso proviene de las **Ventas Externas** ($18 millones), en cuanto a las otras sedes, reportan ingresos significativamente menores (de $3 millones para abajo).
* Ventas por Año: Hay una caída importante en 2020, con una disminución a solo $1 millon, frente a los $4.8 millones de 2019.

La disminución de las ventas en 2020 es considerable, lo que hace notable el impacto de la pandemia en las operaciones de la empresa. La concentración de ventas en 'Ventas Externas' nos indica que la mayor parte de los ingresos
vienen de contratos o fuera de las sedes físicas, lo que podría ser una oportunidad, pero también un riesgo, porque depende de una fuente muy concentrada. La fuerte caída en 2020 indica la necesidad de evaluar estrategias, sea 
reducción de costos, ventas de la empresa o búsqueda de nuevos mercados.

<img src="Análisis de Cantidad.jpg" alt="Análisis de Cantidad">

**Datos Clave**:
