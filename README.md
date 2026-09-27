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



