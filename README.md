# pasteflow-landing

Landing page pública de PasteFlow, servida por GitHub Pages. Sitio estático plano — sin build, sin dependencias.

## Vista previa local

```bash
open index.html
```

## Publicar

Cualquier push a `main` se refleja automáticamente en `https://mriveaux.github.io/pasteflow-landing/` (GitHub Pages).

## Publicar una nueva versión del `.dmg`

`pasteflow-app` es un repo privado, así que su página de Releases no es visible públicamente. El binario descargable vive como Release **en este repo**:

```bash
gh release create vX.Y.Z "/ruta/al/PasteFlow_X.Y.Z_universal.dmg" \
  --repo mriveaux/pasteflow-landing \
  --title "PasteFlow vX.Y.Z" \
  --notes "Ver CHANGELOG en el repo principal."
```

El botón de descarga de la landing apunta a `/releases/latest`, que siempre redirige a la versión más reciente publicada aquí.
