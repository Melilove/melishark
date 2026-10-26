# Melishark 🦈 — v2.1.1
App personal para aprender de tiburones. Creada por **melitalove**.
Es una PWA: se instala en el celular o el computador y funciona sin conexión.

## Qué hay en esta carpeta
- `index.html` — toda la app
- `manifest.webmanifest` — nombre, íconos y colores al instalar
- `sw.js` — modo sin conexión
- `icons/` — íconos de la app
- `fonts/` — tipografías incluidas (no dependen de internet)
- `GUIA-FOTOS.md` — cómo y dónde conseguir fotos con licencia, y la lista de 60 especies

## Publicar en GitHub Pages
1. Crea un repositorio nuevo en GitHub (por ejemplo `melishark`).
2. Sube **el contenido** de esta carpeta (que `index.html` quede en la raíz del repo, no dentro de otra carpeta).
3. En el repo: **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, carpeta `/ (root)`. Guarda.
4. En uno o dos minutos tendrás la dirección `https://TU-USUARIO.github.io/melishark/`.

> Las rutas son relativas, así que funciona dentro de una subcarpeta como `/melishark/`.
> El modo sin conexión y la instalación solo funcionan por **HTTPS** (GitHub Pages lo es). Abriendo `index.html` directo desde el computador la app funciona, pero sin instalación ni offline.

## Instalar
- **iPhone (Safari):** botón Compartir → *Añadir a pantalla de inicio*.
- **Android (Chrome):** menú ⋮ → *Instalar app*, o el botón "Instalar app" en la pestaña **Tú**.
- **Computador (Chrome/Edge):** ícono de instalar en la barra de direcciones.

## Subir de versión
Cuando cambies algo, actualiza el número en **dos** lugares (deben ser iguales):
1. `index.html` → `const APP_VERSION = '2.1.1';`
2. `sw.js` → `const VERSION = '2.1.1';`

Así el celular descarga la versión nueva y borra la anterior.

## Tus datos
Perfil, pines, bitácora y rango se guardan **solo en el dispositivo** (localStorage). Las fotos del Álbum también (IndexedDB), así que **no están en el repositorio** ni se suben a GitHub. No hay servidor. Si instalas la app en otro dispositivo, empieza de cero.
En iPhone, instala la app en la pantalla de inicio: así Safari no borra las fotos guardadas.

## Estado de conservación
Los estados (UICN) de cada especie son referenciales y pueden cambiar con nuevas evaluaciones.

## Licencias de tipografías
- Special Elite — Apache 2.0
- Libre Baskerville — SIL Open Font License 1.1
