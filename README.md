# TDE NFC – Ficha de vehículo

Landing page estática que muestra los datos de un vehículo a partir de los parámetros de la URL grabada en la etiqueta NFC.

## Formato de la URL

Claves largas:

```
https://ruttosa.github.io/tde-nfc/?vin=9BRA78BF8V3006997&motor=2TBR391947&color=ROJO&pedido=NBQ2435&modelo=TGN156L-SDMLK&anio=2026
```

Claves cortas (recomendadas para etiquetas pequeñas como NTAG213):

```
https://ruttosa.github.io/tde-nfc/?v=9BRA78BF8V3006997&m=2TBR391947&c=ROJO&p=NBQ2435&mo=TGN156L-SDMLK&a=2026
```

| Campo  | Clave larga | Clave corta |
|--------|-------------|-------------|
| VIN    | `vin`       | `v`         |
| Motor  | `motor`     | `m`         |
| Color  | `color`     | `c`         |
| Pedido | `pedido`    | `p`         |
| Modelo | `modelo`    | `mo`        |
| Año    | `anio`      | `a`         |

Sin parámetros, la página muestra los datos de ejemplo.

## Publicación

El workflow `.github/workflows/pages.yml` despliega el sitio en GitHub Pages en cada push.
En **Settings → Pages → Build and deployment → Source** debe estar seleccionado **GitHub Actions**.
