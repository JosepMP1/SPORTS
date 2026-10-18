# SPORTS

Portal de noticias y análisis deportivos de fútbol, baloncesto, motor y tenis. La portada carga los metadatos desde `articles.json` y los artículos se leen desde sus páginas en `articles/`.

## Publicar y editar artículos

El panel editorial está en [`admin.html`](./admin.html). Usa la API de contenidos de GitHub para guardar el texto de un artículo en `articles/<slug>.html` y actualizar `articles.json`; los cambios guardados crean commits en el repositorio.

Para usarlo, introduce el token de GitHub y el usuario del repositorio. Crea un token con permisos mínimos de contenido para este repositorio y retíralo al terminar si ya no lo necesitas. El panel no guarda el token, pero se utiliza desde el navegador para realizar peticiones a GitHub.

Los artículos publicados deben tener un slug único, coincidir con el nombre del archivo HTML de `articles/` y disponer de sus metadatos en `articles.json`.
