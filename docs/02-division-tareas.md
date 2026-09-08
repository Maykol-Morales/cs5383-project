# División de tareas — Proyecto 1 (Caso 2: Advantage Online Shopping)

División por secciones del entregable. Roles ("Persona A" / "Persona B") aún por asignar entre los 2 integrantes del grupo.

## Trabajo conjunto previo (ambos)
- Exploración conjunta del sitio real (30-45 min): carrito, tarjetas de regalo/promos, checkout, wishlist, historial de pedidos. Necesario antes de escribir nada, para que el análisis no asuma flujos que no existen.

## Persona A — Planificación + Análisis (5.1 + 5.2)
1. **Plan de pruebas (5.1):** llenar la plantilla — alcance (módulos: registro/login, catálogo/búsqueda, carrito, tarjetas de regalo/promos, checkout, wishlist, historial), objetivos, criterios de entrada/salida, estimación de esfuerzo, recursos, cronograma.
2. **Riesgos del proyecto** (distintos de los riesgos de producto): recursos limitados, tiempo, dependencia de disponibilidad del sitio real, etc.
3. **Estrategia de pruebas justificada:** enfoque priorizado por el impacto de la campaña de temporada alta → foco en carrito/checkout/descuentos por impacto directo en ventas y margen.
4. **Niveles de prueba:** dado que solo hay acceso a la UI pública, probablemente foco en sistema + aceptación (no componente/integración).
5. **Análisis (5.2):** condiciones de prueba a partir de los 8 requisitos funcionales + no funcionales (consistencia del carrito al navegar, carga <2s, sin errores de redondeo).
6. **Riesgos de producto adicionales** más allá de los 3 iniciales del enunciado (descuentos mal calculados, pérdida de carrito, pedidos duplicados) — se evalúa que el grupo identifique riesgos propios.
7. **Matriz de trazabilidad** requisito → condición(es).
8. **Priorización** alto/medio/bajo con justificación de las altas.

**Entregable a Persona B:** lista de condiciones priorizadas (alto/medio) con su justificación — insumo directo para el diseño de casos.

## Persona B — Diseño + Ejecución (5.3 + 5.4)
1. **Diseño de casos (5.3):** derivar ≥15 casos a partir de las condiciones alto/medio de Persona A, cubriendo ≥4 funcionalidades (sugerido: carrito, tarjetas de regalo/promos, checkout, registro/login o wishlist).
2. **Técnicas de caja negra variadas:**
   - Partición de equivalencia / valores límite → montos de tarjeta de regalo, cantidades en carrito.
   - Tabla de decisión → combinaciones de código promo válido/inválido + monto del carrito + tipo de usuario.
   - Transición de estados → flujo carrito → checkout → confirmación → historial (o estado de sesión).
3. **Datos de prueba** necesarios (usuarios de prueba, códigos promo, productos, montos límite).
4. **Ejecución manual (5.4):** correr todos los casos de prioridad alta sobre el sitio real; registrar esperado/obtenido/veredicto.
5. **Hallazgos** con capturas de pantalla.
6. **Reflexión de cierre** sobre candidatos a automatizar en Proyecto 2.

## Trabajo conjunto (ambos, en paralelo/cierre)
- Revisión cruzada: A revisa que el diseño de B cubra bien las condiciones priorizadas; B revisa que el plan/análisis de A sea consistente con lo probable en el sitio real.
- Consolidación del informe final único y pasada de formato/terminología antes de entregar.

## Orden sugerido
1. Ambos: exploración conjunta del sitio.
2. Persona A avanza plan + análisis; Persona B explora técnicas de diseño aplicables y arma el esqueleto de la matriz de casos.
3. Sincronización: A entrega condiciones priorizadas → B arranca diseño de casos en serio.
4. Persona B ejecuta y reporta hallazgos.
5. Ambos: consolidación final del informe.
