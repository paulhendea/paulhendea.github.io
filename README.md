# MEGÒC web project
El proyecto se ha realizado usando PUG, CSS, y JS en conjunto con algunas librerías como [FontAwesome](https://fontawesome.com/) y [Glider.js](https://nickpiscitelli.github.io/Glider.js/).
El sitio web consta de 5 páginas a las que podemos acceder a través del menú de navegación.

## PUG
El motor de plantillas PUG ha sido de gran ayuda a la hora de evitar código duplicado entre las diferentes páginas del sitio web. Ya que todas ellas tienen elementos en común como pueden ser la barra de navegación, el menú desplegable, el pié de página, o el banner de cookies.
Gracias a pug podemos escribir el código relacionado a estos elementos en archivos diferentes y simplemente incluirlo en nuestras páginas mediante `include`.
También facilita tanto la escritura como la lectura y análisis del código ya que es más sencillo y legible.

## CSS
En este caso se ha empleado CSS puro aunque una opción de mejora sería implementar tecnologías como SASS que nos facilte la escritura de código CSS.
Tenemos un archivo `css/styles.css` que contiene todo el código necesario para mostrar correctamente los elementos comunes a todas las páginas. Además, para cada página en particular también disponemos de un archivo css particular que nos ayuda a darle formato a los contenidos específicos de dicha página.
En resumen tenemos un archivo común a todas las páginas y un archivo específico para cada una de ellas.

## JS
Igual que pasa con css, nos encontramos con un archivo `js/main.js` que sirve para dotar de funcionalidad común a las páginas de nuestro sitio web, y para aquellas páginas que necesiten una funcionalidad más específica encontramos un archivo .js específico.
En el fichero común encontramos código para poner y quitar la clase `open` en el menú de navegación y de esta forma mostarlo y ocultarlo mediante eventListeners. También encontramos código para ajustar la posición de los botones para cambiar el idioma y las redes sociales según el mediaQuery. Finalmente también se encuentra aquí la lógica para trabajar con los cookies y mostrar u ocultar el banner.
En cuanto a los archivos para páginas más específicas encontramos `js/carousel.js` y `js/calendar.js` que se encargan de implementar los carouseles de la web mediante la librería Glider.js y de dotar de funcionalidad a la lista estilo acordeon de la seción 'Próximas actuaciones' respectivamente.

### FontAwesome
Se usa simplemente para agregar algunos iconos a la web (redes sociales, flechas, etc).

### Glider.js
Se usa para implementar los carouseles de la web, es muy útil ya que permite modificar las opciones del carousel según el tamaño de la página, lo cual lo convierte en una herramienta perfecta para desarrollar carouseles responsive.
