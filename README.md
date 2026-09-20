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
