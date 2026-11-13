# Plazas turísticas en Málaga

Mapa web de las viviendas turísticas, hoteles, hostales, apartamentos y demás alojamientos inscritos en el Registro de Turismo de Andalucía en el término municipal de Málaga, dibujados sobre los edificios del Catastro.

Es una página estática: no necesita compilación ni servidor propio.

- Ver en local: `npx serve .` o `python3 -m http.server` y abrir `http://localhost:3000` (o `:8000`).
- Publicar: importar este repositorio en Vercel (Framework Preset «Other», sin comando de build, directorio raíz `./`).

## Ficheros

- `index.html`: la página (MapLibre GL desde unpkg, mapa base OpenFreeMap).
- `vut.txt`: viviendas turísticas inscritas (sin titulares ni contactos).
- `alojamientos.txt`: hoteles, hostales, apartamentos, albergues, casas rurales y campings.
- `edificios.txt`: edificios del Catastro (INSPIRE) usados para situar y colorear.
- `direcciones.txt`: callejero y portales del Catastro para el buscador.
- `tiles/`: teselas de respaldo por si OpenFreeMap no responde.
- `vercel.json`: cabeceras de caché.

## Fuentes

- Registro de Turismo de Andalucía, API OpenRTA de datos abiertos de la Junta de Andalucía (consulta del 13/11/2026).
- Catastro, conjuntos INSPIRE de edificios y direcciones del municipio 29900 (13/11/2026).
- Mapa base © OpenFreeMap, © OpenMapTiles, © colaboradores de OpenStreetMap.

Elaborado por Álvaro Carrillo.
