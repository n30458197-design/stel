# Mis videos

Una app web de videos al estilo YouTube que funciona en un solo archivo HTML, sin servidor ni instalación. Subes videos desde tu dispositivo y los ves en tu propia biblioteca.

## Funciones

- Página de inicio con cuadrícula de videos, miniaturas automáticas, duración, canal, vistas y fecha.
- Buscador y filtro de videos con "Me gusta".
- Página de video con reproductor, suscripción al canal, me gusta y comentarios.
- Lista de videos recomendados; al terminar uno pasa al siguiente.
- Subida de videos con título y nombre de canal.
- Opción para eliminar videos de la biblioteca.
- Tema claro y oscuro según la configuración del sistema.
- Diseño adaptable a celular y escritorio.

## Estructura

```
.
├── app-de-videos-yt.html   # Toda la app: HTML, CSS y JavaScript
└── README.md
```

## Cómo usarla

### Con Live Server en VS Code (recomendado)

1. Abre la carpeta del proyecto en VS Code.
2. Instala la extensión **Live Server**.
3. Haz clic derecho en `app-de-videos-yt.html` y elige **Open with Live Server**.

### Con doble clic

Abre `app-de-videos-yt.html` en tu navegador.

> Usa siempre la misma forma de abrirla. Los datos se guardan por navegador y por dirección, así que `127.0.0.1:5500` y `file://` tienen bibliotecas distintas.

## Cómo subir un video

1. Pulsa **Subir video**.
2. Elige el archivo, escribe el título y el nombre del canal.
3. Pulsa **Publicar**. El video aparece al inicio de la cuadrícula.

## Dónde se guardan los datos

Los videos, las vistas, los me gusta, los comentarios y las suscripciones se guardan en tu navegador con **IndexedDB**. Siguen ahí al cerrar y volver a abrir la página.

- Los datos no salen de tu equipo ni se comparten con nadie.
- Si borras los datos del sitio en el navegador, se pierden.
- Los videos ocupan espacio en tu disco, así que usa **Eliminar** cuando no los necesites.

## Tecnologías

- HTML, CSS y JavaScript sin dependencias.
- IndexedDB para guardar los videos y los datos.
- Google Fonts (Bricolage Grotesque). Sin internet funciona con la fuente del sistema.

## Limitaciones

- Es una biblioteca personal: no hay cuentas ni videos de otros usuarios.
- Para compartir videos entre personas haría falta un servidor y una base de datos.
- Los formatos que se pueden reproducir dependen de tu navegador (MP4 con H.264 funciona en casi todos).

## Ideas para ampliarla

- Categorías y listas de reproducción.
- Edición del título y la descripción de cada video.
- Exportar e importar la biblioteca.
- Servidor propio para subir y compartir videos.
