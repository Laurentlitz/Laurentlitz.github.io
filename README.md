# Oracle Sales Play Academy

Versión preparada para GitHub Pages.

## Archivos

- `index.html`: sitio principal para GitHub Pages.
- `offline.html`: copia que puede descargarse y abrirse localmente.
- `.nojekyll`: evita procesamiento innecesario de Jekyll.

## Publicar en GitHub Pages

Repositorio recomendado:

`Laurentlitz/Laurentlitz.github.io`

1. Suba estos archivos a la rama `main`.
2. Abra **Settings > Pages**.
3. En **Build and deployment**, elija **Deploy from a branch**.
4. Seleccione:
   - Branch: `main`
   - Folder: `/ (root)`
5. Pulse **Save**.

El sitio debería quedar disponible como:

`https://laurentlitz.github.io/`

## Importante sobre Login y Register

La aplicación sigue usando almacenamiento local del navegador (`localStorage`).

Esto significa:

- cada navegador/dispositivo mantiene sus propios usuarios y progreso;
- registrar un usuario en una PC no lo registra automáticamente en otro teléfono;
- el login no es seguridad corporativa;
- GitHub Pages no proporciona una base de datos ni autenticación backend;
- no guarde secretos, contraseñas reales corporativas ni información sensible.

El HTML sigue pudiéndose descargar y usar sin conexión.
