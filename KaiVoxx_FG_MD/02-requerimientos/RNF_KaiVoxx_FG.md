---
title: RNF_KaiVoxx_FG
source: RNF_KaiVoxx_FG.docx
---

KaiVoxx FG

Sistema de detección de fraude en facturación y pagos

KaiVoxx FG - Sistema de detección de fraude en facturación y pagos

Elaborado por: Camilo Andrés Osorio Mejía

Equipo: Grupo por definir

Requerimientos no funcionales

Camilo Andrés Osorio Mejía

KaiVoxx FG

| ID | Categoría | Prioridad | Descripción |
| --- | --- | --- | --- |
| RNF-01 | Seguridad | Alta | Cifrado en tránsito y en reposo, control de acceso por roles y auditoría de actividades. |
| RNF-02 | Rendimiento | Alta | Las consultas individuales deben responder en menos de 2 segundos en condiciones normales. |
| RNF-03 | Disponibilidad | Alta | El servicio debe estar disponible al menos 99% en horario operativo. |
| RNF-04 | Escalabilidad | Alta | La solución debe soportar aumento de documentos sin reescritura total de la arquitectura. |
| RNF-05 | Usabilidad | Media | La interfaz debe permitir revisión rápida de alertas y navegación sencilla. |
| RNF-06 | Mantenibilidad | Alta | El sistema debe separarse por capas y servicios para facilitar cambios y pruebas. |
| RNF-07 | Trazabilidad | Alta | Toda alerta debe conservar evidencia, responsable, fecha y motivo de decisión. |
| RNF-08 | Interoperabilidad | Alta | Debe integrarse con ERP, correo y sistemas externos mediante APIs o archivos. |
| RNF-09 | Portabilidad | Media | La solución debe poder desplegarse en nube o entornos equivalentes con ajustes mínimos. |
| RNF-10 | Cumplimiento | Alta | Debe respetar políticas de protección de datos y controles internos de la organización. |

# Notas de diseño relacionadas

- La seguridad requiere autenticación por roles, cifrado y auditoría.

- El rendimiento y la escalabilidad justifican separar el motor de fraude del backend principal.

- La trazabilidad es esencial para justificar por qué un caso fue marcado como sospechoso.
