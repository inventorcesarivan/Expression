# Expression v1

Primera base independiente para evaluación de expresiones artísticas mediante cámara.

## Base reutilizada

La aplicación conserva la parte probada de BodyBeat relacionada con:
- activación explícita de la cámara;
- renderizado de cámara en tiempo real;
- funcionamiento en pantalla horizontal en móviles;
- detección corporal mediante MediaPipe Pose;
- análisis de landmarks y movimiento;
- sistema de puntuación por características del movimiento.

## Qué se eliminó de BodyBeat

Esta versión ya no depende de la grilla, LEDs, pads, bases musicales, loops ni creación musical.

## Categorías iniciales

- Baile / Danza
- Canto — expresión visual
- Actuación
- Farmear Aura / Presencia
- Expresión corporal
- Expresión general

La categoría de canto, en esta primera etapa, evalúa solamente lo observable por cámara. El análisis de voz/afinación queda preparado como futura capa independiente.

## Publicación

Es un sitio estático: `index.html` está en la raíz y puede publicarse directamente en GitHub + Netlify.

La cámara requiere HTTPS o un contexto seguro.
