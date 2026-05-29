---
title: Matriz_Riesgos_KaiVoxx_FG
source: Matriz_Riesgos_KaiVoxx_FG.docx
---

KaiVoxx FG

Sistema de detección de fraude en facturación y pagos

KaiVoxx FG - Sistema de detección de fraude en facturación y pagos

Elaborado por: Camilo Andrés Osorio Mejía

Equipo: Grupo por definir

Matriz de riesgos

Camilo Andrés Osorio Mejía

KaiVoxx FG

La siguiente matriz resume los riesgos más relevantes identificados para el proyecto, con foco en impacto sobre el negocio, la adopción y la calidad de la solución.

| ID | Riesgo | Probabilidad | Impacto | Nivel | Mitigación |
| --- | --- | --- | --- | --- | --- |
| R-01 | Datos incompletos o sucios | 4 | 4 | Alto | Validaciones, limpieza de datos y plantillas de carga. |
| R-02 | Falsos positivos en exceso | 3 | 4 | Alto | Human-in-loop, ajuste de umbrales y retroalimentación. |
| R-03 | Integración compleja con ERP | 3 | 5 | Alto | Adaptadores genéricos, pruebas con sandbox y API contract. |
| R-04 | Resistencia al cambio de usuarios | 3 | 3 | Medio | Capacitación, acompañamiento y despliegue gradual. |
| R-05 | Riesgos de seguridad y privacidad | 3 | 5 | Alto | Cifrado, RBAC, backups y revisión legal. |
| R-06 | Sobrecarga del sistema en picos | 2 | 4 | Medio | Colas, escalado horizontal y monitoreo. |
| R-07 | Reglas de negocio desactualizadas | 3 | 3 | Medio | Comité de revisión mensual y versionado. |
| R-08 | Dependencia de datos históricos | 2 | 4 | Medio | Arranque con reglas base y carga incremental. |

# Criterio de priorización

- Los riesgos con nivel alto deben ser tratados primero.

- Los riesgos medios requieren seguimiento y una estrategia de contingencia.

- El registro de riesgos debe actualizarse durante todo el ciclo del proyecto.
