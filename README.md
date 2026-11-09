
# Laboratorio IIoT | IIoT-Laboratory

**Plataforma experimental de Mantenimiento Inteligente,
Telecomunicaciones y Ciberseguridad Industrial**

**Industria 4.0 | Transformación Digital Industrial | IIoT**

> Del activo al dato, del dato a la decisión.

## 1. Descripción

IIoT-Laboratory es un proyecto experimental y multidisciplinario
de ingeniería orientado al diseño, implementación y validación
de tecnologías de Industria 4.0 aplicadas al monitoreo de
condición y a la gestión inteligente de activos.

El caso de estudio principal es un conjunto motor-bomba.

El laboratorio integra adquisición de señales, sistemas
embebidos, comunicaciones industriales, computación Edge,
supervisión, persistencia de datos, ciberseguridad OT/IT
y analítica avanzada.

El proyecto se desarrolla progresivamente y distingue las
capacidades implementadas de las planificadas.

## 2. Objetivo general

Diseñar, implementar y validar una plataforma experimental
IIoT que permita adquirir, transmitir, almacenar, procesar
y analizar datos de condición de activos industriales,
mediante una infraestructura de comunicaciones segura
y tecnologías de analítica orientadas al mantenimiento.

## 3. Áreas de ingeniería

- Gestión de mantenimiento y activos físicos.
- Electrónica, instrumentación y sensórica.
- Sistemas embebidos e Internet Industrial de las Cosas.
- Redes y telecomunicaciones industriales.
- Ciberseguridad y convergencia OT/IT.
- Ingeniería de datos e inteligencia artificial.
- Transformación Digital Industrial e Industria 4.0.

## 4. Caso de estudio

Activo principal: conjunto motor-bomba.

Variables consideradas:
- Temperatura mediante PT100 y MAX31865.
- Aceleración triaxial mediante ADXL355.
- Variables eléctricas mediante PZEM-004T.

La interpretación de vibración, el establecimiento de
umbrales y la predicción de fallas requieren procedimientos
de procesamiento y validación específicos.

## 5. Arquitectura funcional

Motor-bomba
    |
Sensores y acondicionamiento
    |
ESP32-S3
    |
Wi-Fi / MQTT
    |
Orange Pi Zero 2W
    |
+-- HMI de supervisión
|
+-- Almacenamiento PostgreSQL
      |
      +-- Power BI
      |
      +-- Python / IA / ML

Infraestructura transversal:
- Segmentación y control de redes OT/IT.
- Gestión de identidades y accesos.
- Firewall y monitorización.
- IDS/IPS, SIEM y honeypots.
- Calidad del dato y trazabilidad.
- Gestión de riesgos y continuidad.

## 6. Fases del proyecto

| Fase | Alcance |
|------|---------|
| 1 | Sensado y adquisición |
| 2 | Comunicaciones y Edge |
| 3 | Supervisión y persistencia |
| 4 | Analítica e indicadores |
| 5 | IA/ML y mantenimiento predictivo |

La ciberseguridad, gestión de activos, calidad y continuidad
son requisitos transversales a las cinco fases.

## 7. Tecnologías

Hardware:
ESP32-S3, Orange Pi Zero 2W, PT100, MAX31865,
ADXL355, PZEM-004T y HMI VIEWE.

Software y servicios:
Arduino IDE, LVGL, Mosquitto, Node-RED,
PostgreSQL, Power BI y Python.

Tecnologías objetivo de redes y seguridad:
OpenWrt, Open vSwitch, OPNsense, Suricata,
Wazuh, Zabbix/Nagios y T-Pot.

La inclusión de una herramienta no implica su instalación
ni validación.

## 8. Estado del proyecto

Estado: desarrollo e integración progresivos.

La adquisición y las comunicaciones cuentan con pruebas
documentadas. Existen configuraciones y mediciones que
requieren nueva verificación.

Persistencia histórica, analítica predictiva y
ciberseguridad integral:
implementación o validación pendiente.

Consultar la Guía Técnica v6.1 y los registros de pruebas
para determinar el estado de cada subsistema.

## 9. Documentación

- docs/master-guide/: guía técnica de referencia.
- docs/architecture/: arquitectura física y lógica.
- docs/decisions/: decisiones de ingeniería.
- docs/procedures/: instalación y puesta en servicio.
- tests/: procedimientos y evidencias de validación.

## 10. Seguridad

No se deben publicar credenciales, claves privadas,
configuraciones reales sensibles ni información que
exponga la infraestructura del laboratorio.

Consultar SECURITY.md.

Las pruebas ofensivas y los honeypots se ejecutarán
únicamente en entornos autorizados y aislados.

## 11. Contribuciones

Consultar CONTRIBUTING.md para conocer los requisitos
de documentación, pruebas y revisión de cambios.

## 12. Licenciamiento

Consultar LICENSE y LICENSES/README.md.

Los materiales de terceros conservarán sus licencias
y condiciones originales.

## 13. Principio de ingeniería

Una capacidad no se considerará validada por aparecer
en un diagrama, un código fuente o una pantalla.

Su aceptación requiere pruebas, evidencia y trazabilidad.

---

IIoT-Laboratory | Proyecto de ingeniería aplicada

Autoría y dirección del proyecto

Creador y desarrollador principal: Lewis Rafael Susa Peñate

Perfil profesional:

- Ingeniero Industrial.
- Ingeniero de Sistemas.
- Tecnólogo Naval en Electromecánica.
- Especialista en Seguridad Informática.
- Especialización en Redes de Telecomunicaciones.
- Formación de posgrado en Internet de las Cosas (IoT).

**Rol en el proyecto:** Fundador, diseñador de la arquitectura, responsable de la integración tecnológica y director del desarrollo experimental del Laboratorio IIoT.

**GitHub:** [@lrsusap](https://github.com/lrsusap)

El Laboratorio IIoT es una iniciativa independiente de ingeniería aplicada, concebida y desarrollada para integrar conocimientos de mantenimiento industrial, gestión de activos, telecomunicaciones, ciberseguridad e Internet Industrial de las Cosas.

Su propósito es promover la experimentación, la investigación aplicada y el desarrollo de soluciones tecnológicas alineadas con la Transformación Digital Industrial y la Industria 4.0, Mantenimiento 4.0.

El proyecto podrá incorporar contribuciones de terceros, conservando la trazabilidad y el reconocimiento de sus respectivas aportaciones.
