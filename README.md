# ud1ej2dwec
## Unidad 1 ej3

### async vs defer attributes

async y defer se utiliza para controlar el comportamiento de los scripts en HTML.

async: El script se descarga de manera asíncrona mientras el HTML se sigue analizando. Una vez que se descarga, se ejecutará sin esperar a que se complete el análisis del HTML.

defer: El script se descarga de manera asíncrona, pero se ejecuta después de completar  el análisis del HTML. Si hay varios scripts defer, se ejecutan en el orden en el que aparecen en el HTML.

### Especificación whatwg.org:

La especificación HTM("WhatWG HTML") es un documento que describe cómo se debe interpretar HTML por los navegadores web.

### Dónde poner las etiquetas script en HTML:

Normalmente, se colocan las etiquetas script dentro del elemento head o al final del elemento body en el HTML.

El head se utiliza para scripts críticos que deben cargarse antes de que se vea cualquier parte de la página.
El body es común para scripts no críticos que no bloquean la visualización de la página.

### Etiqueta noscript:

La etiqueta noscript se utiliza para mostrar un contenido diferente al que se muestra cuando JavaScript está deshabilitado en el navegador del usuario.
Puedes colocar contenido dentro de noscript que se verá si JavaScript está deshabilitado. 

### Subresource Integrity (SRI):

SRI es una característica que permite al navegador verificar que los archivos descargados, como  los scripts, no han sido modificados desde que fueron entregados por el servidor. Esto hace apelamiento principalmente a los hashes (SHA256 MD5 SHA1).

### Descarga de jQuery. Genera la etiqueta script con los atributos integrity y crossorigin usados para el control Subresource Integrity (SRI). 

\<script src="mi-script.js" integrity="hash-del-archivo" crossorigin="anonymous"></script>

### Ventajas de incorporar scripts desde un archivo externo:

Mejora la reutilización del código.

Facilita el mantenimiento del código.

Reduce la complejidad del código.

### Atributos aplicables a la etiqueta \<script>:

Algunos atributos comunes son src, async, defer, integrity, crossorigin, type, y charset.

### Atributos por defecto:
El atributo por defecto es type="text/javascript".

### Atributos booleanos:

Son async y defer, si se incluyen en la etiqueta se dan por activados.

### Sitio recomendado para colocar la etiqueta script.

Depende del nivel de crítico del script, si es muy importante en la etiqueta head, si no en el final del body.

### Etiqueta noscript: utilidad, atributos y dónde colocar

Se utiliza para contenido alternativo cuando el usuario no tiene Javascript activado, no tiene atributos y se coloca al final del body 
