
# Guía de Contribución — IIoT-Laboratory

## 1. Propósito

Establecer criterios para incorporar código, documentación,
configuraciones, pruebas y mejoras al Laboratorio IIoT,
garantizando calidad, trazabilidad y seguridad.

## 2. Alcance

Las contribuciones pueden corresponder a:

- Ingeniería de mantenimiento y gestión de activos.
- Instrumentación, sensores y sistemas embebidos.
- Redes y telecomunicaciones OT/IT.
- Ciberseguridad industrial.
- Sistemas de supervisión e integración.
- Bases de datos y analítica.
- Inteligencia artificial y aprendizaje automático.
- Documentación técnica y procedimientos.

## 3. Principios de contribución

Toda contribución deberá:

1. Tener un propósito técnico definido.
2. Identificar los componentes afectados.
3. Mantener compatibilidad con la arquitectura vigente.
4. Considerar riesgos operacionales y de ciberseguridad.
5. Incluir documentación suficiente.
6. Incorporar pruebas cuando corresponda.
7. Diferenciar resultados validados de propuestas.
8. Respetar las licencias y derechos de terceros.

## 4. Flujo de trabajo

1. Registrar la necesidad o mejora mediante GitHub Issues.
2. Definir alcance y criterios de aceptación.
3. Crear una rama de trabajo.
4. Desarrollar y documentar los cambios.
5. Ejecutar las pruebas correspondientes.
6. Revisar impactos sobre otros subsistemas.
7. Crear un Pull Request.
8. Integrar los cambios aprobados.

## 5. Convenciones de ramas

- main: versión estable del repositorio.
- feature/: nuevas funcionalidades.
- fix/: correcciones.
- docs/: documentación.
- test/: procedimientos y pruebas.
- security/: controles de seguridad.

Ejemplo:

feature/esp32-mqtt-telemetry

## 6. Convenciones de commits

Se recomienda utilizar mensajes descriptivos:

- feat: nueva funcionalidad.
- fix: corrección de errores.
- docs: actualización documental.
- test: incorporación de pruebas.
- refactor: reorganización sin cambio funcional.
- chore: mantenimiento del repositorio.
- security: mejora de seguridad.

Ejemplo:

feat: add ESP32-S3 sensor acquisition module

## 7. Validación técnica

Los cambios deberán documentar, cuando corresponda:

- Hardware y firmware utilizados.
- Versiones de dependencias.
- Interfaces y protocolos involucrados.
- Configuraciones modificadas.
- Condiciones y resultados de las pruebas.
- Evidencias de aceptación.
- Problemas conocidos y limitaciones.

Una prueba documental no equivale a validación física.

## 8. Seguridad

No se permite incorporar credenciales reales, claves
privadas, tokens o configuraciones sensibles.

Las pruebas de ciberseguridad deberán realizarse
en entornos controlados y autorizados.

Consultar SECURITY.md.

## 9. Documentación

Los cambios que afecten la arquitectura deberán reflejarse
en los documentos correspondientes.

Las decisiones significativas deberán registrarse mediante
Architecture Decision Records (ADR).

## 10. Criterios de aceptación

Una contribución podrá integrarse cuando:

- Su propósito y alcance estén documentados.
- No incorpore secretos ni información restringida.
- Respete las convenciones del repositorio.
- Sus pruebas estén documentadas.
- Los efectos sobre otros componentes sean conocidos.
- Exista aprobación del responsable del proyecto.

## 11. Autoría y reconocimiento

El Laboratorio IIoT fue creado por
Lewis Rafael Susa Peñate.

Las contribuciones de terceros deberán conservar
el reconocimiento de sus respectivos autores y
cumplir las condiciones de licenciamiento aplicables.

## 12. Estado del proyecto

IIoT-Laboratory es un proyecto experimental en desarrollo.

Los componentes no deben considerarse aptos para uso
industrial en producción sin pruebas y validaciones
específicas.
