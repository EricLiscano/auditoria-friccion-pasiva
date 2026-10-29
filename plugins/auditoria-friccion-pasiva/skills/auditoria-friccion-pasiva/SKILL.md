---
name: auditoria-friccion-pasiva
description: Audita usabilidad con señales pasivas —capturas, eventos y embudos— sin solicitar feedback directo; distingue hechos, hipótesis y métricas no observables.
disable-model-invocation: true
---

# Auditoría de fricción pasiva

Usa esta skill cuando el usuario pida una auditoría de UX basada en comportamiento implícito, eventos, analítica, capturas o recorridos observados, sin encuestas ni entrevistas.

## Principio de evidencia

- Analiza solo datos suministrados o disponibles de forma autorizada en el proyecto. No inventes sesiones, conteos, tasas, causas, abandono ni comportamiento del cursor.
- Separa claramente **observación**, **interpretación/hipótesis** y **dato no disponible**. Acompaña los hallazgos con la fuente concreta y un nivel de confianza.
- Una captura estática permite detectar riesgos de jerarquía, legibilidad, agrupación, redacción o estados visibles. Por sí sola no demuestra rage clicks, dead clicks, movimiento errático, espera excesiva, drop-off ni backtracking.
- Para rage clicks se necesita secuencia temporal de interacciones repetidas sobre un objetivo; para dead clicks, registro de click más estado/resultado del elemento; para mouse thrashing, muestras de movimiento; para permanencia anómala, tiempos comparables con una línea base y complejidad de pantalla; para drop-off/backtracking, eventos de navegación y un embudo con denominadores y periodo.
- Si faltan datos conductuales, entrega el diagnóstico visual posible y enumera exactamente qué eventos agregados harían medible cada pregunta. Recomienda instrumentación mínima, local/privada y respetuosa con datos sensibles. No actives analítica, grabación de sesión ni envío de telemetría sin petición expresa.

## Procedimiento

1. Identifica materiales, periodo, población y flujo disponibles. Si una dimensión no está presente, márcala como no observada.
2. Reconstruye el flujo únicamente con los eventos/capturas provistos. Distingue navegación registrada de la secuencia que se infiere.
3. Busca señales en relación con la línea base, si existe. No impongas umbrales universales de frustración ni llames anomalía a un valor aislado sin contexto.
4. Formula de dos a tres hipótesis que relacionen evidencia con un principio de usabilidad y un mecanismo probable. Evita presentar correlación como causa.
5. Propón acciones inmediatas de bajo esfuerzo y alto impacto sin cambiar funcionalidades principales. Para cada una indica ubicación, ajuste, impacto esperado, esfuerzo y confianza; prioriza primero los riesgos sustentados.
6. Si el usuario pide una auditoría de toda la aplicación, recorre navegación, panorama, listados, detalle, creación/edición, agente, adjuntos, relaciones/mapa, búsqueda y exportaciones. Vincula cada observación con rutas, componentes o datos revisados. No afirmes que se observó a usuarios reales si solo se inspeccionó código.

## Formato de salida

Responde en español con estas cuatro secciones:

### 1. INDICADORES DE FRUSTRACIÓN DETECTADOS
Por señal: estado (medida / indicio visual / no observable), evidencia, interpretación y confianza. Incluye Rage Clicks, Dead Clicks, Mouse Thrashed y permanencia solo si la evidencia permite evaluarlos.

### 2. PUNTOS DE FUGA Y ANOMALÍAS EN EL FLUJO
Expón pasos específicos con evidencia de drop-off o backtracking. Si solo hay una pantalla, describe barreras potenciales de ese paso y deja claro que no hay embudo para confirmar abandono.

### 3. HIPÓTESIS DE DISEÑO (¿Qué está fallando?)
Formula 2–3 hipótesis, cada una con señal que la motiva, heurística afectada, alternativa explicativa y confianza. No fuerces tres si los datos no sostienen más.

### 4. PLAN DE ACCIÓN INMEDIATO
Lista priorizada de cambios visuales, de UX Writing o del flujo técnico; incluye esfuerzo e impacto esperado. Separa correcciones confirmadas de experimentos/validaciones. Añade un bloque breve **Datos faltantes para medirlo** cuando corresponda.

Mantén el diagnóstico accionable y proporcional a la evidencia. No hagas cambios de producto durante una auditoría a menos que el usuario también solicite implementarlos.
