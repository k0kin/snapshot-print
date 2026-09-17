# Listo para imprimir — Snap Shot

Todo en **PETG**, 0.2 mm de capa, 100 % de relleno en las piezas del mecanismo (705, 706,
707) y 40 % o más en el resto. Cada archivo aquí está revisado y no va a cambiar. Los postes
y la barra principal se añadirán cuando estén cerrados.

## Primero, para elegir el ajuste

| Archivo | Cant. | Nota |
|---|---|---|
| `105_socket_gauge.stl` | 1 | Cupón: prueba los zócalos y elige el diámetro antes de imprimir los rieles |

## Rieles

| Archivo | Cant. | Nota |
|---|---|---|
| `501_rail_A_seg1_chamfer_L.stl` | 1 | Riel A trasero, lado +Y |
| `501_rail_A_seg1_chamfer_R.stl` | 1 | Riel A trasero, lado −Y |
| `501_rail_A_seg2_chamfer_L.stl` | 1 | Riel A delantero, lado +Y |
| `501_rail_A_seg2_chamfer_R.stl` | 1 | Riel A delantero, lado −Y |
| `502_rail_B1_rear.stl` | 2 | Riel B trasero, uno por lado |
| `503_rail_B2_front.stl` | 2 | Riel B delantero, uno por lado |

## Barras de ArUco

| Archivo | Cant. | Marcadores que lleva |
|---|---|---|
| `701_fiducial_bar_rear_L.stl` | 1 | IDs 1 y 3 |
| `701_fiducial_bar_rear_R.stl` | 1 | IDs 0 y 2 |
| `702_fiducial_bar_front_L.stl` | 1 | IDs 5 y 7 |
| `702_fiducial_bar_front_R.stl` | 1 | IDs 4 y 6 |

Los marcadores de papel: `aruco_markers_print_at_100pct.svg`, **al 100 %, sin ajustar a
página**, en papel mate. Son de 5 mm; se pegan en los rebajes de 7.1 mm de cada barra.

## Mecanismo de la palanca

| Archivo | Cant. | Nota |
|---|---|---|
| `705_splice_A_L.stl` / `705_splice_A_R.stl` | 1 c/u | Carro del riel A, +Y / −Y |
| `705_splice_B_L.stl` / `705_splice_B_R.stl` | 1 c/u | Carro del riel B, +Y / −Y |
| `706_crank.stl` | 4 | |
| `504_lift_lever_A.stl` | 1 | Una marca |
| `504_lift_lever_B.stl` | 1 | Dos marcas |
| `707_detent_ring.stl` | 2 | **Muesca hacia abajo.** Al sacarlo, flexiona el brazo con el dedo: debe ceder con presión suave. Si no cede, avisar antes de montar |

## Total de piezas: 20 impresiones + la hoja de ArUco

## Orientación de impresión

- Rieles (501, 502, 503): de costado, con la cara exterior sobre la cama.
- Barras de ArUco (701, 702): cara exterior sobre la cama; la cara superior con los rebajes queda arriba y no se toca.
- Carros (705): con la columna vertical, cabeza arriba.
- Manivelas (706) y palancas (504): planas.
- Anillo de detente (707): **muesca hacia abajo**.
Un tirón normal de la palanca necesita medio newton. **Si no se mueve, no está trabada:
algo está mal. No la fuerces** (límite 15 N en el mango).
