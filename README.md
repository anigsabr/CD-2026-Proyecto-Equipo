#  Predicción de Deserción Estudiantil

## 1. Descripción del Problema
La deserción de estudiantes en el primer año universitario genera un impacto académico y económico crítico. La detección de alumnos en riesgo suele ser tardía, cuando ya han reprobado asignaturas clave. Este proyecto desarrolla un modelo analítico para identificar de forma temprana a los estudiantes con alta probabilidad de abandono durante las primeras semanas de clases. Los tomadores de decisiones son las Direcciones de Carrera y los coordinadores de acompañamiento académico. Su resolución permitirá desplegar tutorías preventivas personalizadas, mejorando la retención estudiantil en un 15% y optimizando la asignación de becas de apoyo.

## 2. Preguntas Analíticas

### Pregunta 1: ¿Qué factores de ingreso e interacciones iniciales influyen en el riesgo de deserción del primer semestre?
* **Variable objetivo:** Condición de deserción al finalizar el primer semestre (Binario: 1 = Desertó, 0 = Continuó).
* **Variables predictoras:** Promedio de enseñanza media, puntaje de ingreso, tipo de establecimiento de origen, porcentaje de asistencia a inductivos y nivel socioeconómico.

### Pregunta 2: ¿Cuál es la probabilidad de abandono de un estudiante según su rendimiento en el primer hito de evaluación?
* **Variable objetivo:** Estado de matrícula en el segundo año (Binario: 1 = Inactivo/Desertado, 0 = Activo).
* **Variables predictoras:** Promedio de notas en primer parcial, entregas a tiempo en aula virtual, asistencia a clases y uso de servicios de biblioteca.

## 3. Relación del Proyecto con CRISP-DM

| Fase | ¿Cómo se aplicaría en su proyecto?  |
| :--- | :--- |
| **Business Understanding** | Definición del problema de retención estudiantil, identificación de directores de carrera como clientes y establecimiento de la meta de reducción de deserción. |
| **Data Understanding** | Exploración de registros académicos históricos, perfiles de ingreso y registros de asistencia para verificar calidad de datos y distribuciones. |
| **Data Preparation** | Limpieza de valores nulos en fichas de ingreso, codificación de variables categóricas y estandarización de calificaciones. |
| **Modeling** | Entrenamiento de algoritmos de clasificación (Regresión Logística, Árboles de Decisión, Random Forest) para predecir el riesgo de abandono. |
| **Evaluation** | Validación de modelos usando métricas como *Recall* y *F1-Score* para priorizar la detección correcta de verdaderos estudiantes en riesgo. |
| **Deployment** | Creación de un panel o reporte automatizado para enviar alertas tempranas al equipo de tutorías académicas antes del segundo parcial. |

#  Predicción y Optimización de Ventas en Supermercados

## 1. Descripción del Problema
La alta variabilidad en la demanda de productos dentro de las sucursales de supermercados genera constantes quiebres de stock y pérdidas económicas por vencimiento de productos. Actualmente, las decisiones de reabastecimiento se toman según promedios históricos manuales, sin considerar el impacto de promociones, estacionalidad o días festivos. Este proyecto busca desarrollar un modelo predictivo para estimar la demanda semanal por categoría de producto. Los tomadores de decisiones son la Gerencia de Operaciones y los Jefes de Logística y Abastecimiento. Resolver esta problemática permitirá optimizar las órdenes de compra a proveedores, reduciendo la merma en un 20% y asegurando la disponibilidad de stock en góndola.

## 2. Preguntas Analíticas

### Pregunta 1: ¿Cuáles son los factores de mayor impacto en el volumen de ventas semanales por categoría de producto?
* **Variable objetivo:** Ventas semanales totales en monto/unidades (Continua).
* **Variables predictoras:** Precio unitario, porcentaje de descuento aplicado, ubicación de la sucursal, día de la semana, presencia de feriados y condiciones climáticas.

### Pregunta 2: ¿Cuál es la probabilidad de que una sucursal experimente un quiebre de stock durante un fin de semana o feriado?
* **Variable objetivo:** Evento de quiebre de stock en góndola (Binario: 1 = Ocurrió quiebre, 0 = Stock suficiente).
* **Variables predictoras:** Nivel de inventario inicial, rotación histórica de la categoría, tipo de promoción activa y afluencia estimada de clientes.

## 3. Relación del Proyecto con CRISP-DM

| Fase | ¿Cómo se aplicaría en su proyecto? |
| :--- | :--- |
| **Business Understanding** | Definición de los objetivos de la gerencia de operaciones: minimizar la merma de inventario y evitar pérdidas por falta de producto en días de alta demanda. |
| **Data Understanding** | Análisis exploratorio de las transacciones históricas de ventas, registros de inventario diario y calendarios promocionales para validar la consistencia de los datos. |
| **Data Preparation** | Limpieza de inconsistencias en registros de caja, manejo de valores nulos y creación de variables temporales (mes, día festivo, indicador de fin de semana). |
| **Modeling** | Implementación de modelos de regresión y algoritmos de machine learning (como Random Forest o XGBoost) para la predicción de series de tiempo de ventas. |
| **Evaluation** | Evaluación del desempeño de los modelos utilizando métricas de error como MAE (Error Absoluto Medio) y RMSE para comparar contra el método tradicional. |
| **Deployment** | Creación de una herramienta de consulta o dashboard para los jefes de compras que alerte oportunamente la necesidad de reabastecimiento por sucursal. |
