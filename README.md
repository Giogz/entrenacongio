# Entrena con Gio — Guía para funcionarios consulares

Guía interactiva de capacitación (trámites consulares) del Consulado del Perú en Miami.
Es un sitio estático: **no necesita servidor ni base de datos**.

## Estructura (subir tal cual)
```
index.html          → la guía (página principal)
poderes/            → modelos de poder en PDF (índice + 31 modelos)
README.md
```
> Importante: la carpeta **`poderes/` debe ir junto a `index.html`** para que
> funcionen los enlaces de descarga y el índice de modelos.

## Qué incluye
- 88 temas en 11 áreas (marco normativo, DNI, fichas manuales, SIO, registro
  civil, funciones notariales, pasaportes, visas —incluye visa en línea e-SAMI—
  y modelos de poderes).
- Buscador con sugerencias y flujo "¿No encontraste tu tema?" (formulario de
  solicitud por correo).
- **Modelos de poder**: se leen en la guía, se **completan** (la plataforma
  rellena los datos) y se **descargan en PDF o Word**; además un **selector**
  para bajar cualquier modelo en blanco (PDF/Word).

## Publicar en GitHub Pages
1. Crear un repositorio nuevo (público) y subir estos archivos.
2. En el repo: **Settings → Pages**.
3. En "Build and deployment" → Source: **Deploy from a branch**.
4. Branch: **main** y carpeta **/ (root)** → **Save**.
5. En 1–2 minutos, el sitio queda en `https://TU-USUARIO.github.io/NOMBRE-REPO/`.

## Notas técnicas
- La descarga en **PDF** usa jsPDF por CDN; si no carga, cae a "imprimir → guardar
  como PDF". La descarga en **Word (.doc)** funciona siempre, sin conexión.
- El formulario de "solicitar tema" usa FormSubmit y requiere una **activación
  única** (revisar el correo de destino la primera vez).
- El contador de consultas persiste por navegador (localStorage) en hosting propio.
