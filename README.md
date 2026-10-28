# Risk España

Prototipo web de un juego de estrategia inspirado en Risk, con territorios provinciales españoles. Está pensado para Safari en iPad y navegadores de escritorio.

## Versión 0.4 — mapa corregido

- Proyección uniforme para la Península y Baleares, evitando estirar el mapa de forma distinta en horizontal y vertical.
- Recuadros separados para Canarias, Ceuta y Melilla.
- Geometrías provinciales reales cargadas desde GeoJSON.
- Selección táctil, refuerzos, ataques con dados, movimiento básico y una IA sencilla.
- Guardado y carga local en el navegador.

## Publicación con GitHub Pages

1. Sube `index.html` y `README.md` a la raíz de la rama `main`.
2. En GitHub, entra en **Settings → Pages**.
3. Selecciona **Deploy from a branch**, rama `main` y carpeta `/(root)`.
4. Abre la URL de GitHub Pages en Safari y recarga la página.

## Fuente de los datos geográficos

El mapa se carga desde el GeoJSON público de [Code for America / click_that_hood](https://github.com/codeforamerica/click_that_hood/blob/master/public/data/spain-provinces.geojson). Hace falta conexión a Internet para cargar las fronteras.

## Limitaciones

- Es un prototipo; reglas y estrategia de la IA simplificadas.
- Las conexiones marítimas entre territorios son aproximadas y se definen manualmente.
- La posición de algunas etiquetas puede necesitar ajustes visuales en pantallas pequeñas.
- Para un producto final, conviene validar las fronteras con datos oficiales del IGN/CNIG e incorporar el GeoJSON al proyecto para no depender de un servicio externo.
