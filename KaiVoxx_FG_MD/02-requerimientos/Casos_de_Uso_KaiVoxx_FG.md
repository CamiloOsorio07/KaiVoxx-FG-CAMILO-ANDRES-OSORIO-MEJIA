---
title: Casos_de_Uso_KaiVoxx_FG
source: Casos_de_Uso_KaiVoxx_FG.docx
---

KaiVoxx FG

Sistema de detección de fraude en facturación y pagos

KaiVoxx FG - Sistema de detección de fraude en facturación y pagos

Elaborado por: Camilo Andrés Osorio Mejía

Equipo: Grupo por definir

Casos de uso

Camilo Andrés Osorio Mejía

KaiVoxx FG

## UC-01 - Autenticarse en el sistema

| Campo | Detalle |
| --- | --- |
| Actores | Contabilidad, Tesorería, Auditoría, Gerencia, Administrador |
| Precondición | El actor tiene acceso al sistema o el documento ya está disponible para ingreso. |
| Flujo principal | El actor ingresa credenciales válidas para acceder a la plataforma. El sistema valida el usuario, aplica el rol y muestra el panel correspondiente. |
| Flujos alternativos | Credenciales inválidas, cuenta bloqueada, rol sin permisos. |
| Postcondición | El sistema deja evidencia del resultado y actualiza el estado del caso. |

## UC-02 - Registrar documento de factura o pago

| Campo | Detalle |
| --- | --- |
| Actores | Contabilidad, Tesorería, Integración externa |
| Precondición | El actor tiene acceso al sistema o el documento ya está disponible para ingreso. |
| Flujo principal | El actor carga el documento o el sistema lo recibe desde una integración. El archivo se valida, se almacena y se deja listo para análisis. |
| Flujos alternativos | Documento corrupto, formato no permitido, datos faltantes. |
| Postcondición | El sistema deja evidencia del resultado y actualiza el estado del caso. |

## UC-03 - Analizar riesgo de fraude

| Campo | Detalle |
| --- | --- |
| Actores | Sistema KaiVoxx FG |
| Precondición | El actor tiene acceso al sistema o el documento ya está disponible para ingreso. |
| Flujo principal | Un documento entra al flujo de análisis. El motor evalúa reglas, patrones y anomalías, calcula score y genera alertas si corresponde. |
| Flujos alternativos | Datos insuficientes, falla de motor, umbral no definido. |
| Postcondición | El sistema deja evidencia del resultado y actualiza el estado del caso. |

## UC-04 - Revisar alerta

| Campo | Detalle |
| --- | --- |
| Actores | Contabilidad, Tesorería, Auditoría |
| Precondición | El actor tiene acceso al sistema o el documento ya está disponible para ingreso. |
| Flujo principal | El actor abre una alerta generada por el sistema. Consulta evidencias, agrega comentarios y decide aprobar, rechazar o escalar. |
| Flujos alternativos | El caso ya fue resuelto o el usuario no tiene permisos. |
| Postcondición | El sistema deja evidencia del resultado y actualiza el estado del caso. |

## UC-05 - Bloquear o retener pago sospechoso

| Campo | Detalle |
| --- | --- |
| Actores | Tesorería, Sistema |
| Precondición | El actor tiene acceso al sistema o el documento ya está disponible para ingreso. |
| Flujo principal | Existe un caso con riesgo alto o una regla crítica. El sistema cambia el estado del pago a retenido y notifica a los responsables. |
| Flujos alternativos | Integración caída, pago ya ejecutado. |
| Postcondición | El sistema deja evidencia del resultado y actualiza el estado del caso. |

## UC-06 - Configurar reglas y umbrales

| Campo | Detalle |
| --- | --- |
| Actores | Administrador |
| Precondición | El actor tiene acceso al sistema o el documento ya está disponible para ingreso. |
| Flujo principal | El administrador ingresa al módulo de configuración. Crea, modifica o desactiva reglas, umbrales y catálogos. |
| Flujos alternativos | Valores inválidos, falta de permisos. |
| Postcondición | El sistema deja evidencia del resultado y actualiza el estado del caso. |

## UC-07 - Generar reportes

| Campo | Detalle |
| --- | --- |
| Actores | Gerencia, Auditoría |
| Precondición | El actor tiene acceso al sistema o el documento ya está disponible para ingreso. |
| Flujo principal | El usuario solicita un reporte por periodo o proveedor. El sistema consolida métricas, tendencias y exporta el resultado. |
| Flujos alternativos | No hay datos suficientes o filtro incorrecto. |
| Postcondición | El sistema deja evidencia del resultado y actualiza el estado del caso. |
