# 📦 FoodHub Order Analysis

## 🧠 Contexto

El número de restaurantes en Nueva York está creciendo rápidamente. Muchos estudiantes y profesionales con agendas ocupadas dependen de estos servicios para alimentarse. En este contexto, **FoodHub** ofrece una solución eficiente: una aplicación móvil que permite a los usuarios realizar pedidos desde múltiples restaurantes, con entrega integrada.

El proceso incluye:
- Confirmación del pedido por el restaurante
- Asignación de un repartidor
- Recogida del pedido
- Entrega al cliente
- Evaluación del servicio por parte del usuario

FoodHub obtiene ingresos cobrando un margen fijo por cada pedido entregado.

---

## 🎯 Objetivo del Proyecto

FoodHub ha recopilado datos de los pedidos realizados por sus clientes registrados. El objetivo de este proyecto es analizar dichos datos para:

- Comprender la demanda según tipo de cocina y restaurante
- Identificar patrones de comportamiento de los clientes
- Evaluar tiempos de preparación y entrega
- Proponer recomendaciones que mejoren la experiencia del usuario y optimicen la operación

---

## 📊 Descripción de los Datos

El conjunto de datos contiene información detallada sobre cada pedido:

| Variable               | Descripción                                                                 |
|------------------------|------------------------------------------------------------------------------|
| `order_id`             | ID único del pedido                                                         |
| `customer_id`          | ID del cliente que realizó el pedido                                        |
| `restaurant_name`      | Nombre del restaurante                                                      |
| `cuisine_type`         | Tipo de cocina solicitada                                                   |
| `cost`                 | Costo total del pedido                                                      |
| `day_of_the_week`      | Día en que se realizó el pedido (weekday o weekend)                         |
| `rating`               | Calificación otorgada por el cliente (escala de 1 a 5)                      |
| `food_preparation_time`| Tiempo (minutos) que tardó el restaurante en preparar el pedido             |
| `delivery_time`        | Tiempo (minutos) que tardó el repartidor en entregar el pedido              |

---

## 🔍 Metodología

El análisis se desarrolló en un notebook de Jupyter e incluyó:

1. **Exploración de la estructura de los datos**  
   Revisión de columnas, tipos de datos, valores faltantes y duplicados.

2. **Análisis univariable**  
   Distribuciones de variables como `cost`, `rating`, `delivery_time`, etc.

3. **Análisis multivariable**  
   Relaciones entre variables como:
   - Tipo de cocina vs. calificación
   - Día de la semana vs. tiempo de entrega
   - Costo vs. tiempo de preparación

4. **Recomendaciones**  
   Se entregaron sugerencias basadas en los hallazgos para mejorar la experiencia del cliente y la eficiencia operativa.

---

## 🛠️ Requisitos

Este proyecto utiliza Python 3.9+ y las siguientes librerías:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `jupyter`

Instala las dependencias con:

```bash
pip install -r requirements.txt