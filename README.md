# BodyBeat

Versión estable preparada para publicación como sitio web estático.

## Estructura

- `index.html` — aplicación BodyBeat.
- `assets/bases-laterales/` — 16 bases laterales cargadas por defecto.
- `netlify.toml` — configuración mínima para publicación estática.

## Publicación

### GitHub
Subir todo el contenido de esta carpeta al repositorio, manteniendo la estructura de `assets`.

### Netlify
Conectar el repositorio de GitHub con Netlify. No se necesita build command: `index.html` está en la raíz.

## Audio por defecto

Los 16 audios laterales se cargan cuando el usuario activa BodyBeat:

- `1` a `8` → columna lateral izquierda, de arriba hacia abajo.
- `9` a `16` → columna lateral derecha, de arriba hacia abajo.

Los sonidos del centro no fueron modificados.

## Cámara en móviles

En teléfonos, BodyBeat requiere orientación horizontal. Si el dispositivo está en vertical, aparece una pantalla indicando al usuario que lo gire. La aplicación no solicita la cámara automáticamente mientras está en esa pantalla; la solicitud de cámara/sonido continúa dependiendo de la acción explícita del usuario.

## Nota

La cámara necesita un contexto seguro para funcionar en producción (HTTPS, como el que proporciona Netlify).
