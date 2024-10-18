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

La disminución de las ventas en 2020 es considerable, lo que hace notable el impacto de la pandemia en las operaciones de la empresa. La concentración de ventas en 'Ventas Externas' nos indica que la mayor parte de los ingresos vienen de contratos o fuera de las sedes físicas, lo que podría ser una oportunidad, pero también un riesgo, porque depende de una fuente muy concentrada. La fuerte caída en 2020 indica la necesidad de evaluar estrategias, sea reducción de costos, ventas de la empresa o búsqueda de nuevos mercados.

<img src="Análisis de Cantidad.jpg" alt="Análisis de Cantidad">

**Datos Clave**:

* Cantidad Total de Elementos Vendidos: 317 mil elementos.
* Cantidad Vendida por Sede: Las sedes más productivas son **Calle 80** (81 mil elementos) y **Ventas Externas** (74 mil elementos).
* Cantidad Vendida por Año: La cantidad de elementos vendidos también muestra una caída importante en 2020, bajando a 22 mil elementos comparado con los 93 mil en 2019.

Este dashboard confirma la correlación entre ventas en USD y cantidad de elementos vendidos. La caída en 2020 es un claro reflejo de la reducción de demanda o capacidad operativa, posiblemente causada por restricciones relacionadas
con la pandemia. La empresa debería enfocarse en diversificar o mejorar las operaciones en las sedes con menor desempeño o buscar formas de aprovechar la ventaja que tienen con 'Calle 80' y 'Ventas Externas'.

<img src="Análisis de Servicios.jpg" alt="Análisis de Servicios">

**Datos Clave**:

* Servicios Realizados: 88 mil servicios en total.
* Ganancia de Servicios: $2.59 millones (en USD).
* Facturación de Servicios por Sede: **Grandes Flotas** es la sede más rentable en cuanto a servicios, con $1.9 millones en facturación.
* Servicios por Año: La cantidad de servicios realizados fueron bastante estables entre 2017 y 2019, pero como en los anteriores dashboards, esto cae en 2020.

El impacto de la pandemia también se refleja en la reducción de servicios realizados en 2020. Aunque el volumen total de servicios se mantuvo más estable que las ventas, los servicios parecen no contribuir significativamente al total de ingresos. **Grandes Flotas** es un punto fuerte para la empresa. Esto nos dice que podría valer la pena explorar oportunidades de expansión o mejorar la capacidad de la sede.

<img src="Sedes y Empleados.jpg" alt="Sedes y Empleados">

**Datos Clave**:

* Ventas Totales por Sede en cada Rubro, Familia y Servicio: Como vimos en los anteriores análisis, sabemos que **Ventas Externas**, **Grandes Flotas** y **Calle 80** son los que más contribuyeron a las ventas totales de la empresa.
* Cantidad de Sedes: Teniendo en cuenta el punto anterior, son solo 3 de 7 sedes las que contribuyen principalmente.
* Ventas de cada Empleado: **Esteban Damico** es el empleado que más ventas le generó a la empresa con un total de ventas de $14.3 millones, seguido por **Julian Quevedo** ($4.1 millones) y **Juan Pastran** ($1.3 millones). El resto de empleados no superan el millón en ventas.

Habiendo una cantidad significativa de empleados, la empresa podría pensar en acudir a la dicisión de reducción de personal si es que se tiene que llegar a ese punto de acción. En el caso de las sedes con menor rendimiento, se podrían tomar 3 decisiones: Venderlas, cerrarlas o replicar las operaciones de las sedes que si contribuyen significativamente en la ganancia total de la empresa.

## Impacto de la Pandemia:

El impacto de la pandemia es claro: la empresa sufrió una caída considerable de ventas y cantidad de elementos vendidos en 2020, lo que pone en peligro su viabilidad si no se toman medidas. La empresa dependio mucho de "Ventas Externas" y, auqnue "Grandes Flotas" tiene un buen desempeño con los servicios, no es suficiente para compensar la caída general.

### Opciones para la Empresa:

* Venta de la Empresa: La caída en 2020 puede indicar que la empresa no tiene la capacidad para soportar más tiempo sin cambios significativos. Si los costos fijos y operativos siguen altos, vender la empresa podría ser una opción viable para no llegar a la quiebra.
* Buscar Inversores: Otra opción sería buscar inversores para financiar una expansión internacional o para mejorar las operaciones en las sedes con mejor desempeño. Invertir para la mejora de los servicios y expandir las iperaciones en las principales sedes podría estabilizar los ingresos.
* Mantener la Empresa: Si la empresa tiene suficiente capital de trabajo o acceso a financiamento, podría intentar mantener las operaciones y reducir costos mientras las ventas se recuperan post-pandemia. La contra de esto es que dependería mucho de que tan rápido el mercado automotriz vuelva a la normalidad.

## Franquicias.

Como sabemos, la empresa está bajo un modelo de franquicias pero esto no cambia significativamente los análisis que vimos. Pero, hay algunas consideraciones que podrían influir en la toma de decisiones.

1. Desempeño de las Franquicias Individuales: En un modelo de franquicias, cada sede puede ser operada por diferentes propietarios (franquiciados), lo que podría explicarnos las diferencias en el desempeño entre las sedes. En este caso, la empresa podría hacer foco a las franquicias con mejor funcionamiento y analizar qué prácticas o estrategias están usando.
2. Oprotunidades de Expansión: Si algunas sedes están mostrando ser más rentables, esto podría ser la oportunidad de expander el negocio ofreciendo nuevas franquicias en otras ubicaciones. Si el modelo de franquicias demostró ser resiliente, la empresa podría atraer inversores interesados en adquirir nuevas franquicias o expandir las actuales.
3. Vender la empresa: Como analizamos anteriormente, se podrían vender solo las franquicias de bajo desempeño o replicar operaciones. Esto permitiría a los franquiciados más rentables seguir operando mientra que la empresa puede enfocarse en su núcleo más fuerte.
4. Inversores: También se pueden buscar inversores ya que el modelo de franquicias puede ser un atractivo importante, porque ofrece una estrucutra establecida y comprobada, lo que podría facilitar la expanción. La empresa también podría ofrecer soporte adicional a los franquiciados para mejorar la consistencia y calidad en las operaciones en base a las sedes más rentables.

## Analisis Final:

La empresa tiene que evaluar seriamente la búsqueda de inversores o la venta de la empresa, debido a que la caída en 2020 pone en riesgo su viabilidad. Si la empresa opta por seguir operando, la clave está en enfocarse en las sedes más rentables y en mejorar las operaciones en servicios.
