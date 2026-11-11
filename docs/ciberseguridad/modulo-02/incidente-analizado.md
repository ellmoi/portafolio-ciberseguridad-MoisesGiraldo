# Análisis de escenario: amenazas de identidad e IA

> **Tipo:** ejercicio académico de análisis defensivo.
> **Estado:** escenario de estudio; no es un incidente confirmado ni un informe forense.

## Alcance

El material de estudio plantea riesgos relacionados con identidades digitales, aplicaciones conectadas y agentes de inteligencia artificial con acceso a datos. Este análisis organiza esas áreas desde una perspectiva preventiva. No intenta reproducir una secuencia de ataque ni atribuir actividad a una persona, grupo u organización.

## Resumen

La exposición puede aumentar cuando una identidad conserva sesiones o permisos innecesarios, o cuando un agente automatizado accede a más datos y acciones de los que requiere. Si esos controles fallan, la organización puede perder visibilidad sobre quién accedió a qué información y por qué. El ejercicio recomienda revisar el ciclo de vida de las sesiones, aplicar mínimo privilegio a las cuentas y agentes, exigir aprobación humana para acciones sensibles y conservar registros que permitan investigar anomalías.

## Hipótesis de trabajo

| Hipótesis | Evidencia necesaria para validarla |
| --- | --- |
| Una identidad o sesión podría tener permisos superiores a los necesarios. | Inventario autorizado de roles, sesiones y eventos de acceso. |
| Un agente de IA podría consultar datos fuera de su propósito previsto. | Matriz aprobada de permisos, registros de consultas y revisión del responsable del sistema. |
| Una demora en la revisión o notificación reduciría la capacidad de respuesta. | Cronología sustentada en registros originales y comunicaciones fechadas. |

Estas son preguntas de análisis, no conclusiones sobre un incidente real.

## Controles defensivos prioritarios

1. Asignar a cada identidad y agente solo los permisos indispensables y revisarlos periódicamente.
2. Proteger las cuentas con autenticación resistente al phishing y políticas de sesión adecuadas al riesgo.
3. Delimitar las fuentes de datos y acciones que puede usar cada agente; requerir aprobación humana para operaciones sensibles.
4. Centralizar y revisar registros de autenticación, cambios de permisos y accesos a datos.
5. Definir responsables y un canal de notificación para investigar señales con autorización.

## Límites y calidad de la evidencia

El material de origen compartido no incluye referencias primarias verificables para cada fecha, atribución o impacto que presenta, ni aporta telemetría del entorno. Por ello, este portafolio no repite esas afirmaciones como hechos ni identifica víctimas, responsables o indicadores. Antes de publicar conclusiones sobre un caso real, se deben obtener fuentes originales y evidencia autorizada, documentar su procedencia y registrar el nivel de confianza.

## Entregables relacionados

- [Línea de tiempo del ejercicio](linea-tiempo.md)
- [Mapa de exposición](mapa-exposicion.svg)
- [Brief ejecutivo](brief-150-palabras.md)
- [Bitácora de aprendizaje](fortinet-semana-02.md)
