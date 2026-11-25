# sanq-strokes

Stroke-order data for 4,250 Chinese characters (simplified and traditional), as used by [SanQ](https://sanq.app), the app to learn Mandarin Chinese in Spanish.

Datos de orden de trazos de 4.250 caracteres chinos (simplificados y tradicionales), tal como los usa [SanQ](https://sanq.app), la app para aprender chino mandarín en español.

## Origin / Origen

The data comes from `graphics.txt` in [Make Me a Hanzi](https://github.com/skishore/makemeahanzi). That project derived it from the fonts **AR PL KaitiM GB** and **AR PL UKai** by Arphic Technology Co., Ltd.

Los datos provienen de `graphics.txt` de [Make Me a Hanzi](https://github.com/skishore/makemeahanzi), que los obtuvo de los fonts **AR PL KaitiM GB** y **AR PL UKai** de Arphic Technology Co., Ltd.

## Modifications / Modificaciones

These files are a modified version of the original data (Arphic Public License, section 2):

- **2026-07-03:** extracted one JSON file per character, for the characters of the SanQ vocabulary (simplified).
- **2026-07-20:** added the traditional forms (+1,248 characters).
- Each file is named after the character's Unicode codepoint in hex (`4e00.json` = 一).
- The `character` field was removed. The `strokes` (SVG outlines) and `medians` (centre lines) values are **unchanged**.
- Each file carries an `aviso` field that states these changes.

Estos archivos son una versión modificada de los datos originales (Arphic Public License, sección 2):

- **2026-07-03:** se extrajo un archivo JSON por carácter, para los caracteres del vocabulario de SanQ (simplificado).
- **2026-07-20:** se sumaron las formas tradicionales (+1.248 caracteres).
- Cada archivo lleva por nombre el codepoint Unicode del carácter en hexadecimal (`4e00.json` = 一).
- Se eliminó el campo `character`. Los valores de `strokes` (contornos SVG) y `medians` (líneas medias) **no cambiaron**.
- Cada archivo incluye un campo `aviso` que describe estos cambios.

Format / Formato:

```json
{"aviso": "...", "strokes": ["M 518 382 Q ..."], "medians": [[[121,393],[193,372]]]}
```

## License / Licencia

Arphic Public License. See [ARPHICPL.txt](ARPHICPL.txt). You may copy, modify and redistribute these files under the terms of that license.

Arphic Public License. Ver [ARPHICPL.txt](ARPHICPL.txt). Puedes copiar, modificar y redistribuir estos archivos bajo los términos de esa licencia.

This repository contains only the data. The source code of the SanQ app is not part of it and is not covered by this license.

Este repositorio contiene solo los datos. El código de la app SanQ no forma parte de él ni está cubierto por esta licencia.
