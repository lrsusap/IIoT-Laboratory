
# Registro de Decisiones de Ingeniería — Laboratorio IIoT

## 1. Propósito

Este directorio contiene los registros de decisiones
de arquitectura e ingeniería del Laboratorio IIoT.

Su objetivo es conservar la trazabilidad de las decisiones
técnicas relevantes durante el diseño, implementación,
integración y evolución del proyecto.

## 2. Metodología ADR

Se utilizarán Architecture Decision Records (ADR)
para documentar decisiones significativas.

Cada ADR deberá contener:

- Identificador.
- Título.
- Fecha.
- Estado.
- Contexto y problema.
- Alternativas consideradas.
- Decisión adoptada.
- Justificación técnica.
- Consecuencias y riesgos.
- Componentes afectados.
- Referencias y evidencias.

## 3. Estados de una decisión

- PROPUESTA: pendiente de evaluación.
- ACEPTADA: decisión aprobada.
- IMPLEMENTADA: aplicada en el laboratorio.
- VALIDADA: comprobada mediante pruebas.
- SUSTITUIDA: reemplazada por otra decisión.
- DESCARTADA: no adoptada.

La aceptación documental no implica que una decisión
ya haya sido implementada o validada físicamente.

## 4. Convención de nombres

Los registros seguirán esta estructura:

ADR-0001-titulo-descriptivo.md

Se utilizará numeración consecutiva.

## 5. Decisiones iniciales previstas

| ADR | Decisión |
|-----|----------|
| ADR-0001 | Arquitectura modular del laboratorio |
| ADR-0002 | Selección del ESP32-S3 |
| ADR-0003 | Selección de sensores |
| ADR-0004 | Comunicación MQTT y Edge |
| ADR-0005 | Selección de Orange Pi Zero 2W |
| ADR-0006 | Persistencia mediante PostgreSQL |
| ADR-0007 | Arquitectura de redes OT/IT seguras |
| ADR-0008 | Estrategia de ciberseguridad |
| ADR-0009 | Analítica e IA/ML |
| ADR-0010 | Arquitectura del repositorio GitHub |

Esta tabla representa el índice preliminar.
Cada decisión deberá documentarse individualmente.

## 6. Control de cambios

Los ADR aceptados no se modificarán para ocultar
decisiones anteriores.

Cuando una decisión cambie de manera significativa,
se creará un nuevo ADR que identifique el registro
sustituido y explique el motivo.

## 7. Responsabilidad

Creador y responsable del proyecto:
Lewis Rafael Susa Peñate.

Las decisiones deberán contar con revisión técnica
y conservar las evidencias disponibles.

---

IIoT-Laboratory
Registro de decisiones de ingeniería
