# Martha Martínez | Ropa hecha a mano

Sitio web de Diseños y Creaciones Martha Martínez, publicado con Cloudflare Pages.

- Sitio: https://martha-martinez-disenos.pages.dev/ (Cloudflare Pages, se publica solo desde la rama `main`)
- El enlace viejo (racsoscar.github.io/martha-martinez) redirige al nuevo.
- Las prendas se cargan desde el panel administrativo (Apps Script, `?vista=panel`) y se guardan en Google Sheets.
- Este sitio las lee desde la URL del script configurada en `CONFIG.apiUrl` dentro de `index.html`.
- Los pedidos se envían al mismo script, que los guarda en la pestaña "Pedidos" y avisa por correo.

Para actualizar el diseño, edita `index.html` y sube el cambio a la rama `main`.

## Estampados

- La fila del panel con categoría **Estampados** no se muestra como prenda: es la lista de diseños que la clienta puede agregar a cualquier prenda.
- **Precio** de esa fila = valor que se suma por estampado.
- **Fotos**: la primera es la portada (collage) y no se muestra; las demás son los diseños, en orden: Diseño 1, Diseño 2…
- Si la fila está como **Agotado**, la opción de estampado desaparece de todas las prendas.
- Lugares disponibles: pecho izquierdo rectangular (3 × 5 cm), pecho izquierdo cuadrado (4 × 4 cm) y centro del torso (4 × 12 cm).
- El estampado elegido llega en el pedido al inicio de las notas (diseño, lugar y total) y también en los campos `estampado`, `estampadoLugar`, `estampadoPrecio` y `total`.
