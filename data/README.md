
# Datos y Persistencia — Laboratorio IIoT

**Proyecto:** IIoT-Laboratory  
**Creador y responsable:** Lewis Rafael Susa Peñate  
**Estado:** Implementación progresiva  
**Referencia documental:** Guía Técnica v6.1

---

## 1. Propósito

Este directorio contiene los recursos técnicos
utilizados para estructurar, validar, almacenar,
consultar y preparar los datos del Laboratorio IIoT.

Su objetivo es facilitar la integración entre
los sistemas de adquisición, comunicaciones,
persistencia y analítica.

La documentación metodológica se encuentra en:

`../docs/data/`

## 2. Alcance

El módulo comprende:

- Contratos de datos y mensajes.
- Esquemas de validación.
- Diseño de bases de datos.
- Scripts SQL.
- Migraciones de estructuras.
- Consultas de información.
- Datos sintéticos.
- Datos de ejemplo autorizados.
- Control de calidad.
- Preparación de datasets analíticos.

## 3. Fuentes de información

### 3.1 Motor-bomba

| Fuente | Variables |
|--------|-----------|
| PT100 + MAX31865 | Temperatura, resistencia RTD |
| ADXL355 | Aceleración triaxial |
| PZEM-004T | Tensión, corriente, potencia y frecuencia |
| ESP32-S3 | Estado de adquisición y diagnóstico |

Las mediciones disponibles dependerán de
la integración y validación de cada dispositivo.

### 3.2 Infraestructura digital

Se contempla la adquisición de información sobre:

- Disponibilidad de dispositivos.
- Estado de conectividad.
- Eventos MQTT.
- Estado de servicios Edge.
- Rendimiento de red.
- Eventos de seguridad.
- Estado de bases de datos.

Estos registros deberán clasificarse y
protegerse según su sensibilidad.

### 3.3 Fuentes externas

El laboratorio podrá utilizar datasets
industriales públicos para desarrollar
procedimientos analíticos.

MetroPT3 será uno de los casos de estudio.

Los datasets externos conservarán su
procedencia, atribución y condiciones de uso.

## 4. Arquitectura funcional

La cadena de datos prevista es:

Motor-bomba
    |
Sensores
    |
ESP32-S3
    |
MQTT
    |
Mosquitto / Orange Pi Zero 2W
    |
Node-RED
    |
PostgreSQL
    |
Python / Power BI / IA-ML
    |
Información para mantenimiento

La arquitectura representa el objetivo
de integración y no implica que todos
los tramos estén implementados.

## 5. Organización del directorio

| Directorio | Función |
|------------|---------|
| contracts/ | Estructura y requisitos de mensajes |
| schemas/ | Esquemas de validación |
| postgresql/ | Estructuras, migraciones y consultas SQL |
| sample-data/ | Conjuntos pequeños de ejemplo |
| synthetic/ | Datos generados artificialmente |
| raw/ | Datos originales de trabajo local |
| processed/ | Datos transformados de trabajo local |
| quality/ | Reglas y recursos de validación |

Los subdirectorios se crearán progresivamente
cuando existan archivos que deban incorporarse.

## 6. Contratos de datos

Los contratos definirán, según corresponda:

- Identificador de activo.
- Identificador de dispositivo.
- Identificador de variable.
- Valor medido.
- Unidad.
- Marca temporal.
- Calidad de lectura.
- Estado de adquisición.
- Versión de mensaje.
- Campos opcionales y obligatorios.

Se documentará la correspondencia entre
los mensajes MQTT y las estructuras SQL.

Los ejemplos utilizarán identificadores
y configuraciones ficticias o saneadas.

## 7. Persistencia PostgreSQL

La estructura prevista es:

postgresql/
    schema/
    migrations/
    queries/

Se utilizará para documentar e implementar:

- Creación de tablas.
- Relaciones y restricciones.
- Índices.
- Consultas.
- Migraciones controladas.
- Integridad referencial.
- Preparación de vistas analíticas.

No se publicarán respaldos operativos ni
credenciales de acceso a bases de datos.

## 8. Calidad de los datos

Se considerarán los siguientes criterios:

- Completitud.
- Validez.
- Consistencia.
- Integridad.
- Unicidad.
- Oportunidad.
- Coherencia temporal.
- Trazabilidad.
- Exactitud cuando sea verificable.

Las reglas de validación deberán distinguir
entre fallas de adquisición, transmisión,
procesamiento y condiciones reales del activo.

## 9. Datos de ejemplo y sintéticos

### sample-data/

Contendrá datos pequeños que puedan publicarse
legalmente y utilizarse para ejecutar ejemplos.

### synthetic/

Contendrá datos generados artificialmente para
pruebas de algoritmos, visualización y validación
funcional del procesamiento.

Cada dataset deberá documentar:

- Procedencia.
- Variables y unidades.
- Método de generación o adquisición.
- Número de registros.
- Limitaciones.
- Condiciones de reutilización.
- Licencia aplicable.

Los datos sintéticos no constituyen evidencia
del comportamiento real del motor-bomba.

## 10. Datos operativos privados

Los directorios raw/ y processed/ se utilizarán
para almacenamiento local de trabajo.

Sus contenidos operativos estarán excluidos
del versionamiento público conforme a .gitignore.

No se incorporarán:

- Credenciales.
- Datos sensibles de infraestructura.
- Respaldos operativos.
- Registros privados de seguridad.
- Capturas de tráfico confidenciales.
- Datos de terceros sin autorización.

El archivo .gitignore no reemplaza la
revisión de seguridad previa al commit.

## 11. Integración con analítica

Los recursos de este directorio podrán
utilizarse desde:

- ../analytics/notebooks/
- ../analytics/case-studies/
- ../analytics/models/
- ../analytics/reports/

Los procesos analíticos deberán documentar
la fuente y la transformación de los datos.

## 12. Control de versiones

Los cambios en esquemas o contratos deberán:

1. Identificar la versión afectada.
2. Evaluar compatibilidad.
3. Documentar los campos modificados.
4. Actualizar consumidores relacionados.
5. Incorporar pruebas.
6. Registrar los cambios.
7. Conservar trazabilidad de migraciones.

No se modificará la estructura de datos
operativa sin evaluar sus dependencias.

## 13. Estados de implementación

- PROPUESTO.
- DOCUMENTADO.
- IMPLEMENTADO.
- EN PRUEBAS.
- VALIDADO.
- OBSOLETO.

Los scripts SQL y esquemas no se considerarán
validados hasta superar las pruebas aplicables.

## 14. Documentación relacionada

- ../docs/data/
- ../docs/analytics/
- ../docs/architecture/
- ../docs/procedures/
- ../docs/standards/
- ../analytics/
- ../tests/

## 15. Seguridad y licenciamiento

Consultar:

- ../SECURITY.md
- ../LICENSE
- ../LICENSES/README.md

Los datasets externos deberán conservar
sus licencias y condiciones de utilización.

---

**IIoT-Laboratory**

*Del activo al dato, del dato a la decisión.*
