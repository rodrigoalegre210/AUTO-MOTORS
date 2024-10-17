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
