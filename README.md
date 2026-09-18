# Listo para imprimir — Snap Shot

Todo en **PETG**, 0.2 mm de capa, 100 % de relleno en las piezas del mecanismo (705, 706,
707) y 40 % o más en el resto. Cada archivo aquí está revisado y no va a cambiar. Faltan
solo los clips de sujeción al gancho, la caja de la electrónica y el soporte de pantalla.

## Primero, para elegir los ajustes

| Archivo | Cant. | Nota |
|---|---|---|
| `105_socket_gauge.stl` | 1 | Cupón: prueba los zócalos y elige el diámetro antes de imprimir los rieles |
| `104_dowel_pin_card.stl` | 1 | Tarjeta con 6 pasadores en 3 diámetros: elige el que entre a presión en la mitad A y deslice en la B, antes de unir la barra |

## Barra principal (la columna vertebral, lleva las cámaras)

| Archivo | Cant. | Impresión | Nota |
|---|---|---|---|
| `101_bar_half_A.stl` | 1 | Cara inferior sobre la cama, canal hacia arriba | Mitad trasera, X 0–178.4 |
| `102_bar_half_B.stl` | 1 | Igual | Mitad delantera, X 178.4–356 |
| `103_channel_lid_A.stl` | 1 | Plana | Tapa del canal, mitad A |
| `103_channel_lid_B.stl` | 1 | Plana | Tapa del canal, mitad B |
| `601_camera_clamp.stl` | 2 | Marco hacia abajo | Sujetador de la cámara, uno por cámara |

**La cámara tiene una sola orientación correcta.** El escalón donde apoya lleva un pin que
entra en uno de los agujeros del módulo: bien puesta, la placa asienta a fondo; girada,
queda 1.5 mm levantada y los tornillos no entran. Si no asienta, gírala, no la fuerces.

**Unión de las mitades:** el pasador se mete **a fondo en la mitad A** (entra 15.5 mm) y
la mitad B se desliza sobre los 4.5 mm que sobresalen. Está hecho así a propósito: el
tornillo del poste central pasa a 1.2 mm del asiento en B.

## Postes

| Archivo | Cant. | Impresión | Nota |
|---|---|---|---|
| `401_post_outer.stl` | 4 | De pie, con el pie sobre la cama | Postes exteriores, ambos lados |
| `402_post_mid.stl` | 2 | De pie, con el pie sobre la cama | Poste central; los dos cubos horizontales del eje pueden necesitar un soporte corto |

## Rieles

| Archivo | Cant. | Nota |
|---|---|---|
| `501_rail_A_seg1_chamfer_L.stl` | 1 | Riel A trasero, lado +Y |
| `501_rail_A_seg1_chamfer_R.stl` | 1 | Riel A trasero, lado −Y |
| `501_rail_A_seg2_chamfer_L.stl` | 1 | Riel A delantero, lado +Y |
| `501_rail_A_seg2_chamfer_R.stl` | 1 | Riel A delantero, lado −Y |
| `502_rail_B1_rear.stl` | 2 | Riel B trasero, uno por lado |
| `503_rail_B2_front.stl` | 2 | Riel B delantero, uno por lado |

De costado, con la cara exterior sobre la cama.

## Barras de ArUco

| Archivo | Cant. | Marcadores que lleva |
|---|---|---|
| `701_fiducial_bar_rear_L.stl` | 1 | IDs 1 y 3 |
| `701_fiducial_bar_rear_R.stl` | 1 | IDs 0 y 2 |
| `702_fiducial_bar_front_L.stl` | 1 | IDs 5 y 7 |
| `702_fiducial_bar_front_R.stl` | 1 | IDs 4 y 6 |

Cara exterior sobre la cama; la cara superior con los rebajes no se toca. Los marcadores de
papel: `aruco_markers_print_at_100pct.svg`, **al 100 %, sin ajustar a página**, en papel
mate. Son de 5 mm; se pegan en los rebajes de 7.1 mm.

## Mecanismo de la palanca

| Archivo | Cant. | Impresión | Nota |
|---|---|---|---|
| `705_splice_A_L.stl` / `705_splice_A_R.stl` | 1 c/u | Columna vertical, cabeza arriba | Carro del riel A |
| `705_splice_B_L.stl` / `705_splice_B_R.stl` | 1 c/u | Igual | Carro del riel B |
| `706_crank.stl` | 4 | Plana | |
| `504_lift_lever_A.stl` | 1 | Plana | Una marca |
| `504_lift_lever_B.stl` | 1 | Plana | Dos marcas |
| `707_detent_ring.stl` | 2 | **Cara del saliente hacia abajo, pivotes arriba** | Al sacarlo, flexiona el brazo con el dedo: debe ceder con presión suave. Si no cede, avisar antes de montar |

## Total: 28 impresiones + la hoja de ArUco

Un tirón normal de la palanca necesita medio newton. **Si no se mueve, no está trabada:
algo está mal. No la fuerces** (límite 15 N en el mango).

### Vigilar en la primera impresión
- El labio de 0.5 mm junto a la ranura del LED en la barra: un perímetro, sin carga; si el slicer lo omite, no importa.
- El voladizo de 2 mm bajo el escalón de la cámara, dentro de la barra.
- El sujetador de cámara: al apretar debe flexionar ligeramente; si queda plano sin resistencia, avisar.
