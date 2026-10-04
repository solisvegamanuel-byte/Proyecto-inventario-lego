# LEGO Set Explorer – Power BI Dashboard

## Descripción

Este proyecto consiste en el desarrollo de un dashboard interactivo en Power BI para explorar distintos sets de LEGO y facilitar la búsqueda de productos según criterios como temática, grupo de temática, rango de edad, precio y cantidad de piezas.

El objetivo principal fue construir una herramienta visual que permitiera al usuario filtrar rápidamente el catálogo y consultar la información más relevante de cada set.

---

## Objetivo del proyecto

Crear una herramienta interactiva que permita:

- Explorar diferentes sets de LEGO.
- Filtrar productos por temática.
- Filtrar por grupo de temática.
- Filtrar por rango de edad.
- Filtrar por rango de precio.
- Comparar cantidad de piezas y precio.
- Visualizar información detallada de un set seleccionado.
- Restablecer todos los filtros mediante un botón.

---

## Preparación de los datos

La base de datos original fue revisada y limpiada antes de construir el dashboard.

Durante el proceso se realizaron tareas como:

- Revisión de tipos de datos.
- Análisis de valores nulos.
- Eliminación de registros sin información relevante para el análisis.
- Eliminación de columnas innecesarias.
- Validación de precios.
- Validación de cantidad de piezas.
- Validación de edades mínimas recomendadas.
- Preparación de campos para su uso dentro de Power BI.

También se trabajó previamente con Python y pandas para revisar la estructura del dataset y detectar problemas de calidad en los datos.

---

## Transformaciones realizadas

Dentro de Power Query se realizaron diferentes transformaciones para preparar la información.

### Rango de edad

Se creó una clasificación de edad basada en la edad mínima recomendada:

- 1 a 4
- 5 a 9
- 10 a 17
- Mayor de 18

### Rango de precio

Los sets fueron agrupados en diferentes niveles de precio para facilitar la exploración:

- $
- $$
- $$$
- $$$$
- $$$$$

Esto permite utilizar rangos categóricos además del filtro numérico de precio.

---

## Medidas DAX

Se crearon diferentes medidas para resumir la información del catálogo, entre ellas:

```DAX
Total Sets =
DISTINCTCOUNT(lego_sets[set_id])
