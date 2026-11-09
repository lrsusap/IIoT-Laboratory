
# Política de Seguridad — IIoT-Laboratory

## Alcance

Esta política aplica al código, configuraciones,
documentación técnica e infraestructura experimental
del Laboratorio IIoT.

## Principios

- Seguridad desde el diseño.
- Mínimo privilegio.
- Separación entre entornos de prueba y operación.
- Protección de credenciales y claves privadas.
- Validación controlada de cambios.
- Trazabilidad de configuraciones y versiones.

## Información que no debe publicarse

- Contraseñas y tokens reales.
- Claves privadas y certificados confidenciales.
- Archivos .env con secretos.
- Respaldos con credenciales.
- Configuraciones que revelen accesos sensibles.
- Registros con información privada.
- Datos o materiales de terceros sin autorización.

## Reporte de vulnerabilidades

No publicar detalles explotables de vulnerabilidades
no corregidas mediante Issues públicos.

Utilizar el canal de reporte privado de vulnerabilidades
de GitHub cuando esté habilitado.

En ausencia de ese canal, suspender la divulgación
pública hasta definir un medio de contacto seguro.

## Pruebas de ciberseguridad

Las pruebas de penetración, generación de tráfico
malicioso y utilización de honeypots deberán realizarse
exclusivamente en entornos propios o autorizados.

Se documentarán el alcance, las condiciones,
los resultados y los controles de aislamiento.

## Estado de soporte

El proyecto se encuentra en desarrollo experimental.

No se declara apto para proteger procesos industriales
de producción sin evaluación y validación específicas.
