
# Gestión de Activos y Mantenimiento — Laboratorio IIoT

## 1. Propósito

Este directorio contiene la documentación técnica
relacionada con los activos físicos utilizados
en el Laboratorio IIoT.

Su objetivo es establecer el contexto operacional,
las condiciones de funcionamiento y los requisitos
de monitoreo, confiabilidad y mantenimiento.

## 2. Activo principal

**Activo:** Conjunto motor-bomba.

**Identificador propuesto:** MOTOR-1.

**Estado:** Caracterización técnica en desarrollo.

Los datos de placa, potencia, velocidad nominal,
fabricante y condiciones de servicio deberán
incorporarse a partir de evidencias físicas.

No se asignarán valores nominales sin
documentación técnica verificable.

## 3. Variables de condición

| Variable | Sensor o dispositivo |
|----------|----------------------|
| Temperatura | PT100 + MAX31865 |
| Aceleración triaxial | ADXL355 |
| Tensión eléctrica | PZEM-004T |
| Corriente eléctrica | PZEM-004T |
| Potencia eléctrica | PZEM-004T |
| Frecuencia eléctrica | PZEM-004T |

La evaluación de vibración mecánica requerirá
procesamiento y validación específicos.

## 4. Gestión de mantenimiento

Se considerarán actividades relacionadas con:

- Identificación y clasificación del activo.
- Definición del contexto operacional.
- Identificación de funciones y fallas funcionales.
- Análisis de modos de falla.
- Monitoreo de condición.
- Definición de indicadores.
- Evaluación de tendencias de degradación.
- Planificación de intervenciones.
- Gestión de riesgos asociados al activo.
- Mejora continua del mantenimiento.

## 5. Referencias técnicas

- ISO 55000 e ISO 55001.
- ISO 14224.
- ISO 17359.
- ISO 20816, según parte aplicable.
- ISO 50001.
- ISO 31000.

Las normas serán utilizadas como referencias
técnicas y metodológicas, sin declarar
certificación ni cumplimiento integral.

## 6. Organización prevista

- motor-pump/: caracterización del conjunto.
- operating-context/: contexto operacional.
- failure-modes/: modos de falla.
- condition-monitoring/: variables y criterios.
- maintenance-plans/: planes de mantenimiento.
- reliability/: indicadores y análisis.
- energy-performance/: desempeño energético.

## 7. Integración con otros subsistemas

La información del activo se relacionará con:

- hardware/: sensores e instrumentación.
- firmware/: adquisición y procesamiento.
- data/: almacenamiento y calidad del dato.
- analytics/: análisis y modelos.
- tests/: pruebas y evidencias.
- docs/: arquitectura y procedimientos.

## 8. Estados de validación

- PROPUESTO: pendiente de evaluación.
- DOCUMENTADO: información registrada.
- IMPLEMENTADO: aplicado en el laboratorio.
- VALIDADO: verificado mediante evidencia.
- OBSOLETO: reemplazado.

## 9. Responsable

Creador y responsable del proyecto:

Lewis Rafael Susa Peñate.

---

IIoT-Laboratory
Gestión de activos y mantenimiento
