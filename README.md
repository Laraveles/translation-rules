# Laraveles / docs

En _Laraveles_ hace tiempo que iniciamos el proceso para traducir la documetación de Laravel a español. Es por este tiempo y experiencia que ha surgido la necesidad de crear una _**Guía de Estilos**_ para las aportaciones a este proyecto.

Este documento pretende recopilar una serie de normas que hagan que el resultado de la traducción sea homogéneo y coherente en cuanto a las diferentes variedades del idioma Español se refiere.

La plataforma de traducción es libre y cualquier usuario puede registrarse y contribuir. Desde Laraveles **se ruega la lectura de este documento antes de realizar cualquier aportación** al proyecto.

Todas las aportaciones que no sigan la _**Guía de Estilos**_ serán descartadas de inmediato.

## Enlaces

Proyecto de traducción de Laravel a español: https://crowdin.com/project/laravel-documentation/es-ES

Documentación traducida en español: http://laraveles.com/docs

## Guía de traducción

Traducir puede resultar una tarea relativamente sencilla pero una traducción de calidad ha de respetar ciertas normas. Este documento incluye una serie de normas para hacer que el contenido de toda la traducción sea homogéneo, coherente y lo más estandarizado posible.

Por favor, leer con atención todos los apartados de esta guía.

### Evitar pronombres

A la hora de escribir, se evitará el _tuteo_, aunque se mantendrá un tono cordial siempre se utilizará el modo cortés, se tratará al usuario de _usted_ eliminando así las diferentes variantes del Español, esto es, se evitará `vos`, `tu`, y otras acepciones que pueda tener el Español. Únicamente será válido el uso de usted y su concordancia en cuanto a forma y número.

Para traducir la cadena:

```
Note that we are able to inject any dependencies we need into the command's constructor.
---
Correcto:
  Tenga en cuenta que puede inyectarse cualquier dependencia que se necesite en el constructor del comando.
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

A pesar de que este proyecto se encarga de traducir la documentación de Laravel de ingés a español, desde _Laraveles_ se recomienda que se programe utilizando el idioma inglés. Programando de este modo, el código podrá ser leido por prácticamente cualquier persona, pues el vocabulario que se utiliza suele ser muy similar, además de crear una armonía al no mezclar dos idiomas en una misma sentencia.

**LOS BLOQUES DE CÓDIGO NO SE TRADUCIRÁN**, se debe dejar tal cual aparece en la plataforma, en **ROJO**.

### Traducciones sugeridas y traductores

La plataforma _CrowdIn_ ofrece siempre una traducción más o menos acertada sobre la cadena que se desea traducir. Normalmente esta sugerencia no es acertada al 100%, ya que se está trabajando sobre lenguaje bastante técnico y no se espera encontrar `table` como `mesa` ni otras erratas por el estilo.

Se ruega encarecidamente que se eviten estas sugerencias así como traducciones automáticas de otros motores como `Google` o `Bing`. Si bien se pueden utilizar como guía y apoyo a la traducción, se espera que las traducciones se aporten de forma manual y coherente.

Como webs de referencia para comprobar y buscar el término más correcto en una traducción sugerimos que se utilice el sitio [Word Reference](URL "http://www.wordreference.com") 

### Nomenclatura natural del lenguaje

La mayoría de lenguajes de programación están desarrollados en el idioma sajón por excelencia. En multitud de ocasiones, Laravel utiliza una terminología propia que describe muchos de sus elementos y funcionalidades. 

Por eso, a la hora de traducir, es a menudo complicado encontrar una traducción acertada 
para ciertos conceptos que ni siquiera existen en otros idiomas. Es por ello que no se deben traducir conceptos nativos del lenguaje, o aquellas cuya traducción alteren el significado de la frase original. 

En este caso se escribirá el térnimo en el idioma original entre los símbolos <i> y </i> para que aparezca en cursiva y denote que no ha sido traducido a propósito, por ejemplo `<i>type-hint</i>` que debería verse como _type-hint_. A modo de _**orientación**_ se ofrece la siguiente tabla:

| Término     | Término           | Término           | 
|:------------|:------------------|:----------------- |
| timestamp   | closure           | render            |
| schema      | type-hint         | seed              |
| helper      | service provider  | service container |
| true        | false             | null              |
| login       | reset             | query builder     |
| facade      | join              | cache             |
| middleware  | accessor          | mutator           |
| slug        | scope             | constraint        |
| casting     | join              | timestamp         |

Y así cualquier otro elemento que sea común al lenguaje de programación. Cualquier programador debe conocer estos términos en el idioma base. Traducirlos, una vez más puede inducir a 
confusión, pues de nuevo las diferentes variedades del lenguaje los traducen de formas diferentes.

Teniendo en cuenta esto, veamos un ejemplo:

```
The second argument passed to helper is an array of data that should be made available to the view.
---
Correcto:
El segundo parámetro es una matriz de datos que debería hacerse disponibles en la vista.
---
Incorrecto:
El segundo argumento es un arreglo / array de datos que deberán estar disponibles en la vista.
```
  
### Ortografía y gramática

Otro de los problemas comunes a la hora de traducir es la cantidad de aportaciones que se realizan sin haber comprobado la ortografía y gramática de estas.

Revisar que efectivamente la aportación que se está realizando cumple con las reglas ortográficas y gramaticales del idioma es fundamental para que sea aprobada por un moderador. No comprobar lo que se está aportando afecta de forma directa al proyecto de traducción, pues un moderador deberá emplear parte de su tiempo en corregir las sentencias en lugar de contribuir directamente al proyecto con nuevas traducciones u otras tareas.

Por favor, revisar todas las aportaciones y preguntad en los canales de Slack en caso de duda. No hay un premio al usuario que más traducciones aporte ni se va a convertir en un reconocimiento.

### Títulos y cabeceras

La traducción de los títulos se realizará conforme cualquier otra frase, esto es, **salvo que la palabra esté comienzo de frase, a continuación de un punto o sea nombre propio, no deberá escribirse con mayúsculas**. Un ejemplo lo tenemos en el siguiente fragmento.

```
- Installation
- Configuration
  · Basic Configuration
  · Environment Configuration
  · Configuration Caching
  · Accessing Configuration Values
  · Naming Your Application
- Maintenance Mode
```

Quedaría así:

```
- Instalación
- Configuración
  · Configuración básica
  · Configuración de entorno
  · Configuración de caché
  · Accediendo a los valores de configuración
  · Nombrando tu aplicación
- Modo de mantenimiento
```

## Moderadores

Existen moderadores que además de participar en el proceso de traducción, revisan y validan las aportaciones que realiza cada uno de los miembros. Actualmente son:

* @IsraelOrtuno
* @codeAtBusiness 

## Contribuir

Cualquier aportación a esta guía es más que bienvenida. Tan solo con hacer pull-request será evaluada o bien contactar con alguno de los administradores para debatir el tema.