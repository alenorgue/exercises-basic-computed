# Ejercicios sobre _computed properties_ o estado derivado

Abre con Live Server cada uno de los ficheros index.html del ejercicio a ralizar.

## ¿Algo va mal?

0. Intenta no pedir la solución directa a la IA.
1. Asegurate de que has hecho bien el [setup]((https://vuejs.org/guide/quick-start.html#using-the-global-build)) , engoblado todo el HTML por un contenedor `<div id="app"></div>` 
2. Echa un vistazo a la consola del navegador. Normalmente sucede que nos olvidamos importar algo o hay un error de sintaxis
<img src="https://oscarm.tinytake.com/media/17910d3?filename=1753086794204_TinyTake21-07-2025-10-33-00_638886835924646084.png&sub_type=thumbnail_preview&type=attachment&width=615&height=486" title="Powered by TinyTake Screen Capture"/>

## 1-basic-name

Disponemos de dos _input_ en los que podemos poner el nombre y apellidos de una persona.
Mediante el uso de [computed properties](https://vuejs.org/guide/essentials/computed) calcula todos los estados derivados que puedes leer en el HTML

1. Combined name (ya está hecho)
2. Text Length: tamaño total del nombre y el apellido juntos 
3. Debe aparecer 'Yes' o 'No' en función de si el número de carácteres del nombre y el apellido juntos es par o impar
4. Debe aparecer 'Yes' si, entre el nombre y apellidos, contienen todas las vocales del abecedario.

<details>
  <summary>Pisa apartado 4</summary>
  - 'Pedro Murcielago" contiene todas las vocales
  - Hay un método de array perfecto para determinar si, _cada una de las vocales del abacedario_, estan contenidas en otro string
</details>

## 2-qa-list

Implementa un "Preguntas más frequentes" con buscador. Es el típico buscador que escribes una palabra clave y solo aparecen las pregutnas y respuestes que contienen la palabra clave, o bien en la pregunta, o bien en la respuesta.

1. Debes crear un estado derivado que, dado el término de búsqueda _searchTerm_ (acuérdate de usar searchTerm.value, faqs.value, etc), devuelve solamente aquellos elementos del array que contienen dicho término en la pregunta o en la respuesta (hay un método de array excelente para _filtrar_ esa información)
2. Substiuye tu estado derviado por el estado original en la directiva v-for

`<details v-for="(faq, index) in miEstadoDerivado" :key="index">`

## 3-dynamic-computed-style

Crea un componente que, en función del valor del selector de rango, rellena proporcionalmente la barra inferior.

1. Usa adecaudamente la directiva v-model para gobernar el valor del _input_ y mostrarlo en el HTML
2. Calcula un estado derivado que, en función del estado del input, rellena la barra inferior. Para el valor 0 del input rellena un 0%, para el 1, un 25%, para el 2, un 50%, para el 3, un 75% y para el 4, el máximo, un 100%
  - Muestra ese % también en el template
  - Usa la propiedad [style](https://vuejs.org/guide/essentials/class-and-style.html#binding-inline-styles) para establecer el valor de la propiedad CSS _width_
3. Fíjate en los dos mensajes de información "Estás en el nivel más bajo...alto". El primer mensaje solo se debe mostrar si estamos en el nivel 0 del input, mientras que el segunda mensaje si estamos en el nivel 4.
4. Crea una segunda propiedad computada para establecer el color de fondo de la barra. Si el nivel es 4, debe verse de un tono rojo, y azul, en cualquier otro caso.

