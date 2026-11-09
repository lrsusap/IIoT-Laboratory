
# Procedimientos Técnicos — Laboratorio IIoT

## 1. Propósito

Este directorio reúne los procedimientos técnicos
para instalar, configurar, integrar, verificar,
operar y recuperar los subsistemas del Laboratorio IIoT.

Su finalidad es garantizar que las actividades sean
reproducibles, seguras y técnicamente verificables.

## 2. Alcance

Los procedimientos abarcan:

- Instrumentación y acondicionamiento de señales.
- Sensores y sistemas embebidos.
- Firmware ESP32-S3.
- Pantallas HMI y visualización.
- Computación Edge y Orange Pi Zero 2W.
- MQTT, Mosquitto y Node-RED.
- Redes y telecomunicaciones OT/IT.
- Segmentación, firewall y ciberseguridad.
- Bases de datos y persistencia.
- Analítica, Power BI e IA/ML.
- Diagnóstico, mantenimiento y recuperación.

## 3. Organización prevista

| Directorio | Responsabilidad |
|------------|-----------------|
| installation/ | Instalación de hardware y software |
| configuration/ | Configuración de dispositivos y servicios |
| commissioning/ | Comisionamiento y puesta en servicio |
| integration/ | Integración entre subsistemas |
| operation/ | Operación y supervisión |
| maintenance/ | Mantenimiento y diagnóstico |
| troubleshooting/ | Identificación y solución de fallas |
| recovery/ | Respaldos, restauración y recuperación |
| security/ | Procedimientos de seguridad OT/IT |

Los directorios se crearán cuando existan procedimientos
que deban incorporarse.

## 4. Estructura de un procedimiento

Cada procedimiento deberá contener:

1. Identificador y título.
2. Objetivo.
3. Alcance.
4. Responsable.
5. Requisitos previos.
6. Equipos, instrumentos y herramientas.
7. Condiciones de seguridad.
8. Configuración inicial.
9. Secuencia de actividades.
10. Parámetros y criterios de aceptación.
11. Verificaciones y pruebas.
12. Evidencias requeridas.
13. Posibles fallas y acciones correctivas.
14. Procedimiento de reversión, cuando aplique.
15. Referencias y control de versión.

## 5. Identificación de procedimientos

Se utilizará la siguiente convención:

PROC-[DOMINIO]-[NÚMERO]-[DESCRIPCIÓN].md

Ejemplos:

PROC-HW-001-verificacion-electrica.md

PROC-FW-001-programacion-esp32.md

PROC-NET-001-configuracion-vlan.md

PROC-SEC-001-endurecimiento-mqtt.md

PROC-DATA-001-instalacion-postgresql.md

## 6. Requisitos de seguridad

Antes de ejecutar cualquier procedimiento:

- Identificar los riesgos técnicos y operacionales.
- Verificar el estado del sistema.
- Confirmar los requisitos de alimentación.
- Disponer de respaldo cuando corresponda.
- No publicar credenciales ni claves privadas.
- Evitar cambios no autorizados en redes OT/IT.
- Prever un mecanismo de recuperación.
- Registrar los resultados.

Las intervenciones eléctricas deberán cumplir
las condiciones de seguridad correspondientes.

Las pruebas ofensivas de ciberseguridad se realizarán
exclusivamente en entornos autorizados y aislados.

## 7. Validación

Un procedimiento se considerará validado cuando
haya sido ejecutado bajo condiciones documentadas
y exista evidencia de cumplimiento de sus criterios
de aceptación.

Estados:

- BORRADOR: procedimiento en preparación.
- APROBADO: revisado y autorizado para ejecución.
- EN PRUEBAS: ejecución y verificación en curso.
- VALIDADO: resultados comprobados.
- OBSOLETO: reemplazado por una nueva revisión.

## 8. Evidencias

Las evidencias podrán incluir:

- Fotografías del montaje.
- Mediciones eléctricas.
- Registros de monitor serie.
- Capturas de osciloscopio.
- Registros de comunicación.
- Resultados de pruebas.
- Consultas de bases de datos.
- Eventos de seguridad.
- Configuraciones saneadas.

Los resultados y evidencias se organizarán
en el directorio tests/ del repositorio.

## 9. Trazabilidad

Cada procedimiento deberá relacionarse,
cuando corresponda, con:

- Guía Técnica vigente.
- Documentos de arquitectura.
- ADR aplicables.
- Componentes y versiones.
- Casos de prueba.
- Riesgos y controles.
- Registro de cambios.

## 10. Referencia principal

Guía Técnica del Laboratorio IIoT — Versión 6.1.

Los procedimientos deberán mantener coherencia
con la arquitectura aprobada y diferenciar
las configuraciones propuestas de las validadas.

## 11. Responsable

Creador y responsable del proyecto:

Lewis Rafael Susa Peñate.

---

IIoT-Laboratory
Procedimientos de ingeniería
