## Guía de traducción
Traducir puede resultar una tarea relativamente sencilla pero una traducción de calidad ha de respetar ciertas normas. Este documeto incluye una serie de normas para hacer que el contenido de toda la traducción sea homogéneo y lo más estandarizado posible.

Por favor, leer con atención todos los apartados de esta guía.

### Evitar pronombres

A la hora de escribir, se intentará evitar la utilización de pronombres lo máximo posible. 

La razón por la que se deben evitar es para intentar estandarizar los diferentes pronombres para las diferentes variantes del lenguaje. En algunas variantes del idioma se utiliza `vos`, en otras `tu`, en otras `usted`, etc... Evitando estos pronombres conseguiremos una forma más cercana a la aceptada por todas las variantes.

Para traducir la cadena:

```
Note that we are able to inject any dependencies we need into the command's constructor.
---
Correcto:
Tener en cuenta que se puede inyectar cualquier dependencia que se necesite en el constructor del comando.
---
Incorrecto:
Tengamos en cuenta que podemos inyectar cualquier dependencia que necesitemos en el constructor del comando.
```

Así mismo otro ejemplo:

```
If you need to ask the user for a simple confirmation, you may use the <0>confirm</0> method.
---
Correcto:
Si es necesario solicitar al usuario una confirmación simple, se puede utilizar el método <0>confirm</0>.
---
Incorrecto:
Si necesitamos preguntar al usuario por una confirmación simple, podemos utilizar el método <0>cofirm</0>.
```

### Bloques de código

A pesar de que este proyecto se encarga de traducir la documentación de Laravel de ingés a español, desde Laraveles se recomienda que se programe utilizando el idioma inglés. Programando de este modo, el código podrá ser leido por prácticamente cualquier persona, pues el vocabulario que se utiliza suele ser muy similar, además de crear una armonía al no mezclar dos idiomas en una misma sentencia:

```php
// Correcto
$user = User::find(1);
// Incorrecto
$usuario = Usuario::find(1);
```

Al traducir un bloque de código, se debe dejar tal cual aparece en la documentación. De forma opcional se pueden traducir los comentarios o información de los docblocks.

### Traducciones sugeridas y traductores

La plataforma CrowdIn ofrece siempre una traducción más o menos acertada sobre la cadena que se desea traducir. Normalmente esta sugerencia no es acertada al 100%, pues se está trabajando sobre lenguaje bastante técnico y no se espera encontrar `table` como `mesa` ni otras erratas por el estilo.

Se ruega encarecidamente que se eviten estas sugerencias así como traducciones automáticas de otros motores como `Google` o `Bing`. Si bien se pueden utilizar como guía y apoyo a la traducción, se espera que las traducciones se aporten de forma manual y coherente.

### Nomenclatura natural del lenguaje

La mayoría de lenguajes de programación están desarrollados en el idioma sajón por excelencia, inglés. A la hora de traducir, es a menudo complicado encontrar una traducción acertada para ciertos conceptos que ni siquiera existen en otros idiomas. Es por ello que no se deben traducir conceptos nativos del lenguaje como por ejemplo:

- Array
- Closure
- Schema
- Type-hint
- ...

Y así cualquier otro elemento que sea común al lenguaje de programación. Cualquier progrmador debe conocer estos términos en el idioma base. Traducirlos, una vez mas puede inducir a confusión, pues de nuevo las diferentes variedades del lenguaje los traducen de formas diferentes.

Teniendo en cuenta esto, veamos un ejemplo:

```
The second argument passed to helper is an array of data that should be made available to the view.
---
Correcto:
El segundo parámetro es un array de datos que deberán estar disponibles en la vista.
---
Incorrecto:
El segundo argumento es un arreglo de datos que deberán estar disponibles en la vista.
```

### Ortografía y gramática

Otro de los problemas comunes a la hora de traducir es la cantidad cantidad de aportaciones que se realizan sin haber comprobado la ortografía y gramática de éstas.

Revisar que efectivamente la aportación que se está realizando cumple con las reglas ortográficas y gramaticales del idioma es fundamental para que sea aprobada por un moderador. El no comprobar lo que se está aportando afecta de forma directa al proyecto de traducción, pues un moderador deberá emplear parte de su tiempo en corregir las sentencias en lugar de contribuir directamente al proyecto con nuevas traducciones u otras tareas.

Por favor, revisar todas las aportaciones, no hay un premio al usuario que más traducciones aporte ni se va a convertir en un reconocimiento.
