#Desarrollo Del Proyecto sobre HTML con CSS en una pagina.
Proyecto iniciado el 19 de octubre.

Maqueta web estática de la fundación Patitas Felices (rescate, cuidado y adopción de animales), hecha solo con HTML y CSS, sin JavaScript. El diseño se hizo primero en Figma (wireframes en la carpeta `wireframes/`) y luego se pasó a código.

Cómo ejecutarlo
Abrir la carpeta `patitas-felices` en Visual Studio Code.
Instalar la extensión Live Server.
Clic derecho en `index.html` → Open with Live Server.
(También se puede abrir `index.html` con doble clic en el navegador.)
Estructura

patitas-felices/
├── index.html
├── views/        adopta.html, perfil.html, contacto.html
├── css/          variables.css, style.css, home.css, adopta.css, perfil.css, contacto.css
├── storage/img/  imágenes
├── wireframes/   diseño de Figma (1440 px)
└── README.md


Diseño responsive
Se diseñó primero para celular y se fue agregando con `min-width`:
600 px: celulares grandes (el catálogo pasa a 2 columnas)
768 px: tablet (el menú, el banner y misión/visión pasan a fila)
1024 px: computador (el catálogo pasa a 4 columnas y el formulario queda al lado de los datos)

Componentes simulados con CSS
Carrusel: 3 fotos que se turnan con `@keyframes`, una cada 3 segundos.
Filtros: 4 -select- con estilos (solo visuales, no filtran).
Validación del formulario: `:placeholder-shown`, `:valid` e `:invalid`, y las clases `.error` y `.success` en un bloque de ejemplo.
Footer con Flexbox y catálogo/galería con Grid.
