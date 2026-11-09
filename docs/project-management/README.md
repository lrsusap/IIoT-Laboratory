
# Gestión del Proyecto — Laboratorio IIoT

## 1. Identificación

**Proyecto:** IIoT-Laboratory

**Denominación:** Plataforma Experimental de
Mantenimiento Inteligente, Telecomunicaciones
y Ciberseguridad Industrial.

**Creador y responsable:**
Lewis Rafael Susa Peñate.

**Enfoque metodológico:** Híbrido.

**Referencias:**
- ISO 21500:2021.
- ISO 21502:2020.
- PMBOK Guide, 8.ª edición (2025).
- The Standard for Project Management (PMI, 2025).

**Estado:** En desarrollo progresivo.

## 2. Propósito

Establecer el marco para dirigir, planificar,
ejecutar, monitorear, controlar y cerrar
los trabajos del Laboratorio IIoT.

La gestión del proyecto busca asegurar
coherencia entre alcance, tiempo, recursos,
costos, calidad, riesgos y resultados.

## 3. Objetivo de gestión

Coordinar el desarrollo e integración de los
subsistemas del laboratorio mediante prácticas
predictivas y adaptativas, manteniendo
trazabilidad técnica, gestión de riesgos
y criterios verificables de aceptación.

## 4. Enfoque híbrido

### 4.1 Gestión predictiva

Se aplicará principalmente a:

- Definición de arquitectura.
- Alcance y requisitos.
- Estructura de Desglose del Trabajo.
- Selección de hardware.
- Presupuesto y adquisiciones.
- Instalación física.
- Comisionamiento.
- Hitos y entregables.
- Seguridad eléctrica y operacional.

### 4.2 Gestión adaptativa

Se aplicará principalmente a:

- Firmware ESP32-S3.
- Interfaces HMI.
- Integración MQTT.
- Flujos Node-RED.
- Automatización y scripts.
- Configuraciones de servicios.
- Experimentos de redes y seguridad.
- Analítica de datos.
- Modelos de inteligencia artificial.

Los desarrollos adaptativos utilizarán
ciclos de planificación, implementación,
prueba, revisión y mejora.

### 4.3 Integración híbrida

Ambos enfoques se coordinarán mediante:

- Plan general del proyecto.
- Backlog priorizado.
- Hitos de integración.
- Gestión de dependencias.
- Control de configuraciones.
- Gestión de riesgos.
- Control integrado de cambios.
- Verificación de entregables.
- Documentación de decisiones.

## 5. Diferencia entre gestión y fases técnicas

El laboratorio contempla cinco fases técnicas:

1. Sensado y adquisición.
2. Comunicaciones y Edge.
3. Supervisión y persistencia.
4. Analítica e indicadores.
5. IA/ML y mantenimiento predictivo.

Estas fases representan la arquitectura de
implementación tecnológica.

La dirección del proyecto comprende procesos
de inicio, planificación, ejecución,
seguimiento, control y cierre.

Ambas estructuras se vincularán mediante
la EDT/WBS, los entregables, hitos y criterios
de aceptación.

## 6. Organización documental

| Directorio | Responsabilidad |
|------------|-----------------|
| initiation/ | Acta de constitución y justificación |
| planning/ | Alcance, EDT, cronograma y recursos |
| execution/ | Coordinación y desarrollo |
| monitoring-control/ | Indicadores, riesgos y cambios |
| closure/ | Aceptación y lecciones aprendidas |

## 7. Instrumentos de gestión

Se desarrollarán progresivamente:

- Acta de constitución del proyecto.
- Definición de alcance.
- Registro de requisitos.
- EDT/WBS.
- Cronograma e hitos.
- Presupuesto.
- Plan de recursos.
- Registro de interesados.
- Plan de comunicaciones.
- Registro de riesgos.
- Plan de calidad.
- Plan de adquisiciones.
- Registro de cambios.
- Informes de seguimiento.
- Registro de lecciones aprendidas.

## 8. Gestión mediante GitHub

### Issues
Registro de actividades, incidencias,
requisitos, riesgos y mejoras.

### Projects
Visualización y seguimiento del trabajo
mediante tableros y campos de control.

### Milestones
Agrupación de entregables e hitos.

### Pull Requests
Revisión técnica e integración de cambios.

### Releases
Publicación de versiones del laboratorio.

### ADR
Documentación de decisiones de ingeniería.

## 9. Ciclo de trabajo adaptativo

Cada iteración podrá seguir:

1. Seleccionar actividades del backlog.
2. Definir criterios de aceptación.
3. Identificar dependencias y riesgos.
4. Desarrollar la solución.
5. Ejecutar pruebas.
6. Revisar resultados.
7. Documentar evidencias.
8. Integrar cambios aceptados.
9. Actualizar el backlog.

La duración de las iteraciones se establecerá
según las características del trabajo.

## 10. Gobernanza y responsabilidades

El creador y responsable del laboratorio
dirige las decisiones de alcance, arquitectura,
priorización y aceptación.

Las contribuciones externas deberán cumplir
los requisitos de documentación, seguridad,
licenciamiento y validación del repositorio.

Las decisiones significativas se registrarán
mediante ADR.

## 11. Gestión de riesgos

Se identificarán y evaluarán riesgos
relacionados con:

- Seguridad eléctrica.
- Integridad de mediciones.
- Compatibilidad de hardware.
- Fallas de comunicación.
- Disponibilidad de servicios.
- Ciberseguridad OT/IT.
- Calidad de datos.
- Integración de subsistemas.
- Recursos y presupuesto.
- Cambios de alcance.
- Dependencias tecnológicas.

Los tratamientos deberán ser proporcionales
a la criticidad de cada riesgo.

## 12. Gestión de calidad

Cada entregable deberá contar con:

- Requisitos documentados.
- Criterios de aceptación.
- Pruebas aplicables.
- Evidencias verificables.
- Registro de incidencias.
- Control de versiones.
- Aprobación correspondiente.

La finalización de una tarea de desarrollo
no equivale necesariamente a la validación
integral del subsistema.

## 13. Gestión de cambios

Las modificaciones relevantes deberán:

1. Identificar su justificación.
2. Evaluar impacto técnico.
3. Evaluar riesgos.
4. Estimar recursos y esfuerzo.
5. Revisar dependencias.
6. Obtener aprobación.
7. Ejecutar y verificar.
8. Actualizar documentación.

## 14. Seguimiento y desempeño

Se definirán indicadores de:

- Avance de entregables.
- Cumplimiento de hitos.
- Actividades completadas.
- Incidencias abiertas y resueltas.
- Pruebas ejecutadas.
- Porcentaje de aceptación.
- Cambios de alcance.
- Riesgos pendientes.
- Disponibilidad de recursos.
- Desviaciones de cronograma y costos.

Los indicadores deberán basarse en
información verificable.

## 15. Control de versiones

Se diferenciarán:

- Versión documental de la Guía Técnica.
- Versiones de firmware y software.
- Versiones de configuraciones.
- Versiones integradas del laboratorio.
- Versiones de documentación de gestión.

Las modificaciones deberán mantener
trazabilidad mediante Git.

## 16. Criterios de cierre

Una etapa o entregable se considerará
cerrado cuando:

- Cumpla sus criterios de aceptación.
- Exista evidencia suficiente.
- Sus incidencias estén tratadas.
- La documentación esté actualizada.
- Los cambios estén registrados.
- El responsable haya aprobado el resultado.

## 17. Documentación relacionada

- ../master-guide/
- ../architecture/
- ../decisions/
- ../procedures/
- ../standards/

Documentos generales:

- ../../README.md
- ../../CHANGELOG.md
- ../../CONTRIBUTING.md
- ../../SECURITY.md

## 18. Principio de gestión

La planificación orienta el trabajo,
la experimentación genera conocimiento
y la evidencia determina la aceptación.

---

**IIoT-Laboratory**

*Del activo al dato, del dato a la decisión.*
