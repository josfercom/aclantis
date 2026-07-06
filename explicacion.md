# Explicación de mi Proyecto - PA4

En este documento explico cómo he construido el sitio web de **Aclantis Group** para la Evaluación Continua 4, agregando nuevas páginas y ampliando el contenido del proyecto inicial de PA3.

---

## 1. Temática del Sitio Web (Requerimiento 1)
Mi sitio web está enfocado en **Aclantis Group**, una agencia que ayuda a pequeños negocios (como tiendas, restaurantes y consultorios locales) a posicionarse en las búsquedas de Google Maps. 
* **¿Por qué elegí este tema?**: Hoy en día, cuando la gente busca un lugar cercano para comprar, abre Google Maps desde su celular. Considero que este servicio es de gran utilidad para los pequeños negocios que quieren conseguir más clientes en su propia zona sin gastar mucho dinero.

---

## 2. Menú de Navegación o Navbar (Requerimiento 2)
Diseñé una barra de navegación en la parte superior que tiene **5 opciones** bien organizadas:
1. **Inicio**: Te lleva a la pantalla de bienvenida con la simulación del mapa.
2. **Nosotros**: Explica quiénes somos y nuestro propósito.
3. **Servicios**: Detalla qué hacemos (mejorar el perfil, conseguir reseñas y analizar la competencia).
4. **Beneficios**: Muestra por qué a un negocio le conviene estar en Google Maps.
5. **Contacto**: Lleva a un formulario de contacto y a los datos de la agencia.

---

## 3. Estructura HTML del Sitio (`index.html`) (Requerimiento 3)
El archivo `index.html` cuenta con las etiquetas estructurales y semánticas de HTML5 para ordenar la información:
* **`<header>`**: Contiene el nombre del negocio (logo) y el menú de navegación para poder desplazarse por la web.
* **`<nav>`**: Dentro de la cabecera, agrupa la lista de enlaces de navegación de forma ordenada (`<ul>`, `<li>`, `<a>`).
* **`<main>`**: Es el cuerpo principal del sitio. Dentro de él agrupé las 5 secciones de la página usando la etiqueta `<section>` y les puse IDs únicos (como `id="inicio"` o `id="contacto"`) para enlazarlas al menú.
* **`<footer>`**: El pie de página que muestra los derechos de autor de Aclantis Group y una nota sobre el curso.

---

## 4. Estilos y Diseño Visual (`style.css`) (Requerimiento 3)
Para la hoja de estilos, apliqué los temas avanzados y básicos de CSS aprendidos en clase:

* **Variables CSS (`:root`)**: Creé variables al inicio del código para guardar los colores de la marca (como el azul para botones y tonos grises para los textos y fondos). Esto me ayudó a tener un código ordenado y poder cambiar un color en toda la página con solo modificar una línea.
* **Selectores por Clase e ID**: Usé IDs (`#header`, `#inicio`, etc.) para estructurar secciones de navegación y clases (`.boton`, `.tarjeta-servicio`, etc.) para dar estilos comunes a elementos repetitivos de forma limpia.
* **Márgenes y Rellenos (Margin y Padding)**: Usé `padding` para darle aire interno a las secciones y cajas, evitando que los textos se vean apretados. Usé `margin` para separar títulos y párrafos externamente.
* **Flexbox para Alinear Elementos**: Usé Flexbox en varios puntos del sitio para que el diseño sea ordenado y moderno:
  1. En el **Header** (`display: flex` y `justify-content: space-between`), para que el logo se vaya a la izquierda y el menú a la derecha de forma automática.
  2. En el **Hero** (sección de Inicio), para colocar los textos a un lado y la simulación del mapa al otro, centrados a la misma altura.
  3. En las **Tarjetas de Servicios**, para alinearlas de forma horizontal. Usé `flex-wrap: wrap` para que si se reduce la pantalla (como en un celular), las tarjetas se acomoden una debajo de la otra.

---

## 5. Diseño Adaptivo y Git (Requerimiento 4 y 5)
* **Adaptación a Celulares**: Al final de mi archivo CSS configuré reglas para que en pantallas de celulares o tablets los elementos se apilen de forma vertical (`flex-direction: column`) y se adapten sin crear barras de desplazamiento incómodas hacia los lados.
* **Subida a GitHub**: Inicialicé el repositorio en mi consola (`git init`), añadí todos los archivos (`git add .`), realicé el commit obligatorio con el mensaje `"Primer commit examen"` y lo subí a la rama `main` de mi cuenta de GitHub para completar la entrega.

---

## 6. PA4: Nuevas Páginas (nosotros.html y servicios.html)
Para la segunda etapa del proyecto, agregué dos páginas nuevas que tienen contenido más detallado:

### Página: Nosotros (nosotros.html)
En esta página agregué:
* **Seccion Hero**: Una introduccion sobre el equipo de Aclantis Group con un titulo llamativo.
* **Mision y Vision**: Tres tarjetas que muestran la mision, vision y valores de la empresa. Las tarjetas tienen un efecto hover que las eleva un poco.
* **Por qué elegirnos**: Una lista con 4 razones principales. Cada razon tiene un borde azul en la izquierda para que se vea mas interesante.
* **Datos de la empresa**: Una grilla con 4 estadisticas (negocios posicionados, años, clientes satisfechos, soporte).

### Página: Servicios (servicios.html)
En esta página mostré todos los servicios que ofrece Aclantis:
* **Servicios principales**: Las 3 tarjetas de servicios pero ahora con mas detalles y precio aproximado en cada una.
* **Servicios adicionales**: Una lista numerada con 4 servicios extra (auditoria gratuita, gestion mensual, fotos, campañas).
* **Planes de precios**: Una comparativa con 3 planes diferentes (Basico, Profesional, Premium). El plan Profesional está destacado porque es el mas popular.

### Estilos CSS utilizados
Para estas dos páginas no creé CSS nuevo inecesario. Solo agregué las clases que faltaban:
* `.tarjeta-valor` - Para las tarjetas de mision y vision
* `.razon-item` - Para los items de razones con borde azul
* `.estadisticas-grid` - Grid de 4 columnas para las estadisticas
* `.servicio-fila` - Para los servicios adicionales en fila
* `.planes-comparativa` - Grid de 3 columnas para los planes

Todas estas clases reutilizan las variables de color y estilos base que ya tenia en el archivo CSS principal.

### Estructura y Links
* El header y footer son identicos en todas las paginas para mantener consistencia.
* Los links del navbar ahora apuntan a las nuevas paginas: `nosotros.html` y `servicios.html`.
* Desde cualquier pagina se puede volver al inicio con el logo.
* Todo sigue siendo responsive con media queries adaptadas para celular.
