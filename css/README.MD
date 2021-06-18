Reglas CSS

Selector, propiedad y valor
más de un selector
Tipos de Selectores

- => Global
  etiqueta => h1,h2 body
  clase => .title, se pone un nombre
  #id=> id y se pone #
  [atributo]=> selector por un atributo

selector de grupo
#title, .sub-title{
color:red
}

-combinados
Descendente
body .title{
color
}

hijo directo=> primer nivel luego de body
body > .title{
color: red
}

hermano
h1~h2{
color: red
}

+adyacente =>más proxímo
h1 + h2 {
color:red
}

:PseudoClase
h1:hover{
color:red
}

::PseudoElemento
h1 ::after{
content:"\_"
}
h1::before{
content:"-"
}

User Agent Styles
Tienen estilos por defecto, eso depende del navegador

Cascada
dos reglas per
.title{
color:red;
}
.title{
color:orange;
}

especificidad
h2{
color:orange
}

el id es superior a la clase

h2.title es mucho más específico

h2{
color: green !important; sobre escribe todo
}

Herencia
hereda de todo un ejmeplo es el body
bodymain
solo algunas etiquetas heredan
color
fuente

Content / Component / Layout

Display/flujo/línea y bloque

Display

flow layout Diseño de Flujo
Flex y grid otro curso

display: block; Esperan ocupar todo el espacio en su línea
display: inline; Solo ocupan el espacio físico en la línea
dislay: inline-block

Flow : obedece al writing-mode y direction
Se siente como el agua
Valores lógicos, para un cambio de idiomas

Medidas
https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units
formas de representar valores
absolutos:
PIXEL= px
Relativos más o menos px
em = valor de fuente más cercano asignado
rem= siempre toma el valor del padre superior y solo de ese

Resolución de la pantalla
1920x1080

pseudo Clases y estilo de texto
https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-classes

Custom Propierties
Ayudarán a almacenar datos para ser reutilizados por referencia en múltiples partes
https://developer.mozilla.org/es/docs/Web/CSS/--*
