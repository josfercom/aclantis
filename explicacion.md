# Explicación del Proyecto - Evaluación Integral

En este documento explico cómo he reestructurado y finalizado el sitio web de **Aclantis Group** para cumplir con todos los requerimientos de la **Evaluación Integral**, mejorando notablemente la versión entregada en la Evaluación Continua 4.

---

## 1. Estructura y Organización (Requisito cumplido)
Para mantener un proyecto ordenado y profesional, separé todos los recursos en carpetas específicas:
* El archivo `index.html` se mantiene en la raíz principal.
* Creé la carpeta `pages/` donde moví todas las páginas secundarias (`nosotros.html`, `servicios.html`, `beneficios.html` y `contacto.html`).
* Creé la carpeta `css/` donde ubiqué mi hoja de estilos `style.css`.
* Esto me obligó a actualizar con mucho cuidado todas las rutas relativas en los enlaces (ej. `href="../css/style.css"`).

---

## 2. Navegación y 5 Páginas Funcionales
En el PA4, algunas opciones de mi menú solo hacían "scroll" hacia abajo en la misma página. Para este trabajo final:
* Eliminé los anclajes de scroll.
* Ahora el menú cuenta con **5 opciones** (Inicio, Nosotros, Servicios, Beneficios y Contacto) y **cada una lleva a una página HTML física e independiente**.
* En todas las páginas mantuve la estructura semántica de `<header>`, `<nav>`, `<main>` y `<footer>` para conservar la consistencia.

---

## 3. Integración de Herramientas Obligatorias
Reescribí gran parte del código para integrar las librerías modernas exigidas en la rúbrica:

* **Bootstrap 5.3**: Lo utilicé en todas las páginas para estructurar el contenido rápidamente sin tener que hacer Flexbox manual. Usé el sistema de grillas (`row`, `col-md-4`, etc.), las utilidades de espaciado (`py-5`, `mb-4`) y componentes como `Card` y botones (`btn-primary`).
* **Font Awesome**: Eliminé los emojis que usaba antes y los reemplacé por íconos vectoriales profesionales (ej. `<i class="fa-solid fa-map-pin"></i>`).
* **AOS (Animate On Scroll)**: Agregué la librería AOS a todas mis páginas. Ahora, a medida que el usuario hace scroll, las tarjetas y textos van apareciendo con efectos como `fade-up` o `fade-right`, dándole un toque mucho más dinámico y premium.
* **Google Fonts**: Seguí utilizando la tipografía *Poppins* para darle un aspecto moderno a todo el sitio.
* **UIColors**: Usé la herramienta para generar y afinar mi paleta de tonos azules corporativos.

---

## 4. Diseño, CSS Limpio y Recursos Visuales
Me aseguré de no tener "código zombie" ni duplicado. 

* **Limpieza Absoluta del CSS**: Al integrar Bootstrap, mucho de mi CSS antiguo ya no era necesario. Borré todas las líneas de código inútil y dejé mi archivo `style.css` súper limpio (apenas 70 líneas). Solo conservé mis variables de colores (`:root`), y algunas clases de microinteracciones (`.hover-lift` y `.bounce-animation`).
* **Imágenes de Alta Calidad**: Tomando en cuenta el feedback de la evaluación pasada ("Las imágenes son un elemento importante..."), inyecté imágenes profesionales libres de derechos de *Unsplash*. 
* **Simulador de Google Maps**: Perfeccioné la sección principal (Hero) del inicio. Diseñé un simulador visual interactivo combinando una imagen de mapa real de fondo, un "popup" de reseña simulado y un icono animado, logrando que destaque de inmediato el propósito de la agencia.

---

## 5. Repositorio en GitHub
A lo largo de este refactor, hice commits claros para reflejar mis avances de forma ordenada en mi repositorio. El proyecto está finalizado, es 100% responsivo y está listo para ser revisado.
