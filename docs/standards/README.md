
# Normas, Estándares y Buenas Prácticas
## Laboratorio IIoT — IIoT-Laboratory

**Proyecto:** Laboratorio IIoT  
**Creador y responsable:** Lewis Rafael Susa Peñate  
**Versión del documento:** 1.0  
**Fecha:** 2026-11-09  
**Estado:** Marco normativo de referencia  
**Guía técnica de referencia:** Versión 6.1  

---

## 1. Propósito

Establecer el marco normativo y metodológico de referencia
para el diseño, gestión, implementación, operación,
verificación y evolución del Laboratorio IIoT.

El laboratorio integra tecnologías y conocimientos de:

- Ingeniería de mantenimiento y gestión de activos.
- Instrumentación y sistemas embebidos.
- Internet Industrial de las Cosas (IIoT).
- Redes y telecomunicaciones industriales.
- Ciberseguridad OT/IT.
- Ingeniería y analítica de datos.
- Inteligencia artificial y aprendizaje automático.
- Gestión de proyectos.
- Gestión de riesgos y continuidad operacional.
- Transformación Digital Industrial e Industria 4.0.

Las normas se aplicarán de manera proporcional al alcance,
riesgo y madurez de cada subsistema.

**La utilización de una norma como referencia no implica
certificación ni conformidad integral con sus requisitos.**

---

## 2. Objetivos del marco normativo

1. Establecer referencias técnicas y metodológicas.
2. Relacionar requisitos con componentes del laboratorio.
3. Orientar decisiones de ingeniería.
4. Promover seguridad desde el diseño.
5. Mejorar confiabilidad, disponibilidad y calidad.
6. Estandarizar procedimientos y registros.
7. Facilitar la gestión de riesgos y cambios.
8. Garantizar trazabilidad de pruebas y resultados.
9. Apoyar la gestión y seguimiento del proyecto.
10. Promover la mejora continua y la reproducibilidad.

---


## 3. Gestión y Dirección de Proyectos

### 3.1 Referencias normativas y metodológicas

| Referencia | Edición | Aplicación |
|------------|---------|------------|
| ISO 21500 | 2021 | Contexto y conceptos de gestión de proyectos, programas y portafolios |
| ISO 21502 | 2020 | Directrices para la gestión de proyectos |
| PMBOK Guide - PMI | 8.ª edición, 2025 | Principios, dominios de desempeño, prácticas y entrega de valor |
| The Standard for Project Management - PMI | 2025 | Fundamentos y principios de dirección de proyectos |

### 3.2 Aplicación al Laboratorio IIoT

La gestión del proyecto considerará:

- Definición de objetivos, alcance y entregables.
- Estructura de Desglose del Trabajo (EDT/WBS).
- Planificación y control del cronograma.
- Gestión de costos y presupuestos.
- Gestión de recursos y adquisiciones.
- Identificación y gestión de interesados.
- Gobierno y toma de decisiones.
- Gestión de riesgos y oportunidades.
- Gestión de calidad.
- Gestión de comunicaciones.
- Seguimiento del desempeño.
- Control integrado de cambios.
- Entrega de valor y beneficios esperados.
- Cierre de fases y lecciones aprendidas.

### 3.3 Dominios de desempeño del PMBOK

Se considerarán los siete dominios de desempeño
presentados en la octava edición:

1. Gobernanza.
2. Alcance.
3. Cronograma.
4. Finanzas.
5. Interesados.
6. Recursos.
7. Riesgos.

Los dominios se aplicarán proporcionalmente a la
complejidad y madurez del Laboratorio IIoT.

### 3.4 Enfoque metodológico

El proyecto podrá combinar prácticas predictivas,
adaptativas e híbridas.

Se utilizará planificación estructurada para
arquitectura, adquisición de hardware, instalación
y puesta en servicio.

Para firmware, software, analítica y experimentación,
podrán utilizarse ciclos iterativos de desarrollo,
pruebas y mejora.

### 3.5 Integración con GitHub

| Herramienta | Aplicación |
|-------------|------------|
| GitHub Issues | Actividades, incidencias y mejoras |
| GitHub Projects | Planificación y seguimiento |
| Milestones | Hitos y entregables |
| Pull Requests | Revisión e integración |
| Releases | Versiones y entregas |
| ADR | Decisiones de ingeniería |
| CHANGELOG.md | Historial de modificaciones |

### 3.6 Documentación de gestión

Directorio:

`docs/project-management/`

Se desarrollarán progresivamente:

- Acta de constitución del proyecto.
- Definición de alcance.
- EDT/WBS.
- Cronograma e hitos.
- Presupuesto y recursos.
- Registro de riesgos.
- Registro de interesados.
- Plan de comunicaciones.
- Plan de calidad.
- Control de cambios.
- Seguimiento y desempeño.
- Lecciones aprendidas.

### 3.7 Criterios de aplicación

Las referencias ISO y PMI serán utilizadas como
marcos complementarios y adaptadas al alcance
experimental del laboratorio.

Su aplicación no implica certificación ni
conformidad integral con los estándares.

Los resultados deberán sustentarse mediante
documentación, indicadores y evidencias.

---

## 4. Gestión de mantenimiento y activos

### 4.1 Referencias

| Norma | Aplicación |
|-------|------------|
| ISO 55000 | Conceptos, principios y terminología de gestión de activos |
| ISO 55001 | Requisitos del sistema de gestión de activos |
| ISO 14224 | Recopilación e intercambio de datos de confiabilidad y mantenimiento |
| ISO 17359 | Directrices de monitoreo de condición y diagnóstico |
| ISO 20816 | Evaluación de vibraciones mecánicas según la parte aplicable |
| ISO 50001 | Gestión y mejora del desempeño energético |

### 4.2 Aplicación al laboratorio

- Identificación y caracterización del motor-bomba.
- Registro de información del activo.
- Definición de variables de condición.
- Identificación de modos de falla.
- Análisis de causas y consecuencias.
- Monitoreo de parámetros operacionales.
- Evaluación de tendencias de degradación.
- Indicadores de disponibilidad y confiabilidad.
- Seguimiento del desempeño energético.
- Apoyo a decisiones de mantenimiento.
- Evolución hacia mantenimiento predictivo.

### 4.3 Consideraciones técnicas

El ADXL355 entrega mediciones de aceleración.

La magnitud vectorial medida incluye la contribución
de la gravedad cuando corresponda.

No deberá interpretarse directamente como velocidad
de vibración mecánica expresada en mm/s.

Los procedimientos de procesamiento, filtrado,
conversión, evaluación y establecimiento de límites
deberán justificarse y validarse.

---

## 5. Instrumentación y sistemas embebidos

### 5.1 Referencias técnicas

Se utilizarán las especificaciones oficiales de:

- ESP32-S3.
- ADXL355.
- MAX31865.
- PT100.
- PZEM-004T.
- Pantallas HMI utilizadas.
- Interfaces eléctricas y módulos asociados.

### 5.2 Interfaces consideradas

- SPI.
- I2C.
- UART.
- GPIO.
- ADC, cuando corresponda.
- Interfaces de comunicación inalámbrica.

### 5.3 Criterios de ingeniería

- Compatibilidad eléctrica.
- Alimentación y niveles lógicos.
- Protección de interfaces.
- Integridad y acondicionamiento de señales.
- Frecuencia y resolución de muestreo.
- Exactitud, precisión y sensibilidad.
- Calibración o contrastación.
- Tratamiento de ruido e interferencias.
- Detección de fallas de adquisición.
- Trazabilidad y calidad de las mediciones.

Las hojas de datos no sustituyen las pruebas físicas
ni la verificación de los módulos realmente utilizados.

---

## 6. Internet Industrial de las Cosas

### 6.1 Ámbitos de referencia

- Arquitectura de dispositivos IIoT.
- Adquisición y procesamiento local.
- Computación Edge.
- Interoperabilidad.
- Mensajería y transporte de datos.
- Gestión de dispositivos.
- Identificación y autenticación.
- Seguridad de comunicaciones.
- Calidad y trazabilidad de la información.

### 6.2 Arquitectura funcional

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
Supervisión y persistencia
    |
Analítica e IA/ML
    |
Información para decisiones de mantenimiento

Los componentes no implementados deberán identificarse
expresamente como arquitectura objetivo.

---

## 7. Redes y telecomunicaciones industriales

### 7.1 Referencias

| Norma o protocolo | Aplicación |
|-------------------|------------|
| IEEE 802.3 | Ethernet |
| IEEE 802.11 | Redes inalámbricas |
| IEEE 802.1Q | VLAN |
| TCP/IP | Arquitectura de comunicaciones |
| MQTT | Mensajería publish/subscribe |
| Modbus | Comunicación industrial |
| TLS | Protección de comunicaciones |
| DNS | Resolución de nombres |
| DHCP | Asignación dinámica de direcciones |
| NTP | Sincronización horaria |

### 7.2 Aplicaciones previstas

- Diseño físico y lógico de red.
- Planificación de direccionamiento IPv4.
- Segmentación por VLAN.
- Enrutamiento entre segmentos autorizados.
- Control de acceso mediante ACL.
- Separación de zonas OT/IT.
- Seguridad inalámbrica.
- Monitoreo del tráfico.
- Medición de latencia y jitter.
- Análisis de pérdida de paquetes.
- Disponibilidad y recuperación de servicios.
- Evaluación de QoS cuando sea necesario.

### 7.3 Tecnologías consideradas

- OpenWrt.
- Open vSwitch.
- Switch Ethernet gestionable.
- Herramientas de diagnóstico de red.
- Wireshark.
- Servicios de monitoreo.

Se distinguirán las soluciones virtuales de los
dispositivos físicos requeridos para la implementación.

---

## 8. Ciberseguridad industrial OT/IT

### 8.1 Referencias

| Norma o marco | Aplicación |
|---------------|------------|
| IEC 62443-2-1 | Programa de seguridad para sistemas IACS |
| IEC 62443-3-2 | Riesgos, zonas y conductos |
| IEC 62443-3-3 | Requisitos de seguridad del sistema |
| IEC 62443-4-1 | Desarrollo seguro de productos |
| IEC 62443-4-2 | Requisitos técnicos de componentes |
| NIST SP 800-82 | Seguridad de tecnología operacional |
| NIST CSF 2.0 | Gestión de riesgos de ciberseguridad |
| ISO/IEC 27001 | Sistema de gestión de seguridad de la información |
| ISO/IEC 27002 | Controles de seguridad |
| ISO/IEC 27005 | Gestión de riesgos de seguridad de la información |

### 8.2 Principios de diseño

- Security by Design.
- Defense in Depth.
- Mínimo privilegio.
- Denegación predeterminada.
- Segmentación de red.
- Gestión de identidades.
- Control de accesos.
- Endurecimiento de sistemas.
- Gestión de vulnerabilidades.
- Monitoreo y registro de eventos.
- Respuesta a incidentes.
- Recuperación y continuidad.

### 8.3 Tecnologías previstas

| Tecnología | Función |
|------------|---------|
| OPNsense | Firewall y control perimetral |
| Suricata | IDS/IPS |
| Snort | IDS/IPS y evaluación comparativa |
| Wazuh | SIEM/XDR |
| T-Pot | Plataforma de honeypots |
| Zabbix | Monitoreo de infraestructura |
| Nagios Core | Monitoreo de servicios |
| Zeek | Análisis de tráfico de red |

Las tecnologías previstas no se declararán operativas
sin instalación, configuración, pruebas y evidencias.

### 8.4 Seguridad operacional

Las pruebas de ciberseguridad deberán ejecutarse
únicamente en entornos propios o autorizados.

Los honeypots se desplegarán en redes aisladas,
sin acceso iniciado hacia los sistemas OT.

Los controles de seguridad deberán diseñarse
evitando interferencias no controladas con la
adquisición y supervisión del activo.

---

## 9. Gestión de riesgos y continuidad

### 9.1 Referencias

| Norma | Aplicación |
|-------|------------|
| ISO 31000 | Gestión de riesgos |
| ISO 22301 | Gestión de continuidad del negocio |
| ISO 9001 | Gestión de calidad |

### 9.2 Aplicación al laboratorio

- Identificación de riesgos técnicos.
- Análisis de probabilidad y consecuencias.
- Evaluación y tratamiento de riesgos.
- Gestión de cambios.
- Control documental.
- Protección de la disponibilidad.
- Respaldo y restauración de configuraciones.
- Recuperación de servicios.
- Pruebas de continuidad.
- Seguimiento de acciones correctivas.
- Mejora continua.

La pérdida de comunicaciones o de servicios
analíticos no deberá detener innecesariamente
la adquisición local de datos.

---

## 10. Ingeniería y analítica de datos

### 10.1 Ámbitos de aplicación

- Adquisición y almacenamiento.
- Calidad y procedencia de datos.
- Integridad temporal.
- Validación de registros.
- Limpieza de datos.
- Tratamiento de valores ausentes.
- Estadística descriptiva.
- Estadística inferencial.
- Ingeniería de características.
- Análisis de tendencias.
- Indicadores de condición.

### 10.2 Tecnologías consideradas

- PostgreSQL.
- SQLite.
- Node-RED.
- Python.
- Jupyter Notebook.
- Google Colab.
- Power BI.

### 10.3 Requisitos de trazabilidad

Cada conjunto de datos deberá identificar:

- Origen.
- Activo y dispositivo.
- Variables y unidades.
- Método de adquisición.
- Frecuencia de muestreo.
- Marcas temporales.
- Tratamientos aplicados.
- Estado de calidad.
- Limitaciones conocidas.

Los datasets sintéticos deberán distinguirse
explícitamente de los datos reales.

---

## 11. Inteligencia artificial y aprendizaje automático

### 11.1 Referencias

| Norma o marco | Aplicación |
|---------------|------------|
| ISO/IEC 42001 | Gestión de sistemas de inteligencia artificial |
| NIST AI RMF | Gestión de riesgos relacionados con IA |

### 11.2 Aplicaciones previstas

- Detección de anomalías.
- Clasificación de condiciones.
- Análisis de degradación.
- Identificación de patrones.
- Pronóstico de variables.
- Evaluación de modelos predictivos.

### 11.3 Buenas prácticas

- Separación de datos de entrenamiento y prueba.
- Validación adecuada para series temporales.
- Prevención de fuga de información.
- Control de calidad de datasets.
- Comparación de algoritmos.
- Reproducibilidad de experimentos.
- Evaluación de generalización.
- Seguimiento del desempeño del modelo.
- Registro de limitaciones y supuestos.

Los resultados obtenidos con datasets sintéticos
no demostrarán por sí solos capacidad predictiva
sobre el motor-bomba real.

---

## 12. Transformación Digital Industrial e Industria 4.0

### 12.1 Alcance

El Laboratorio IIoT constituye una plataforma
experimental alineada con los principios de
Transformación Digital Industrial e Industria 4.0.

### 12.2 Tecnologías habilitadoras

- Sensórica inteligente.
- Sistemas embebidos.
- IIoT.
- Computación Edge.
- Convergencia OT/IT.
- Redes industriales seguras.
- Persistencia de datos.
- Analítica avanzada.
- Inteligencia artificial.
- Mantenimiento inteligente.

### 12.3 Cadena de valor

Magnitud física
    |
Adquisición
    |
Digitalización
    |
Comunicación
    |
Persistencia
    |
Procesamiento y análisis
    |
Información
    |
Decisiones de mantenimiento

### 12.4 Criterio de madurez

La alineación con Industria 4.0 no significa que
todas las tecnologías estén implementadas.

La madurez deberá evaluarse mediante:

- Capacidades efectivamente instaladas.
- Integración entre subsistemas.
- Resultados de pruebas.
- Disponibilidad y confiabilidad.
- Calidad de datos.
- Seguridad de comunicaciones.
- Uso de información para decisiones.
- Evidencias de mejora.

---

## 13. Matriz de aplicabilidad normativa

Se desarrollará el documento:

`standards-applicability-matrix.md`

Cada referencia deberá registrar:

| Campo | Descripción |
|-------|-------------|
| ID | Identificador |
| Norma | Referencia técnica |
| Edición | Año o versión aplicable |
| Organismo | Entidad responsable |
| Dominio | Área de ingeniería |
| Requisito | Criterio relevante |
| Componente | Elemento relacionado |
| Riesgo | Riesgo asociado |
| Control | Medida prevista |
| Evidencia | Registro verificable |
| Estado | Situación de aplicación |

La selección final de requisitos se realizará
según su aplicabilidad al laboratorio.

---

## 14. Estados de aplicación

Se utilizarán los siguientes estados:

- REFERENCIA: norma identificada.
- EN EVALUACIÓN: aplicabilidad en estudio.
- APLICABLE: criterios relevantes identificados.
- PLANIFICADO: implementación definida.
- IMPLEMENTADO: control o actividad ejecutada.
- VERIFICADO: resultado comprobado con evidencia.
- NO APLICABLE: exclusión justificada.

El estado VERIFICADO no representa certificación
ni conformidad integral con la norma.

---

## 15. Organización documental futura

Este directorio podrá incorporar:

- standards-applicability-matrix.md
- project-management.md
- maintenance-and-asset-management.md
- instrumentation-and-iiot.md
- industrial-networks.md
- ot-cybersecurity.md
- risk-and-continuity.md
- data-analytics-and-ai.md
- industry-4.0-alignment.md

Los archivos se crearán cuando resulte necesario
desarrollar su contenido técnico.

---

## 16. Control documental y versiones

Toda referencia normativa deberá identificar,
cuando corresponda:

- Edición utilizada.
- Fecha de consulta o revisión.
- Alcance de aplicación.
- Requisitos relevantes.
- Cambios frente a versiones anteriores.
- Impacto sobre el laboratorio.

Las actualizaciones de normas deberán evaluarse
antes de modificar configuraciones, procedimientos
o criterios de aceptación.

---

## 17. Derechos de autor y distribución

No se publicarán copias completas de normas
protegidas por derechos de autor sin autorización.

El repositorio podrá contener:

- Referencias bibliográficas.
- Enlaces a fuentes oficiales.
- Matrices originales de aplicabilidad.
- Análisis técnicos propios.
- Procedimientos desarrollados para el laboratorio.

Los materiales de terceros conservarán sus
licencias y condiciones de uso.

Consultar:

`../../LICENSES/README.md`

---

## 18. Responsabilidad y referencia

**Creador y responsable:**
Lewis Rafael Susa Peñate.

**Repositorio:**
https://github.com/lrsusap/IIoT-Laboratory

**Documento técnico principal:**
Guía Técnica del Laboratorio IIoT — Versión 6.1.

**Estado:**
Marco normativo de referencia en desarrollo progresivo.

---

**IIoT-Laboratory**  
*Del activo al dato, del dato a la decisión.*
