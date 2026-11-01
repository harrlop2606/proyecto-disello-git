Lo primero que he hecho ha sido mirar la imagen del enunciado y el HTML que nos daban para ver qué clases traía ya puestas. Como no había que cambiar el HTML,
he trabajado solo en el archivo de estilos, usando esas clases tal cual.

Después he preparado lo básico: con `box-sizing: border-box` he hecho que el padding no agrande las cajas, con `margin: 0` he quitado los márgenes que pone el
navegador al body, y con `font-family` y `background-color` he elegido una letra sencilla y un fondo clarito. Con `list-style: none` he quitado las bolitas de las
listas. También he puesto `display: flex` y `flex-direction: column` al body con `min-height: 100vh`, y `flex: 1` al `main`, para que el contenido ocupe todo el
espacio libre y el pie se quede siempre abajo.

Luego he hecho la cabecera con `display: flex`. He movido el nombre "DAW Mobility" a la izquierda y el menú a la derecha con `justify-content: space-between`, y los
he centrado en vertical con `align-items: center`. Para que los enlaces del menú se pongan en fila he puesto `display: flex` a la lista, y para separarlos he usado
`gap`. A la página en la que estamos ("Solicitud") le he puesto `font-weight: 700` para la negrita y un `border-bottom` amarillo para la rayita. A todos los enlaces
les he puesto un borde transparente del mismo grosor para que no se muevan al aparecer la raya, y con `:hover` hago que se subrayen al pasar el ratón.

Por último he hecho el pie de página, igual que la cabecera: `display: flex` con `justify-content: space-between` para dejar el copyright a la izquierda y los
enlaces a la derecha, `gap` para separar los enlaces y `text-decoration: underline` para subrayarlos. Además he añadido un `@media (max-width: 700px)` en el que
cambio `flex-direction` a `column`, para que la cabecera y el pie se pongan uno debajo de otro cuando la pantalla es estrecha, y `flex-wrap: wrap` para que los
enlaces bajen de línea si no caben.
