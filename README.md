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

**Problema:** la información del catálogo debía
