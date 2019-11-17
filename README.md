# curl
[ejemplos](http://programandolo.blogspot.com/2013/08/herramienta-curl-en-el-interprete-de.html)

#!/bin/bash

### EJECUTAR DESDE CONSOLA

Get los response y guardar en archivo y poner salto linea al final.

> curl localhost:8080/greeting -w "\n" >> salida.json

_Get los response de la llamada pero usando como name llamadas desde 1 a 10_

```
curl localhost:8080/greeting?name=[1-10] -w "\n" >> nuevo.json
```

_Igual que el anterior, pero crea un archivo para cada llamada_

> curl localhost:8080/greeting?name=[1-10] -w "\n" -o nuevo#1.html

**Get las response de cada llamada, pero usando texto como param**

```
curl localhost:8080/greeting?name={"ana","pedro"} -w "\n" >> respuestas.json
```

Igual que el anterior, pero crea un archivo para cada llamada

<code> curl localhost:8080/greeting?name={"ana","pedro"}[1-2] -w "\n" -o unicos#1.json
</code>

Enlace para la sintaxis de markdown: [IR](https://markdown.es/sintaxis-markdown/)

<code>altGr+4 para escribir ~~~ delimitar código</code>
