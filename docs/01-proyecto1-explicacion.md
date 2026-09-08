# Proyecto 1 — Qué es y qué se pide

Primer entregable de una secuencia de 3 proyectos del curso **CS5383 · Verificación y Pruebas de Software**. Trabajamos sobre el **Caso 2 — E-commerce (Advantage Online Shopping)**: https://www.advantageonlineshopping.com/

## Contexto de negocio

Advantage está a semanas de su campaña de temporada alta. Le preocupa que errores en el carrito o en la aplicación de tarjetas de regalo/promociones generen pérdida de ventas o descuentos mal calculados, afectando el margen del negocio.

**Alcance funcional del sistema:** registro y login de usuarios, navegación y búsqueda de productos por categoría, carrito de compras, aplicación de tarjetas de regalo/promociones, checkout (dirección de envío + método de pago), lista de deseos (wishlist), historial de pedidos.

**Requisitos funcionales clave (8):**
1. Registro/login validan campos obligatorios y muestran errores claros ante datos inválidos.
2. La búsqueda de productos devuelve resultados relevantes al término buscado.
3. Agregar un producto al carrito actualiza contador de items y subtotal correctamente.
4. Quitar un producto del carrito recalcula el subtotal correctamente.
5. Aplicar tarjeta de regalo/código promocional reduce el total en el monto correcto, sin permitir montos negativos.
6. El checkout exige dirección de envío y método de pago antes de confirmar la compra.
7. Al confirmar una compra, el pedido aparece correctamente en el historial de pedidos.
8. Agregar un producto a la wishlist no afecta el carrito ni genera un cargo.

**Requisitos no funcionales:** carrito consistente al navegar entre páginas, carga de catálogo <2s, cálculos monetarios sin errores de redondeo.

**Riesgos iniciales (no exhaustivos — el análisis debe sumar más):** descuentos mal calculados, pérdida del contenido del carrito al navegar, pedidos duplicados por doble clic en "Comprar".

## Estructura del entregable

Es **un solo informe** con 4 secciones, alineadas al proceso ISTQB:

### 5.1 Planificación de pruebas
- Plan de pruebas completo (plantilla del profesor): alcance, objetivos, criterios de entrada/salida, estimación de esfuerzo, recursos, riesgos, cronograma.
- Estrategia de pruebas justificada según el contexto del caso.
- Niveles de prueba a aplicar (componente/integración/sistema/aceptación) y profundidad.

### 5.2 Análisis de pruebas
- Condiciones de prueba derivadas de los requisitos funcionales y no funcionales (la "base de pruebas").
- Matriz de trazabilidad **Requisito → Condición(es) de prueba**, sin huecos de cobertura.
- Priorización de condiciones (alto/medio/bajo) con justificación de cada prioridad alta.

### 5.3 Diseño de pruebas
- **Mínimo 15 casos de prueba**, derivados de condiciones alto/medio riesgo, cubriendo **al menos 4 funcionalidades distintas**.
- Cada caso: ID, condición relacionada, precondiciones, pasos, datos de prueba, resultado esperado, prioridad.
- Técnicas de caja negra distintas (partición de equivalencia, valores límite, tabla de decisión, transición de estados), justificando dónde se aplicó cada una.
- Datos de prueba necesarios para ejecutar sobre el sistema real.

### 5.4 Ejecución manual de casos críticos y hallazgos
- Ejecutar **todos** los casos de prioridad **alta** (no todo el diseño) sobre el sitio real.
- Registrar resultado esperado vs. obtenido y veredicto (pasó/falló/bloqueado).
- Reportar hallazgos (no necesariamente defectos): resumen, pasos de reproducción, esperado vs. obtenido, severidad, evidencia (captura de pantalla).
- Reflexión de cierre: qué casos automatizarían en el Proyecto 2 y por qué, sustentado en lo observado (no en teoría general).

## Formato de entrega

- Informe en Word o PDF.
- Casos de prueba y matriz de trazabilidad como tablas en el informe o anexo Excel referenciado.
- Nombre de archivo sugerido: `Proyecto1_Caso2_Grupo[X].docx`.

## Notas del enunciado

- Grupos de máximo 2 integrantes.
- El caso elegido (Caso 2) se reutiliza en el Proyecto 2 — decisiones tomadas aquí (qué funcionalidades priorizar, qué automatizar) tienen impacto directo ahí.
