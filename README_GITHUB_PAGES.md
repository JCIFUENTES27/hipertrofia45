# Hipertrofia 45 — GitHub Pages / iPhone

## Estructura
- `index.html` — aplicación
- `manifest.webmanifest` — configuración PWA
- `sw.js` — caché offline
- `icons/` — iconos para iPhone/PWA
- `.nojekyll` — evita procesamiento Jekyll
- `404.html` — respaldo de GitHub Pages
- `.github/workflows/pages.yml` — despliegue automático

## Publicación en GitHub

1. Crea un repositorio nuevo, por ejemplo: `hipertrofia45`.
2. Sube **el contenido de esta carpeta**, no la carpeta contenedora.
3. Verifica que la rama principal sea `main`.
4. En GitHub entra a: **Settings → Pages**.
5. En **Build and deployment → Source**, selecciona **GitHub Actions**.
6. Haz un commit/push a `main`.
7. Abre la pestaña **Actions** y espera a que `Deploy GitHub Pages` finalice correctamente.
8. La URL tendrá el formato:
   `https://TU_USUARIO.github.io/hipertrofia45/`

## Instalación en iPhone

1. Abre la URL publicada en **Safari**.
2. Pulsa **Compartir**.
3. Selecciona **Añadir a pantalla de inicio**.
4. Confirma el nombre **Hipertrofia 45**.
5. Abre la app desde el nuevo icono.

## Importante

- La app local ya no se abre como `file://`: se ejecuta bajo HTTPS desde GitHub Pages.
- El `service worker` permite que la interfaz principal funcione después de la primera carga incluso sin conexión.
- Los videos externos requieren conexión a Internet.
- Los datos de progreso y ejercicios completados se guardan con `localStorage` bajo la URL publicada.
