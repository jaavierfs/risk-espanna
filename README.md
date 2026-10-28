# Risk España

Prototipo web de un juego de estrategia inspirado en Risk, con un mapa de las provincias de España. Está pensado para ejecutarse en Safari en iPad y en navegadores de escritorio.

## Estado actual: versión 0.3

- Mapa con geometrías provinciales reales cargadas desde un GeoJSON público.
- Selección de provincias mediante toque o clic.
- Reparto inicial de territorios y tropas.
- Refuerzos, ataques con dados y movimiento de tropas.
- Oponente controlado por una IA sencilla.
- Vista separada para Canarias, Ceuta y Melilla.
- Guardado y carga local de la partida mediante `localStorage`.

## Cómo publicarlo con GitHub Pages

1. Sube `index.html` a la raíz del repositorio.
2. En GitHub, entra en **Settings → Pages**.
3. En **Build and deployment**, selecciona **Deploy from a branch**.
4. Elige la rama `main` y la carpeta `/(root)`, y guarda los cambios.
5. Abre la URL de GitHub Pages en Safari. Si no aparece la versión nueva, recarga la página.

## Requisitos y limitaciones

- La conexión a Internet es necesaria para descargar los límites provinciales del GeoJSON externo.
- Es un prototipo: las reglas y la IA son simplificadas y no reproducen exactamente las del Risk del vídeo de referencia.
- Las fronteras compartidas se utilizan para estimar adyacencias terrestres; se añaden conexiones marítimas manuales para islas y ciudades autónomas.
- La geometría cartográfica procede del proyecto público `codeforamerica/click_that_hood`, archivo `spain-provinces.geojson`. Para una versión de producción, convendría verificar y sustituir estos datos por una fuente oficial del IGN/CNIG.

## Próximos pasos recomendados

- Probar en Safari de iPad el mapa, los controles táctiles y el guardado/carga.
- Revisar las adyacencias provinciales y las conexiones marítimas.
- Mejorar el modo multijugador local, la IA y el equilibrio de las reglas.

## Licencia y atribución

Este repositorio es un prototipo. Antes de redistribuirlo como producto, revisa las condiciones de licencia del código y de los datos cartográficos utilizados.
