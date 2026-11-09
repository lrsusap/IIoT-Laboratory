
# Ingeniería y Analítica de Datos — Laboratorio IIoT

## 1. Propósito

Documentar los fundamentos, metodologías,
procedimientos y criterios de validación
de los procesos analíticos del Laboratorio IIoT.

Este directorio contiene documentación técnica.
Los notebooks, scripts y modelos ejecutables
se almacenarán en /analytics/.

## 2. Alcance

- Análisis exploratorio de datos.
- Estadística descriptiva e inferencial.
- Tratamiento de series temporales.
- Limpieza y transformación de datos.
- Ingeniería de características.
- Visualización e interpretación.
- Detección de anomalías.
- Aprendizaje automático.
- Evaluación de modelos predictivos.

## 3. Cadena analítica

Adquisición
    |
Validación de datos
    |
Persistencia
    |
Preparación y limpieza
    |
Análisis exploratorio
    |
Ingeniería de características
    |
Modelado y evaluación
    |
Información para mantenimiento

## 4. Casos de estudio

### MetroPT3

Se utilizará como referencia metodológica
para explorar y analizar registros industriales.

El caso permitirá documentar procedimientos
de estadística descriptiva, visualización
y análisis de variables.

Los datos de MetroPT3 no representan mediciones
del motor-bomba del Laboratorio IIoT.

### Motor-bomba

Se documentarán progresivamente los análisis
realizados con datos adquiridos mediante:

- PT100 + MAX31865.
- ADXL355.
- PZEM-004T.

## 5. Calidad de los datos

Todo procedimiento deberá considerar:

- Procedencia y trazabilidad.
- Variables y unidades.
- Resolución y frecuencia de muestreo.
- Integridad temporal.
- Registros duplicados.
- Valores ausentes.
- Valores atípicos.
- Ruido y errores de medición.
- Condiciones operacionales.
- Transformaciones efectuadas.

## 6. Validación de modelos

Se documentarán:

- Objetivo del modelo.
- Dataset y características.
- División de entrenamiento y prueba.
- Prevención de fuga de información.
- Métricas de evaluación.
- Validación temporal cuando corresponda.
- Limitaciones.
- Reproducibilidad.
- Evidencias de desempeño.

Los resultados obtenidos con datos sintéticos
no demostrarán por sí solos capacidad predictiva
sobre el activo físico real.

## 7. Documentos previstos

- analytics-methodology.md
- exploratory-data-analysis.md
- statistical-analysis.md
- time-series-analysis.md
- feature-engineering.md
- anomaly-detection.md
- predictive-modeling.md
- model-validation.md

## 8. Relación con el repositorio

- ../../analytics/: notebooks y código.
- ../data/: documentación de datos.
- ../../data/: datasets y esquemas.
- ../architecture/: arquitectura.
- ../../tests/: pruebas y evidencias.

## 9. Referencias

- Guía Técnica del Laboratorio IIoT v6.1.
- Marco normativo en docs/standards/.
- Buenas prácticas de analítica reproducible.

## 10. Responsable

Lewis Rafael Susa Peñate.

---

IIoT-Laboratory
Del activo al dato, del dato a la decisión.
