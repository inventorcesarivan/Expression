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

Esta versión incorpora una primera capa de música de fondo para las evaluaciones. Las bases musicales por defecto se conectan desde `assets/music/`; también se permite cargar un archivo de audio propio desde el dispositivo.

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

## Música de fondo

Desde el panel de evaluación se puede abrir **Evaluar con música de fondo**. El usuario puede seleccionar una base, escucharla como vista previa y confirmar con **Guardar selección**. La base confirmada queda preparada para comenzar automáticamente al iniciar la evaluación.

Se incluyen 20 estilos en el selector:
- Break dance
- Cumbia
- Cuarteto
- Cinemático
- Electrónica
- Épica
- Funk
- Hip hop
- Jazz
- Latino
- Merengue
- Pop
- Rap
- Reggaetón
- Reggae
- Rock
- Salsa
- Soft
- Tango
- Trap

Se agregaron **Electrónica, Funk y Reggae** como tres estilos adicionales.

Los archivos por defecto todavía no están incluidos porque serán enviados posteriormente para conectarlos a sus respectivos estilos. La aplicación ya tiene preparado el mapa de nombres y rutas en `index.html`.

También existe la opción **Cargar mi propia música**, que permite seleccionar un archivo de audio compatible desde el dispositivo, escucharlo y guardarlo como base para la evaluación.
