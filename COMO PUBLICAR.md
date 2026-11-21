# Publicar el panel y la app con link fijo (gratis)

Esta carpeta son páginas web normales, como tus otros tableros. Se conectan a la planilla por detrás y **no usan tus cuentas de Google**, así que abren siempre, con todas tus cuentas abiertas.

| Página | Link final (ejemplo) | Para quién |
|---|---|---|
| `panel.html` | `https://TU-SITIO/panel.html` | Tú: panel de cobros y bodegaje |
| `index.html` | `https://TU-SITIO/` | Conductores: se instala en el teléfono con el ícono HDE Stange |

## Paso 1: actualizar el código en Apps Script (una vez)
El código ahora tiene una "puerta" para estas páginas.
1. Pega `PARA COPIAR/1 Codigo.txt` en `Código.gs` (reemplaza todo) y guarda.
2. **Implementar > Gestionar implementaciones > Editar > Versión: Nueva versión > Implementar.**

## Paso 2: poner tu URL en config.js
Abre `config.js` con el Bloc de notas y pega tu URL `/exec` (botón **Copiar** de "Aplicación web", sin `?p=admin`) entre las comillas. Guarda.

## Paso 3: subir la carpeta
Súbela al mismo lugar donde tienes tus otros tableros. Si es GitHub Pages:
1. En github.com: **+ > New repository**, nombre `hde-stange`, **Public**, **Create repository**.
2. **uploading an existing file**: arrastra todos los archivos de esta carpeta (menos este .md) > **Commit changes**.
3. **Settings > Pages > Branch: main / (root) > Save**. En 1 o 2 minutos aparece el link.

## Paso 4: usar
- **Panel:** guarda `…/panel.html` en favoritos. Entra con tu PIN de administrador.
- **Conductores:** mándales `…/` (la raíz). En Android aparece **Instalar app** (o menú de tres puntos > Instalar app); en iPhone, Safari > Compartir > **Agregar a inicio**. Entran con el PIN 1216.

Si más adelante cambias el diseño o el código de las páginas, se sube de nuevo esta carpeta. El link no cambia.
