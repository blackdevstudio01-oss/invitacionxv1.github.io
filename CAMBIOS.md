# Cambios para pantallas móviles

Fecha: 28 de octubre de 2026.

## Implementación
1. Se quitaron las alturas fijas de las secciones. La portada conserva una altura mínima y puede crecer con el contenido.
2. La fecha ya no está encerrada en un cuadrado con recorte. Su tamaño de letra es adaptable y el interlineado es mayor.
3. Las imágenes de contenido ahora usan elementos img con altura automática, dimensiones declaradas y texto alternativo; el listón decorativo tiene alt vacío.
4. Todas las secciones comparten un ancho máximo de 430 px, centrado y espacio lateral.
5. Los párrafos tienen tamaño e interlineado explícitos; sus saltos de línea se ajustan al ancho disponible. La fecha conserva sus tres líneas.
6. El nombre y el subtítulo están centrados y usan tamaños adaptables.
7. Se generaron cinco imágenes WebP, con calidad 85 y un tamaño máximo de 960 × 1600 px, conservando los PNG originales. Los archivos utilizados pasan de aproximadamente 7.73 MiB a 0.56 MiB (reducción cercana al 93 %). Las imágenes inferiores usan carga diferida.
8. El listón y el collage final conservan sus proporciones originales. El fondo floral de la portada usa cover para cubrirla; puede recortar parte de su borde decorativo según la altura.
9. Los botones se convirtieron en enlaces con href="" por petición del usuario. Se añadieron estados de pulsación y foco visible, una altura mínima de 48 px y se corrigió la unidad de la sombra.
10. El idioma del documento es español y se corrigieron acentos en los textos.

## Enlaces pendientes
En index.html, completar los href de .btn-mesage y .btn-rsvp cuando se tengan los destinos.
Actualmente un href vacío apunta al documento actual y puede recargarlo; no abre una ubicación ni envía una confirmación.

## Archivos
- index.html: estructura, imágenes, idioma y enlaces.
- style.css: adaptación a móviles y estados interactivos.
- assets/*.webp: versiones optimizadas.
- Los PNG originales se conservan como fuentes.

## Verificación
Se verificaron las rutas locales, la lectura de los cinco WebP y los dos enlaces vacíos.
La prueba automática en navegador no pudo ejecutarse: Chromium no está instalado en el entorno de pruebas y Edge no logró iniciar.
Queda pendiente la revisión visual en 320, 375, 390 y 430 px, orientación horizontal y texto ampliado al 200 %.
