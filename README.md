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

**Correcciones realizadas:**

### Página 3

**Errores encontrados:**
- El documento estaba configurado con `lang="en"`, aunque su contenido estaba escrito en español.
- El nombre de la imagen contenía un espacio (`TEMA 3.jpg`), lo que generaba un error en el atributo `src`.
- Se utilizaba el atributo `border="1"` en las tablas, considerado obsoleto por el estándar HTML.

**Correcciones realizadas:**
- Se cambió `lang="en"` por `lang="es"` para indicar que la página está escrita en español.
- Se cambió el nombre de la imagen de `TEMA 3.jpg` a `TEMA-3.jpg` y se actualizó la ruta en el atributo `src`.
- Se eliminó el atributo `border="1"` de las tablas.
