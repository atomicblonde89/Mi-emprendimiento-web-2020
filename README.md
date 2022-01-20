# Mi-emprendimiento-web-2020
_**Prueba final CSS Avanzado**_

![gif](https://github.com/atomicblonde89/Mi-emprendimiento-web-2020/blob/main/assets/img/gitAnimacion.gif)

# **Mockups**

* [Mobile](https://github.com/atomicblonde89/Mi-emprendimiento-web-2020/blob/main/assets/img/mobile-mockup.png)

* [Desktop](https://github.com/atomicblonde89/Mi-emprendimiento-web-2020/blob/main/assets/img/desktop-mockup.png)

* [Style Guide](https://github.com/atomicblonde89/Mi-emprendimiento-web-2020/blob/main/assets/img/style-guide.pdf)
# Requerimientos
1. Desarrollar la estructura base del proyecto en HTML. **(1 Punto)**

● Crea la carpeta base del proyecto con el archivo index.html y la carpeta de
assets con sus respectivas subcarpetas y archivos, es decir, dentro de assets
se debe crear las carpetas “css para el resultado de la compilación, img para
las imágenes en SVG o PNG y sass para las subcarpetas abstracts, base,
components, layout, pages, themes, vendors y el archivo main.scss.

● Implementa etiquetas semánticas para definir las distintas secciones de la
página.

● Indentar el código y ordenar la carga de archivos en el index.html.

2. Implementar en la estructura HTML de la maqueta la nomenclatura de clases de
acuerdo a la metodología BEM. **(1 Punto)**

3. Utilizar SASS para modularizar y organizar estilos de CSS dando aspecto visual al
documento. **(2 Puntos)**

● Emplear el patrón 7-1 para modularizar y organizar SASS.

● Separar la lógica visual del proyecto usando parciales, directivas @import y
manifiesto.

● Crear variables, implementar nesting, parent selector y mixins.

4. Crear una grilla usando la propiedad de CSS denominada “Grid”, para luego ser
aplicada en los elementos de HTML que permiten visualizar un diseño responsivo de
acuerdo a los resultados finales de la página web mostrado en las imágenes del
archivo de apoyo.  
**(2 Puntos)**

● Crea un archivo exclusivo para el sistema de grillas en SASS.

● Agregar las clases correspondientes de la grilla a los elementos del
documento HTML que requieran trabajar con grillas para ser responsivo.

5. Utilizar flexbox para posicionar y alinear elementos en la maqueta que permitan
obtener una página web responsiva. **(2 Puntos)**

6. Implementar transiciones y animaciones al elemento SVG indicado en la imagen
animada con la extensión “.gif”. **(1 Punto)**

● Separar los @keyframes de animaciones en el directorio base con un archivo
único para las animaciones.

7. Crear media queries bajo breakpoints que permitan visualizar la página web en
cualquier tamaño de dispositivo. **(1 Punto)**


## SASS/
~~~
https://sass-guidelin.es/es/#arquitectura

sass/
|
|– base/
|   |– _reset.scss       # Reset/normalize
|   |– _typography.scss  # Reglas tipográficas
|   …                    # Etc.
|
|– components/
|   |– _buttons.scss     # Botones
|   |– _carousel.scss    # Carousel
|   |– _cover.scss       # Cubierta
|   |– _dropdown.scss    # Dropdown
|   …                    # Etc.
|
|– layout/
|   |– _navigation.scss  # Navegación
|   |– _grid.scss        # Sistema de retícula
|   |– _header.scss      # Encabezamiento
|   |– _footer.scss      # Pie de página
|   |– _sidebar.scss     # Barra lateral
|   |– _forms.scss       # Formularios
|   …                    # Etc.
|
|– pages/
|   |– _home.scss        # Estilos específicos para la página de inicio
|   |– _contact.scss     # Estilos específicos para la página de contacto
|   …                    # Etc.
|
|– themes/
|   |– _theme.scss       # Tema por defecto
|   |– _admin.scss       # Tema del administrador
|   …                    # Etc.
|
|– utils/
|   |– _variables.scss   # Variables Sass
|   |– _functions.scss   # Funciones Sass
|   |– _mixins.scss      # Mixins Sass
|   |– _helpers.scss     # Clases & placeholders
|
|– vendors/
|   |– _bootstrap.scss   # Bootstrap
|   |– _jquery-ui.scss   # jQuery UI
|   …                    # Etc.
|
|
`– main.scss             # Archivo principal de Sass
~~~

## PARA IMPORTAR LOS PARCIALES

- @import 'abstracts/variables';
- @import 'abstracts/mixins';
- @import 'base/base';
- @import 'base/reset';
- @import 'base/typography';
- @import 'layout/header';
- @import 'layout/main-section.scss';
- @import 'layout/forms';
- @import 'components/buttons';
- @import 'components/inputs';
- @import 'pages/home';
- @import 'pages/contact';
- @import 'themes/theme';
- @import 'themes/admin';

## REALIZAR LA COMPILACIÓN
- `sass --watch styles.scss:styles.css`
