# Oracle Sales Play Academy — V10 Complete

Esta versión implementa los tres cambios solicitados:

## 1. Anti-cheat local
- Respuestas aleatorias.
- Metadatos de evaluación ofuscados.
- No aparecen `best`, `partial` o `risky` junto a las opciones.
- No se muestra puntaje durante el caso.
- No se revela la mejor respuesta después de cada decisión.
- El feedback detallado se reserva para el final.
- Firma local de puntaje.
- Hash de ruta de respuestas.
- Historial de intentos.
- Detección de manipulación y tiempos anormalmente rápidos.

**Límite real:** GitHub Pages sigue siendo una aplicación estática. Un usuario
muy técnico con control total del navegador puede estudiar el JavaScript. Estas
medidas dificultan el cheating casual, pero no sustituyen validación server-side.

## 2. Popup obligatorio al terminar
Incluye:
- puntaje final
- banda de desempeño
- óptimas / defendibles / mayor riesgo
- duración
- fortalezas
- recomendaciones
- mensaje de cierre específico
- estado de integridad
- repetir caso
- volver a Sales Plays
- ir a Mi progreso

## 3. Preguntas y respuestas más difíciles
Se revisaron las 75 decisiones.
- Las cuatro opciones tienen estructura y longitud mucho más similares.
- Los distractores absolutos se suavizaron.
- Varias respuestas son comercialmente razonables.
- La diferencia está en prioridad, timing, riesgo y contexto.
- La respuesta óptima dejó de ser visualmente la más larga.

Métrica de longitud:
- Antes: 2.00
- V10: 1.02

## Prueba funcional
La versión fue probada en Chromium completando:
autenticación simulada → Sales Play → 5 decisiones → popup final → Mi progreso.

Resultado del test: sin errores JavaScript, popup visible, puntaje visible, recomendaciones presentes, mensaje de cierre presente e integridad local visible.

Consulte `AUDIT.txt` para el detalle.


### Control adicional de dificultad
En las 75 decisiones, la respuesta óptima es la más larga en 27 casos, la más corta en 32 y queda en posición intermedia en 16. Esto elimina el patrón visual que hacía fácil identificarla por extensión.
