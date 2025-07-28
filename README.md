# Ejercicios sobre _computed properties_ o estado derivado

Abre con Live Server cada uno de los ficheros index.html del ejercicio a ralizar.

## ¿Algo va mal?

0. Intenta no pedir la solución directa a la IA.
1. Asegurate de que has hecho bien el [setup]((https://vuejs.org/guide/quick-start.html#using-the-global-build)) , engoblado todo el HTML por un contenedor `<div id="app"></div>` 
2. Echa un vistazo a la consola del navegador. Normalmente sucede que nos olvidamos importar algo o hay un error de sintaxis
<img src="https://oscarm.tinytake.com/media/17910d3?filename=1753086794204_TinyTake21-07-2025-10-33-00_638886835924646084.png&sub_type=thumbnail_preview&type=attachment&width=615&height=486" title="Powered by TinyTake Screen Capture"/>

# 1-basic-name

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
