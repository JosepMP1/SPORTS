# SPORTS

Portal deportivo estático de noticias, análisis y contenidos de fútbol, baloncesto, motor y tenis.

## Panel editorial

La web usa [Decap CMS](https://decapcms.org/) para editar artículos desde `/admin/`. El contenido se guarda en `content/articles.json` y los cambios se versionan en Git; no hace falta mantener un servidor propio.

### Activación en Netlify

1. Importa el repositorio `JosepMP1/SPORTS` en Netlify y despliega la rama `main`. El archivo `netlify.toml` publica la raíz del repositorio sin paso de compilación.
2. En la configuración del sitio, activa **Identity** y limita el registro a invitaciones.
3. En **Identity > Services**, activa **Git Gateway** y conecta el repositorio de GitHub del sitio.
4. Invita desde Identity a las personas que podrán editar y publicar.
5. Abre `https://<tu-sitio>.netlify.app/admin/` e inicia sesión. Las publicaciones usan flujo editorial para poder revisar los cambios antes de publicarlos.

La autenticación de Netlify y la conexión de Git Gateway se habilitan desde el panel de Netlify; no se guardan credenciales en este repositorio.

### Crear o editar un artículo

En el panel, abre **Artículos > Noticias y artículos**. Completa el titular, el deporte, la competición, el resumen, la fecha, la imagen, su texto alternativo y el artículo. Separa los párrafos del artículo con una línea en blanco. La URL debe ser única y usar solo minúsculas, números y guiones, por ejemplo `analisis-del-partido`.

Los artículos publicados aparecen en la portada y cada uno tiene su propia página de lectura. Los filtros por deporte y la búsqueda se generan a partir de los mismos datos.
