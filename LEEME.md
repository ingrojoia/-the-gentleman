# The Gentleman — Agenda (prototipo 0.1)

Agenda privada y local para una sola profesional. Incluye vista diaria/semanal/mensual, citas flexibles, detección de traslapes, búsqueda de espacios y respaldos JSON. No incluye precios, cuentas ni reservas de clientes.

## Probar en computadora

Abre `index.html` en un navegador moderno. IndexedDB guarda las citas localmente. Para probar el service worker, sirve el directorio en localhost (por ejemplo, `python -m http.server 8000`) y abre `http://localhost:8000`.

## Instalar en iPhone

Publica **los cuatro archivos de la carpeta juntos** en un hosting estático con HTTPS, abre la dirección en Safari, pulsa Compartir > Añadir a pantalla de inicio > Abrir como app. El alojamiento solo distribuye los archivos; las citas quedan en el almacenamiento local del iPhone. Tras cargar por primera vez, prueba el modo avión para verificar que el contenido se abre sin conexión.

## Importante

- No abras el archivo `index.html` directamente en iPhone desde Archivos: para instalación PWA se necesita HTTPS.
- La información **no se sincroniza** entre dispositivos.
- Exporta respaldos frecuentemente. Borrar datos del sitio, desinstalar la web app o determinadas políticas de almacenamiento de iOS pueden eliminar las citas.
- El horario de búsqueda de huecos es de 9:00 a 19:00; las citas pueden registrarse a cualquier hora del día.
- No se admiten citas que crucen medianoche ni citas simultáneas; los tintes con tiempos de espera se modelarán en una futura versión.
- Antes de uso profesional, verifica el flujo de instalación y persistencia en el iPhone real.
