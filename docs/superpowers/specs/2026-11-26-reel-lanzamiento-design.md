# Reel de lanzamiento: Martha Martínez

## Intención
El primer Reel se sentía plano porque solo mostraba prendas. Este debe sentirse como un **lanzamiento** que reúne tres cosas: la marca (hecho a mano), la colección (busos y hoodies) y la tienda en línea (pedir desde el celular).

## Objetivos / no objetivos / anti-objetivos
- **Objetivo:** un Reel vertical de 1080×1920, de 35 a 40 s, con ritmo, expectativa y revelación, que termine en el enlace del sitio.
- **No objetivo:** campaña de varios Reels, versión para el feed o para WhatsApp (se pueden hacer después).
- **Anti-objetivos:** alterar o inventar el aspecto de las prendas (no se usa IA generativa), mostrar precios inventados, generar costos o usar música con derechos de autor.

## Restricciones
- Costo $0: todo se genera en este entorno (Playwright + ffmpeg).
- Fotos reales del catálogo: 36 fotos de 600×800 (BU-002, BU-003, HO-003 a HO-008), tomadas del historial del repositorio. Por su baja resolución, nada de acercamientos mayores a ~1,6×.
- Tipografías y logo del sitio (Big Shoulders Display, Hanken Grotesk, logo color y claro). Paleta: vino #400C32, fondo #FBF9F8, dorado de costura #C9A24A.
- Zona segura de Instagram: el texto clave va entre y≈250 y y≈1550.

## Enfoques considerados
1. **Un video en tres actos (elegido):** cuenta la historia completa en un solo Reel, ideal para fijarlo en el perfil.
2. Campaña de 3 Reels cortos: más expectativa, pero exige publicar con constancia. Descartado por ahora.
3. Plugin de animación dibujada: cambia las prendas reales por ilustraciones. Descartado.

## Diseño (guion)
| Acto | Tiempo | Contenido |
|---|---|---|
| 1. Marca | 0–10 s | Fondo vino oscuro. Una línea de costura dorada se dibuja. Entran frases al ritmo: "Cortada a mano." / "Cosida a mano." / "Para quien la va a usar." Revelación del logo con un destello suave. |
| 2. Colección | 10–24 s | Cortes al ritmo: acercamientos a detalles (cierres, bolsillos, cordones); prendas que cambian de color en cada golpe; nombre de la prenda en grande; mosaico final con toda la colección y "Nueva colección". |
| 3. Tienda | 24–38 s | Celular con el sitio real (capturas del sitio local con las fotos reales): tocar una prenda → cambia el color → "Agregar estampado" → abrir la tabla de medidas. Cierre: "Ya disponible", "Pide en línea" y racsoscar.github.io/martha-martinez. |

- **Música:** pista original sintetizada por código (pulso grave + percusión suave + un arpegio), ~110 BPM; los cortes caen en los tiempos. Se exporta mezclada en el MP4.
- **Movimiento** (skill emil-design-eng): curvas ease-out fuertes en las entradas, nada de rebotes, duraciones de 200 a 500 ms en los elementos y cortes secos en el tiempo del compás.
- **Dirección visual** (skill frontend-design): contraste entre los actos oscuros (marca y cierre) y el acto claro (colección), tipografía display grande como protagonista y la costura dorada punteada como hilo conductor.
- **Portada** (skill canvas-design): un cuadro estático de 1080×1920 para la portada del Reel.

## Decisiones del constructor (mías, para revisar)
- Nombres de las prendas: los mismos descriptivos del primer video, hasta que Martha diga los reales.
- En las capturas del sitio no se ve ningún precio de prenda; solo se ve "+$5.000" del estampado, que sí es real.
- La salida queda en el scratchpad de la sesión, no en el repositorio.
