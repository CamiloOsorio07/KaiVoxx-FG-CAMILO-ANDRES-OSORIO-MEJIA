---
title: RF_KaiVoxx_FG
source: RF_KaiVoxx_FG.docx
---

KaiVoxx FG

Sistema de detección de fraude en facturación y pagos

KaiVoxx FG - Sistema de detección de fraude en facturación y pagos

Elaborado por: Camilo Andrés Osorio Mejía

Equipo: Grupo por definir

Requerimientos funcionales

Camilo Andrés Osorio Mejía

KaiVoxx FG

| ID | Descripción | Prioridad | Criterio de aceptación |
| --- | --- | --- | --- |
| RF-01 | El sistema debe permitir el inicio de sesión con roles diferenciados para contabilidad, tesorería, auditoría, gerencia y administrador. | Alta | Un usuario con credenciales válidas accede y ve únicamente las funciones permitidas por su rol. |
| RF-02 | El sistema debe recibir facturas desde carga manual, correo, API o SFTP. | Alta | El sistema registra correctamente el documento en al menos uno de los canales permitidos. |
| RF-03 | El sistema debe extraer y normalizar datos clave de las facturas y pagos. | Alta | Se obtienen número, fecha, valor, proveedor y cuenta asociada con un nivel aceptable de precisión. |
| RF-04 | El sistema debe detectar duplicados, montos atípicos y cambios sospechosos de cuenta bancaria. | Alta | Se genera una alerta cuando el documento cumple la regla o el patrón anómalo definido. |
| RF-05 | El sistema debe calcular un puntaje de riesgo por caso. | Alta | Cada caso recibe un score y una clasificación clara (bajo, medio, alto). |
| RF-06 | El sistema debe permitir revisión humana de alertas con comentarios y decisión final. | Alta | Un usuario revisa la alerta y registra aprobar, rechazar o escalar. |
| RF-07 | El sistema debe bloquear preventivamente pagos con riesgo alto o según configuración. | Alta | Los pagos marcados como críticos quedan en estado retenido hasta revisión. |
| RF-08 | El sistema debe notificar por correo o canal interno los casos relevantes. | Media | El usuario recibe la alerta con enlace o referencia al caso. |
| RF-09 | El sistema debe registrar trazabilidad completa de cada caso y su evidencia. | Alta | Quedan guardadas fechas, actores, decisión y soportes adjuntos. |
| RF-10 | El sistema debe generar reportes y tableros de seguimiento. | Media | Se visualizan métricas de alertas, casos resueltos y tendencia de riesgo. |
| RF-11 | El sistema debe administrar catálogos de reglas, umbrales y proveedores. | Media | Un administrador puede crear, editar o inactivar reglas sin romper el sistema. |
| RF-12 | El sistema debe integrarse con el ERP para consultar y actualizar estados. | Alta | Se evidencia intercambio de datos con el sistema externo configurado. |

# Observaciones de trazabilidad

- Los requerimientos RF-04, RF-05 y RF-07 son los más críticos para el valor del negocio.

- RF-09 y RF-12 sostienen la auditoría y la integración con sistemas empresariales.

- Cada RF debe reflejarse al menos en un caso de uso y en una o más historias de usuario.
