
# Ingeniería y Gestión de Datos — Laboratorio IIoT

## 1. Propósito

Documentar la arquitectura, adquisición,
transmisión, persistencia, calidad, seguridad,
trazabilidad y utilización de los datos
del Laboratorio IIoT.

Este directorio contiene documentación técnica.

Los datasets, esquemas de bases de datos,
consultas y recursos de implementación
se almacenarán en el directorio /data/.

## 2. Alcance

La gestión de datos comprende:

- Identificación de fuentes.
- Adquisición de mediciones.
- Estructuración de registros.
- Transporte de información.
- Validación de datos.
- Persistencia e históricos.
- Calidad e integridad.
- Seguridad y control de acceso.
- Preparación para analítica.
- Retención y recuperación.
- Trazabilidad y reproducibilidad.

## 3. Fuentes de datos

### 3.1 Motor-bomba

Las fuentes principales previstas son:

| Dispositivo | Variables |
|-------------|-----------|
| PT100 + MAX31865 | Temperatura y medición RTD |
| ADXL355 | Aceleración en ejes X, Y, Z |
| PZEM-004T | Variables eléctricas |

Las variables derivadas deberán documentar
su procedimiento de cálculo, unidades
y condiciones de validez.

### 3.2 Infraestructura IIoT

También podrán registrarse datos relacionados con:

- Estado de dispositivos.
- Disponibilidad de servicios.
- Calidad de comunicación.
- Eventos MQTT.
- Desconexiones y reconexiones.
- Rendimiento de red.
- Eventos de ciberseguridad.

Los registros de seguridad y operación deberán
mantener una clasificación apropiada.

### 3.3 Datasets externos

Se podrán utilizar conjuntos de datos de referencia,
como MetroPT3, para desarrollar y verificar
procedimientos de analítica.

Su procedencia y licenciamiento deberán identificarse.

Los datos externos no se presentarán como mediciones
del motor-bomba del laboratorio.

## 4. Arquitectura de datos

La cadena funcional prevista es:

Magnitud física
    |
Sensor y acondicionamiento
    |
ESP32-S3
    |
Validación y estructuración
    |
MQTT / TCP-IP
    |
Mosquitto / Orange Pi
    |
Node-RED
    |
Persistencia
    |
PostgreSQL
    |
Analítica y visualización
    |
Información para decisiones

Esta arquitectura representa el objetivo del sistema.

Cada tramo deberá identificarse como propuesto,
implementado o validado según sus evidencias.

## 5. Modelo de datos

Los registros deberán contemplar, según corresponda:

- Identificador del activo.
- Identificador del dispositivo.
- Variable medida.
- Valor.
- Unidad.
- Marca temporal.
- Calidad del dato.
- Estado de comunicación.
- Versión de firmware.
- Método de adquisición.
- Estado de procesamiento.

Se definirán contratos de datos para los mensajes
MQTT y esquemas para el almacenamiento.

## 6. Calidad del dato

Los procedimientos deberán evaluar:

- Completitud.
- Validez.
- Consistencia.
- Integridad.
- Exactitud, cuando pueda verificarse.
- Unicidad.
- Oportunidad.
- Coherencia temporal.
- Trazabilidad.

Se documentará el tratamiento de:

- Valores ausentes.
- Registros duplicados.
- Mediciones fuera de rango.
- Datos desactualizados.
- Errores de conversión.
- Fallas de sensores.
- Pérdida de comunicación.
- Valores atípicos.

La ausencia de comunicación no deberá
interpretarse como condición normal del activo.

## 7. Persistencia

La arquitectura objetivo contempla PostgreSQL
para almacenamiento histórico.

Se documentarán:

- Diseño de tablas.
- Tipos de datos.
- Relaciones y restricciones.
- Índices.
- Consultas.
- Políticas de acceso.
- Copias de seguridad.
- Restauración.
- Retención.
- Integridad de registros.

El despliegue y la validación de PostgreSQL
deberán registrarse por separado.

## 8. Seguridad y privacidad

Los controles previstos incluyen:

- Autenticación y autorización.
- Protección de credenciales.
- Cifrado cuando corresponda.
- Restricción de acceso a bases de datos.
- Segmentación de red.
- Registro de eventos.
- Protección de respaldos.
- Control de modificaciones.
- Publicación de datos autorizados.

Los datos operativos privados y los secretos
no deberán incorporarse al repositorio público.

Consultar SECURITY.md en la raíz.

## 9. Datos para analítica

Los conjuntos de datos utilizados para análisis
deberán incluir:

- Descripción de variables.
- Unidades.
- Procedencia.
- Intervalo temporal.
- Frecuencia de muestreo.
- Transformaciones.
- Criterios de limpieza.
- Limitaciones.
- Condiciones de reutilización.

Los datos sintéticos deberán identificarse
explícitamente como tales.

## 10. Organización documental prevista

- data-architecture.md
- data-dictionary.md
- mqtt-data-contracts.md
- data-quality.md
- database-design.md
- data-security.md
- data-governance.md
- backup-and-recovery.md
- data-retention.md

## 11. Integración con el repositorio

- ../../data/: datasets, esquemas y consultas.
- ../analytics/: metodología analítica.
- ../../analytics/: notebooks y modelos.
- ../architecture/: arquitectura del sistema.
- ../procedures/: procedimientos.
- ../../tests/: pruebas y evidencias.

## 12. Estados de implementación

- PROPUESTO.
- DOCUMENTADO.
- IMPLEMENTADO.
- EN PRUEBAS.
- VALIDADO.
- OBSOLETO.

La existencia de datos almacenados no demuestra
por sí sola su integridad, exactitud ni utilidad
para mantenimiento predictivo.

## 13. Referencias

- Guía Técnica del Laboratorio IIoT v6.1.
- Marco de estándares en docs/standards/.
- Política de seguridad del repositorio.
- Documentación oficial de PostgreSQL y MQTT.

## 14. Responsable

Lewis Rafael Susa Peñate.

---

IIoT-Laboratory
Del activo al dato, del dato a la decisión.
