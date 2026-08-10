# Proyecto: Predicción de Deserción Estudiantil

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
