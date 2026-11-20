# Invitación web · Rosa Aurora & Eduardo del Carmen

Carpeta lista para publicar. Contenido:

- `index.html` – la invitación completa (HTML + CSS + JavaScript, sin frameworks)
- `assets/` – imágenes optimizadas, recortadas del diseño original (marco bordado, hibiscos, anillos, bordado, iconos)
- `.nojekyll` – evita que GitHub Pages procese los archivos

## Datos configurables
Al inicio del `<script>` de `index.html` hay un bloque `CONFIG`:

| Campo | Valor actual |
|---|---|
| `whatsapp` | `52992564553` (¡verifícalo! ver nota abajo) |
| `mensaje` | El mensaje prellenado (se codifica solo) |
| `mapsUrl` | Enlace de Google Maps tomado de tu PPTX (vacío = botón desactivado) |
| `youtubeId` | `GxldQ9eX2wo` (video oficial de "Until I Found You") |

**Nota del número:** un celular mexicano tiene 10 dígitos tras el +52. `992 564 553` tiene 9. Si WhatsApp dice "número no válido", falta un dígito.

## Publicar gratis en GitHub Pages
1. Crea cuenta en https://github.com y pulsa **New repository** → nombre, p. ej. `invitacion` → **Public** → *Create*.
2. Pulsa **uploading an existing file** y arrastra **el contenido** de esta carpeta (`index.html`, `assets`, `.nojekyll`; no la carpeta contenedora). *Commit changes*.
3. **Settings → Pages** → *Source*: **Deploy from a branch** → Branch **main** / **(root)** → *Save*.
4. En 1–2 minutos tu enlace será `https://TU-USUARIO.github.io/invitacion/`. Cópialo y compártelo por WhatsApp.
5. (Opcional) Para que WhatsApp muestre vista previa, en `index.html` cambia `content="assets/preview.jpg"` por la URL completa, p. ej. `https://TU-USUARIO.github.io/invitacion/assets/preview.jpg`.

## Alternativa: Cloudflare Pages
1. https://pages.cloudflare.com → *Create a project* → **Direct Upload**.
2. Sube la carpeta completa → *Deploy*. Obtendrás un enlace `https://nombre.pages.dev`.

## Importante
- La música **solo funciona desde un enlace https** (no al abrir `index.html` como archivo local): YouTube bloquea sus reproductores incrustados en `file://`.
- Para probar en tu computadora: `python3 -m http.server` dentro de la carpeta y abre http://localhost:8000.
- Cada cambio que hagas, vuelve a subirlo y se verá en minutos.
