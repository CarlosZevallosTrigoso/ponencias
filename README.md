# ponencias

Lector y anotador de ponencias en markdown, publicado con GitHub Pages.

- `index.html`: lista de ponencias, lector y anotador en un solo archivo.
- `ponencias/`: aquí van los `.md`. Sin front matter (`---`) al inicio.
- `ponencias.json`: plantilla que Jekyll convierte en la lista de archivos en cada publicación. No se edita a mano.
- `_config.yml`: impide que Pages convierta los `.md` en HTML.
- `vendor/marked.umd.js`: marked 18.1.2, local para no depender de un CDN.

Pages debe publicar con **Settings → Pages → Source: Deploy from a branch** (`main`, `/ (root)`). Con «GitHub Actions» o con un archivo `.nojekyll`, `ponencias.json` no se genera.

Las anotaciones se guardan en el navegador de cada equipo. Para moverlas entre equipos: exportar .json y cargar .json.
