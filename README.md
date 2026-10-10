# Martha Martínez | Ropa hecha a mano

Sitio web de Diseños y Creaciones Martha Martínez, publicado con GitHub Pages.

- Sitio: https://racso.github.io/martha-martinez/
- Las prendas se cargan desde el panel administrativo (Apps Script, `?vista=panel`) y se guardan en Google Sheets.
- Este sitio las lee desde la URL del script configurada en `CONFIG.apiUrl` dentro de `index.html`.
- Los pedidos se envían al mismo script, que los guarda en la pestaña "Pedidos" y avisa por correo.

Para actualizar el diseño, edita `index.html` y sube el cambio a la rama `main`.
