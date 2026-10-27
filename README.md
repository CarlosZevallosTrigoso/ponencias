# ponencias

Lector y anotador de ponencias en markdown, publicado con GitHub Pages.

- `index.html`: lista de ponencias, lector y anotador en un solo archivo.
- `ponencias/`: aquí van los `.md`. Sin front matter (`---`) al inicio.
- `anotaciones/`: los `.json` exportados, con el mismo nombre que su ponencia (`ponencias/x.md` → `anotaciones/x.json`). Se cargan solos al abrir la ponencia.
- `ponencias.json`: plantilla que Jekyll convierte en la lista de archivos en cada publicación. No se edita a mano.
- `_config.yml`: impide que Pages convierta los `.md` en HTML.
- `vendor/marked.umd.js`: marked 18.1.2, local para no depender de un CDN.

Pages debe publicar con **Settings → Pages → Source: Deploy from a branch** (`main`, `/ (root)`). Con «GitHub Actions» o con un archivo `.nojekyll`, `ponencias.json` no se genera.

El botón **timer** muestra un timer flotante: se arrastra desde cualquier punto, cambia de tamaño desde la esquina inferior derecha y suma minutos con +1 y +5.

Las anotaciones se guardan en el navegador de cada equipo. Para tenerlas en todos: exportar .json y subirlo a `anotaciones/`.
