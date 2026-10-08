# 🧱 LEGO Set Explorer | De datos a una experiencia interactiva de productos

**Business Intelligence | Power BI · Power Query · DAX · Análisis de Productos**

## 1. 📊 Contexto y problema de negocio

LEGO cuenta con un extenso catálogo de sets dirigidos a consumidores de diferentes edades, intereses y presupuestos. Cada producto posee características como su temática, precio, número de piezas y edad recomendada.

Sin embargo, cuando existe una gran cantidad de productos, explorar y comparar estas características puede resultar complicado si la información únicamente se encuentra disponible en tablas convencionales.

El desafío de este proyecto consistió en transformar un dataset de productos LEGO en una herramienta visual que facilitara la exploración del catálogo y permitiera identificar las características de los diferentes sets.

### Preguntas de negocio

- ¿Cuántos sets componen el catálogo analizado?
- ¿Cuáles son las temáticas y grupos disponibles?
- ¿Cuál es el precio promedio de los productos?
- ¿Cómo varían los precios según la temática y las características de los sets?
- ¿Qué opciones existen para determinados rangos de edad y presupuesto?
- ¿Cómo facilitar que un usuario encuentre productos específicos sin revisar manualmente toda la información?

**Problema central:** convertir un catálogo de productos en una herramienta interactiva que simplificara la búsqueda, comparación y exploración de sets LEGO.

---

## 2. 🎯 Objetivo y estrategia de análisis

El objetivo principal fue desarrollar un dashboard interactivo en Power BI que permitiera explorar los sets LEGO mediante sus principales características, ofreciendo una experiencia de consulta intuitiva y organizada.

Para resolver este problema, estructuré el proyecto en cinco etapas:

1. **Exploración:** comprender la estructura del dataset e identificar las variables relevantes.
2. **Preparación:** limpiar, transformar y organizar la información mediante Power Query.
3. **Modelado:** establecer las variables y clasificaciones necesarias para facilitar la exploración.
4. **Indicadores:** desarrollar medidas DAX para resumir las características generales del catálogo.
5. **Visualización:** construir un dashboard con filtros interactivos, indicadores e información detallada de los productos.

La estrategia consistió en transformar los datos de un catálogo convencional en una interfaz que permitiera a los usuarios encontrar y comparar productos de manera sencilla.

---

## 3. 🧰 Tecnologías utilizadas

| Herramienta | Aplicación |
|---|---|
| Power BI Desktop | Desarrollo del dashboard interactivo |
| Power Query | Preparación, limpieza y transformación de datos |
| DAX | Creación de medidas e indicadores |
| Modelado de datos | Organización de las variables utilizadas en el dashboard |
| Visualizaciones interactivas | Exploración y comparación del catálogo |
| Bookmarks | Restablecimiento de filtros y navegación |

---

## 4. 🔎 Desarrollo del proyecto

### Etapa 1. Exploración y comprensión del dataset

**Problema:** la información del catálogo debía organizarse para identificar qué variables podían utilizarse en los indicadores, filtros y elementos visuales.

Comencé revisando la estructura del dataset `lego_sets`, identificando las características que describían los productos.

Las principales variables de interés fueron:

- Nombre e identificación de los sets.
- Temática y grupo temático.
- Precio de venta.
- Edad mínima recomendada.
- Cantidad de piezas.
- Información visual de los productos.

**Acciones realizadas:**

- Exploración de columnas y tipos de datos.
- Identificación de variables relevantes para el análisis.
- Revisión de valores faltantes.
- Evaluación de los campos necesarios para construir las visualizaciones.
- Identificación de posibles clasificaciones para segmentar los productos.

**Resultado:** se definió la estructura de información necesaria para construir una herramienta de exploración basada en las características del catálogo.

### Etapa 2. Preparación y transformación de datos

**Problema:** algunos campos del dataset requerían ajustes para ser utilizados correctamente en cálculos, segmentaciones y elementos visuales.

Utilicé Power Query para preparar la información antes de desarrollar el dashboard.

**Trabajo realizado:**

- Revisión y ajuste de tipos de datos.
- Eliminación de columnas innecesarias para el objetivo del análisis.
- Tratamiento de valores faltantes según el uso de cada variable.
- Organización de campos descriptivos y numéricos.
- Preparación de variables para filtros y visualizaciones.
- Creación de clasificaciones por rangos de edad y precio.

Estas transformaciones permitieron organizar los productos mediante criterios útiles para los usuarios.

**Resultado:** se obtuvo una estructura de datos preparada para realizar cálculos agregados y explorar los sets mediante diferentes características.

### Etapa 3. Desarrollo de indicadores con DAX

**Problema:** mostrar los registros individuales no era suficiente para comprender las características generales del catálogo.

Para resolverlo, desarrollé medidas DAX destinadas a resumir información relevante sobre los productos.

| KPI | Objetivo |
|---|---|
| Total Sets | Contabilizar los sets disponibles |
| Total Groups | Identificar el número de grupos temáticos |
| Avg. Age | Calcular la edad recomendada promedio |
| Avg. Price | Obtener el precio promedio de los sets |
| Avg. Pieces | Calcular el número promedio de piezas por set |

Las medidas fueron incorporadas al dashboard mediante tarjetas para que los usuarios pudieran consultar los indicadores principales.

Además, los valores podían actualizarse según el contexto de filtros aplicado, facilitando el análisis de segmentos específicos.

**Resultado:** el dashboard permitió pasar de una consulta individual de productos a una visión resumida y dinámica del catálogo.

### Etapa 4. Diseño del dashboard interactivo

**Problema:** un catálogo extenso puede dificultar la búsqueda de productos cuando no existen herramientas para segmentar y visualizar sus características.

Por ello, desarrollé una interfaz interactiva que permitiera a los usuarios explorar el catálogo según sus preferencias.

**Elementos implementados:**

**1. Indicadores generales**

Tarjetas para visualizar el número de sets, grupos temáticos, edad promedio, precio promedio y cantidad promedio de piezas.

**2. Filtros interactivos**

Segmentadores para explorar productos según:

- Temática.
- Grupo temático.
- Edad recomendada.
- Rango de precios.
- Cantidad de piezas.

**3. Catálogo de productos**

Una tabla visual con información de los sets para facilitar la consulta de las características de cada producto.

**4. Información visual**

Incorporación de imágenes e información descriptiva para mejorar la identificación de los productos.

**Resultado:** se desarrolló una herramienta de exploración que permite encontrar sets LEGO bajo diferentes criterios, sin necesidad de revisar manualmente todo el dataset.

### Etapa 5. Experiencia de usuario y navegación

**Problema:** al combinar varios filtros, el usuario podía perder la configuración inicial del dashboard o necesitar restablecer manualmente las selecciones.

Para mejorar la experiencia, incorporé un botón de limpieza de filtros utilizando Bookmarks de Power BI.

**Acciones realizadas:**

- Configuración de un estado inicial del reporte.
- Creación de un marcador para restablecer las selecciones.
- Incorporación de un botón interactivo.
- Prueba de la funcionalidad del botón dentro del dashboard.

**Resultado:** el usuario puede regresar a la vista inicial de forma rápida, facilitando la exploración de diferentes combinaciones de productos.

---

## 5. 📈 Resultados y hallazgos

### Resultado 1. Centralización de la información del catálogo

El proyecto permitió organizar diferentes características de los productos en una misma interfaz visual.

En lugar de consultar únicamente una tabla de datos, el usuario puede visualizar indicadores generales y consultar los sets de acuerdo con sus necesidades.

**Valor:** simplificación de la exploración del catálogo y acceso más directo a la información.

### Resultado 2. Segmentación de productos por características

La incorporación de filtros permitió explorar los sets considerando distintos criterios, como edad recomendada, precio, temática y número de piezas.

**Valor:** facilitar la búsqueda de productos que se ajusten a determinadas preferencias o restricciones presupuestarias.

### Resultado 3. Indicadores dinámicos para comparar segmentos

Las medidas DAX permiten resumir las características de los productos disponibles bajo los filtros seleccionados.

Por ejemplo, al seleccionar una temática específica, es posible consultar el precio promedio o la cantidad promedio de piezas correspondiente al segmento.

**Valor:** facilitar comparaciones entre grupos de productos sin realizar cálculos manuales.

### Resultado 4. Mejora funcional de la experiencia de exploración

La incorporación de imágenes, filtros y un botón de restablecimiento permitió desarrollar una interfaz más cómoda para explorar el catálogo.

**Valor:** una experiencia más accesible que la consulta directa de registros en una tabla convencional.

### Alcance de los hallazgos

El proyecto demuestra la construcción de una solución interactiva de exploración de productos.

No obstante, el dataset no permite afirmar por sí solo que el dashboard haya incrementado las ventas, reducido costos o mejorado la conversión comercial.

Para medir estos efectos sería necesario implementar la herramienta en un entorno real y recopilar métricas de uso y desempeño.

---

## 6. ✅ Validación y confiabilidad del análisis

Durante el desarrollo del dashboard se realizaron revisiones de los datos y de los elementos interactivos.

| Control | Propósito |
|---|---|
| Tipos de datos | Garantizar que precios, edades y piezas puedan utilizarse en cálculos |
| Valores faltantes | Evitar que los campos incompletos afecten la interpretación |
| Clasificación de productos | Revisar la coherencia de los rangos de edad y precio |
| Medidas DAX | Comprobar el comportamiento de los indicadores con distintos filtros |
| Segmentadores | Verificar que los elementos visuales respondan a las selecciones |
| Catálogo visual | Comprobar la presentación de las características de los productos |
| Botón de limpieza | Verificar que el reporte regrese al estado configurado |

### Evidencia del trabajo

El archivo de Power BI permite examinar:

- Las transformaciones aplicadas en Power Query.
- Las medidas DAX utilizadas para construir los indicadores.
- Los filtros y sus interacciones.
- La tabla de productos.
- Las visualizaciones.
- La configuración del marcador de restablecimiento.

**Consideración:** para documentar formalmente la exactitud de los cálculos sería conveniente comparar los resultados de las medidas DAX con agregaciones independientes realizadas sobre el dataset original.

---

## 7. 💡 Conclusiones y recomendaciones

El proyecto permitió transformar información de un catálogo de productos en una herramienta interactiva desarrollada con Power BI.

La principal aportación fue facilitar la exploración de los sets LEGO mediante indicadores, filtros y elementos visuales que permiten consultar información según diferentes características.

### Conclusiones principales

**1. La organización de los datos facilita su utilización.**

Preparar adecuadamente los campos y clasificar los productos permitió desarrollar segmentaciones que mejoran la exploración del catálogo.

**2. Los indicadores agregados complementan la información individual.**

Medidas como el precio promedio, la edad recomendada y la cantidad de piezas permiten obtener una visión general del conjunto de productos.

**3. La interactividad aporta valor a la visualización.**

La posibilidad de filtrar y restablecer selecciones convierte al dashboard en una herramienta de consulta, más allá de una presentación estática de gráficos.

**4. El diseño debe responder a las necesidades del usuario.**

Organizar indicadores, filtros y detalles del producto en una sola interfaz permite simplificar la búsqueda de información relevante.

### Recomendaciones de mejora

Como posibles extensiones del proyecto, propongo:

- Incorporar comparaciones de precio por pieza para estudiar diferencias entre productos.
- Crear rankings de sets por precio, cantidad de piezas o grupos temáticos.
- Añadir más detalles del producto y enlaces al catálogo.
- Incorporar datos de ventas para analizar demanda e ingresos por temática.
- Medir el uso del dashboard si se implementa en un entorno comercial.

### Valor aportado

El principal valor del proyecto fue desarrollar una solución de Business Intelligence orientada a la exploración de productos.

Desde el punto de vista técnico, permitió aplicar habilidades de transformación de datos, creación de medidas DAX, diseño de reportes y configuración de interacciones.

Desde una perspectiva de negocio, ofrece una herramienta que podría apoyar tareas de consulta, comparación y presentación de productos dentro de un catálogo comercial.

---

## 8. 📁 Recursos del proyecto

**Dataset**

- `lego_sets` — información de los sets LEGO analizados.

**Dashboard**

- Archivo de Power BI (`.pbix`).
- Indicadores generales del catálogo.
- Segmentadores interactivos.
- Tabla de productos.
- Imágenes y detalles de los sets.
- Botón para limpiar filtros.

### Vista previa

*Insertar aquí una captura del dashboard final.*

### Acceso al proyecto

*Agregar enlace al archivo `.pbix` o a la publicación de Power BI, si está disponible.*

---

## 👨‍💻 Autor

**Manuel Eduardo Solís Vega**

Data Analyst Jr. | Python · SQL · Power BI · Business Intelligence

Proyecto desarrollado como parte de mi portafolio profesional, enfocado en preparación de datos, diseño de dashboards y desarrollo de soluciones interactivas para la exploración de productos.
