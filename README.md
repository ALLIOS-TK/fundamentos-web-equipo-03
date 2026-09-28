# fundamentos-web-equipo-03

## Validación HTML

### Página 1

**Errores encontrados:**
- El documento estaba configurado con `lang="en"`, aunque su contenido estaba escrito en español.
- Se utilizaba el atributo `border="1"` en las tablas, considerado obsoleto por el estándar HTML.
- Se utilizo el atributo `center` en imagenes y la tabla, considerado obsoleto por el estandar HTML.
- Se utilizaba `p` en listas `ol` y `ul`, este atributo no es aceptado en las listas mencionadas. 

**Correcciones realizadas:**
- Se cambió `lang="en"` por `lang="es"` para indicar que la página está escrita en español.
- Se eliminó el atributo `border="1"` de las tablas.
- Se eliminó el atributo `center` de las imagenes y la tabla.
- se elimino el atributo `p` de las listas en las que se presentaba.




### Página 2

**Errores encontrados:**
- El documento estaba configurado con `lang="en"`, aunque el contenido estaba escrito en español.
- Se utilizaba la etiqueta `<center>`, considerada obsoleta en HTML.
- Se colocaban etiquetas `<h2>`, `<h3>` y `<h4>` dentro de etiquetas `<p>`, provocando errores de estructura.
- La imagen utilizaba `width="30%"` y `height="30%"`. El validador esperaba valores numéricos para esos atributos.
- La tabla utilizaba el atributo `border="1"`, considerado obsoleto por el estándar HTML.
- La etiqueta `<caption>` de la tabla estaba mal estructurada: el `<h2>` se cerraba después de `</caption>`.
- La lista `<ul>` de las fuentes consultadas no estaba correctamente cerrada.
- Debido a los errores anteriores, el validador también detectaba elementos `<section>` y `<main>` sin cerrar correctamente.

**Correcciones realizadas:**
- Se cambió `lang="en"` por `lang="es"` para indicar que la página está escrita en español.
- Se eliminó la etiqueta `<center>` y se dejó directamente el encabezado `<h1>`.
- Se eliminaron las etiquetas `<p>` que envolvían los encabezados `<h2>`, `<h3>` y `<h4>`.
- Se cambiaron los valores `width="30%"` y `height="30%"` de la imagen por valores numéricos: `width="300"` y `height="300"`.
- Se eliminó el atributo `border="1"` de la tabla.
- Se corrigió la estructura del `<caption>` de la tabla.
- Se cerró correctamente la lista `<ul>` de las fuentes.
- Se revisó el cierre de las etiquetas `<section>`, `<main>` y demás elementos para que la estructura HTML quedara correctamente anidada.


### Página 3

**Errores encontrados:**
- El documento estaba configurado con `lang="en"`, aunque su contenido estaba escrito en español.
- El nombre de la imagen contenía un espacio (`TEMA 3.jpg`), lo que generaba un error en el atributo `src`.
- Se utilizaba el atributo `border="1"` en las tablas, considerado obsoleto por el estándar HTML.

**Correcciones realizadas:**
- Se cambió `lang="en"` por `lang="es"` para indicar que la página está escrita en español.
- Se cambió el nombre de la imagen de `TEMA 3.jpg` a `TEMA-3.jpg` y se actualizó la ruta en el atributo `src`.
- Se eliminó el atributo `border="1"` de las tablas.

# fundamentos-web-equipo-03

## Validación HTML

### Página 1

**Errores encontrados:**

* El documento estaba configurado con `lang="en"`, aunque su contenido estaba escrito en español.
* Se utilizaba el atributo `border="1"` en las tablas, considerado obsoleto por el estándar HTML.
* Se utilizó el atributo `center` en imágenes y la tabla, considerado obsoleto por el estándar HTML.
* Se utilizaba `p` en listas `ol` y `ul`, este atributo no es aceptado en las listas mencionadas.

**Correcciones realizadas:**

* Se cambió `lang="en"` por `lang="es"` para indicar que la página está escrita en español.
* Se eliminó el atributo `border="1"` de las tablas.
* Se eliminó el atributo `center` de las imágenes y la tabla.
* Se eliminó el atributo `p` de las listas en las que se presentaba.

### Convención CSS

Para el proyecto se utiliza una convención de nombres en inglés, escrita en minúsculas y utilizando el formato kebab-case. También se utiliza la metodología BEM para organizar los elementos relacionados.

Algunos de los nombres de clases definidos en el proyecto son:

.site-header
.site-header__title
.site-header__intro
.main-nav
.site-main
.topic-section
.site-footer

### Paleta de color

La página de Ciberseguridad utiliza principalmente una paleta basada en tonos azules y colores neutros, buscando proporcionar una apariencia relacionada con el ámbito tecnológico y facilitar la lectura del contenido.

Los colores principales definidos originalmente mediante variables CSS son:

Primary: #091d34
Secondary: #2f75b5
Accent: #0f6b78
Background: #f1f5f9
Surface: #c7d3df
Text: #000000
Border: #000000

### Prueba de cascada

Se puede realizar una prueba temporal para comprobar cómo funcionan la cascada y la especificidad de los selectores CSS.

Para la prueba se puede utilizar un elemento con un selector de elemento, una clase y un ID:

<h2 id="demo-title" class="demo-title">
    Prueba de cascada
</h2>

se realizo con estas reglas:
h2 {
    color: blue;
}

.demo-title {
    color: green;
}

#demo-title {
    color: purple;
}

estilo en linea:
<h2 id="demo-title" class="demo-title" style="color: orange;">
    Prueba de cascada
</h2>

### Resultados de la prueba:
* El selector de elemento h2 tiene menor especificidad.
* El selector de clase .demo-title tiene mayor especificidad que el selector de elemento.
* El selector de ID #demo-title tiene mayor especificidad que el selector de clase.
* El estilo en línea tiene prioridad sobre los selectores anteriores en esta prueba.

La prueba permite comprobar cómo la especificidad influye en la regla CSS que termina aplicándose cuando existen varias reglas dirigidas al mismo elemento.

### Validación CSS
**Errores encontrados:**
* La estructura original del documento HTML presentaba una organización incorrecta de las etiquetas <html>, <head> y <body>, lo que podía afectar la correcta interpretación del documento y de la hoja de estilos.
* El archivo HTML enlazaba la hoja de estilos mediante <link rel="stylesheet" href="css/style.css">, pero el enlace se encontraba fuera del elemento <head>.
**Advertencias encontradas:**
* La etiqueta <link> utilizada para enlazar la hoja de estilos no especificaba el atributo type="text/css". Actualmente, para una hoja de estilos CSS convencional, este atributo no es necesario, pero puede aparecer como recomendación dependiendo del validador utilizado.
* La hoja CSS contiene clases como .site-header, .main-nav, .site-main y .topic-section que originalmente no estaban asociadas a los elementos del HTML.
**Correcciones realizadas:**
* Se ubicó correctamente el elemento <link> dentro de <head>.
* Se reorganizó el documento para utilizar la estructura:
<!DOCTYPE html>
<html lang="es">

<head>
    ...
</head>

<body>
    ...
</body>

</html>
* Se verificó que la ruta de la hoja de estilos corresponda con la estructura del proyecto:
css/style.css
* Se reorganizaron los selectores CSS para que correspondan con los elementos que realmente existen en el HTML.
* Se mantuvieron las variables CSS utilizadas para definir la paleta de colores, facilitando la modificación global del diseño.
* Se mantuvieron las referencias utilizadas en la página, correspondientes a IBM y Microsoft, relacionadas con los contenidos de ciberseguridad.

### Página 2

**Errores encontrados:**

* El documento estaba configurado con `lang="en"`, aunque el contenido estaba escrito en español.
* Se utilizaba la etiqueta `<center>`, considerada obsoleta en HTML.
* Se colocaban etiquetas `<h2>`, `<h3>` y `<h4>` dentro de etiquetas `<p>`, provocando errores de estructura.
* La imagen utilizaba `width="30%"` y `height="30%"`. El validador esperaba valores numéricos para esos atributos.
* La tabla utilizaba el atributo `border="1"`, considerado obsoleto por el estándar HTML.
* La etiqueta `<caption>` de la tabla estaba mal estructurada: el `<h2>` se cerraba después de `</caption>`.
* La lista `<ul>` de las fuentes consultadas no estaba correctamente cerrada.
* Debido a los errores anteriores, el validador también detectaba elementos `<section>` y `<main>` sin cerrar correctamente.

**Correcciones realizadas:**

* Se cambió `lang="en"` por `lang="es"` para indicar que la página está escrita en español.
* Se eliminó la etiqueta `<center>` y se dejó directamente el encabezado `<h1>`.
* Se eliminaron las etiquetas `<p>` que envolvían los encabezados `<h2>`, `<h3>` y `<h4>`.
* Se cambiaron los valores `width="30%"` y `height="30%"` de la imagen por valores numéricos: `width="300"` y `height="300"`.
* Se eliminó el atributo `border="1"` de la tabla.
* Se corrigió la estructura del `<caption>` de la tabla.
* Se cerró correctamente la lista `<ul>` de las fuentes.
* Se revisó el cierre de las etiquetas `<section>`, `<main>` y demás elementos para que la estructura HTML quedara correctamente anidada.

### Página 3

**Errores encontrados:**

* El documento estaba configurado con `lang="en"`, aunque su contenido estaba escrito en español.
* El nombre de la imagen contenía un espacio (`TEMA 3.jpg`), lo que generaba un error en el atributo `src`.
* Se utilizaba el atributo `border="1"` en las tablas, considerado obsoleto por el estándar HTML.

**Correcciones realizadas:**

* Se cambió `lang="en"` por `lang="es"` para indicar que la página está escrita en español.
* Se cambió el nombre de la imagen de `TEMA 3.jpg` a `TEMA-3.jpg` y se actualizó la ruta en el atributo `src`.
* Se eliminó el atributo `border="1"` de las tablas.


## Convención CSS

Para el proyecto se utiliza una convención de nombres en inglés, escrita en minúsculas y utilizando el formato kebab-case. También se utiliza la metodología BEM cuando es conveniente para organizar los elementos relacionados.

Algunos ejemplos utilizados en el proyecto son:

* .site-header

* .site-header__title

* .site-header__intro

* .main-nav

* .site-main

* .topic-section

* .site-footer

Los nombres de las clases describen la función o el contenido del elemento para facilitar la comprensión y el mantenimiento del código.

## Paleta de color

Las tres páginas del proyecto utilizan una paleta basada principalmente en tonos azules y colores neutros, buscando mantener una apariencia visual coherente y facilitar la lectura de los contenidos.

* **Primary:** #17365d

* **Secondary:** #2f75b5

* **Accent:** #0f6b78

* **Background:** #f7f9fc

* **Text:** #1f2937

También se utilizan colores complementarios para superficies y bordes:

* **Surface:** #ffffff

* **Border:** #d0d7de

Los colores principales se encuentran centralizados mediante variables CSS en :root, lo que permite modificar la apariencia general del sitio desde un solo lugar.

La elección de colores busca proporcionar contraste, legibilidad y una apariencia coherente entre las tres páginas del proyecto, cuyos temas son Blockchain, Ciberseguridad y Realidad Virtual.

## Prueba de cascada

Se realizó una prueba temporal para comprobar cómo funciona la cascada y la especificidad de los selectores CSS.

Para la prueba se utilizó un elemento con un selector de elemento, una clase y un ID:

<h2 id="demo-title" class="demo-title">Prueba de cascada</h2>

Se probaron diferentes reglas:

h2 {
    color: blue;
}

.demo-title {
    color: green;
}

#demo-title {
    color: purple;
}

También se probó un estilo en línea:

<h2 id="demo-title" class="demo-title" style="color: orange;">
    Prueba de cascada
</h2>

**Resultados de la prueba:**

* Selector de elemento (h2): menor especificidad.

* Selector de clase (.demo-title): mayor especificidad que el selector de elemento.

* Selector de ID (#demo-title): mayor especificidad que el selector de clase.

* Estilo en línea (style): tiene prioridad sobre los selectores anteriores en esta prueba.

La prueba permitió comprobar cómo la especificidad influye en qué regla CSS termina aplicándose cuando existen varias reglas para el mismo elemento.

Después de realizar la prueba, los estilos utilizados exclusivamente para experimentar fueron retirados del CSS final del proyecto.

### Página 3

**Errores encontrados:**

* El validador CSS del W3C presentó un error al intentar acceder al archivo css/styles.css mediante una ruta local (file://localhost/css/styles.css), mostrando el mensaje Operation not permitted.

**Advertencias encontradas:**

* El elemento <link> utilizado para enlazar la hoja de estilos no tenía especificado el atributo type con el valor text/css.

**Correcciones realizadas:**

* Se agregó el atributo type="text/css" al elemento <link> encargado de enlazar la hoja de estilos CSS.

* Se verificó que la ruta utilizada para enlazar el archivo styles.css fuera correcta de acuerdo con la estructura del proyecto: css/styles.css.

* Se verificó que el archivo styles.css no utilizara reglas @import que pudieran generar problemas adicionales al momento de validar la hoja de estilos.

El error Operation not permitted corresponde al acceso del validador al archivo CSS mediante una ruta local. La ruta utilizada en el proyecto es correcta debido a que el archivo styles.css se encuentra dentro de la carpeta css, al mismo nivel que tema3.html.

