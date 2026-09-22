# METRIX · El Protocolo de la Medida Perdida

Tutor socrático gamificado sobre mediciones y sistemas de unidades para estudiantes que ingresan a universidades del Ecuador.

**[Abrir METRIX](https://mguerreroz-rgb.github.io/metrix/)** · [Actividad](https://mguerreroz-rgb.github.io/metrix/jugar/) · [Guía docente](https://mguerreroz-rgb.github.io/metrix/guia-docente.html)

## La experiencia

- Un participante por sesión, con selección de avatar.
- Cuatro misiones y veinte desafíos; duración orientativa de 60–75 minutos.
- Tutoría socrática, dos intentos y hasta cuarenta puntos.
- Narración, música, contraste alto y texto ampliado.
- Diploma y reporte descargables en PDF.
- Progreso y preferencias guardados en el navegador del dispositivo.

## Estructura y uso local

- `index.html`, `portal.css`: portada del recurso.
- `jugar/`: experiencia interactiva con todos sus recursos locales.
- `guia-docente.html`: orientaciones para el aula e impresión.
- `documentos/`: PDF original de instrucciones.
- `descargas/`: ZIP web y ejecutable Windows originales, sin modificaciones.

Para usar la actividad sin conexión, descomprime el ZIP de `descargas/` y abre su `index.html`. La página publicada necesita internet para descargar inicialmente sus recursos. La narración depende de las voces disponibles en el dispositivo.

El repositorio de publicación contiene `metrix-site.zip` con estos archivos web, junto con los dos paquetes originales descargables. GitHub Actions extrae el sitio, incorpora las descargas, ejecuta `jugar/verify.mjs` y publica el resultado en GitHub Pages. Para actualizar la web, modifica sus fuentes y reemplaza `metrix-site.zip`. No requiere claves de API. [Configuración de GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Adaptación web (septiembre de 2026)

Se añadieron portada, guía docente, navegación y descargas, conservando las veinte preguntas, las cuatro misiones y los recursos originales. La versión de `jugar/` permite continuar si el navegador bloquea el almacenamiento, conserva el estado tras el primer error y pide confirmación antes de sustituir una sesión iniciada. El ejecutable Windows se distribuye tal como fue suministrado; no se ha ejecutado para la publicación.

Comprobación original de contenido y recursos: `node jugar/verify.mjs`.

## Autoría y licencia

Marcos Guerrero · Leonor Sánchez · Bryan Valarezo  
Universidad Estatal de Milagro

Creative Commons Atribución-NoComercial-CompartirIgual 4.0 Internacional ([CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es)). Se mantiene la atribución y la licencia del recurso original. La biblioteca jsPDF conserva su aviso de licencia incluido en `jugar/assets/vendor/jspdf.umd.min.js`.
