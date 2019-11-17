# vuejs-Multiples-ejemplos

## v-show

    Espera: any

    Uso:

    Cambia la propiedad CSS display del elemento basado en la veracidad del valor de la expresión.

    La directiva dispara transiciones cuando su condición cambia.
    Hace aparecer o despararecer un elemento . 
    La diferencia con v-if esque este ultimo borra el elemento y v-show lo oculta.
    
     ejemplo:
    
    ```
    <div id="#app">
    <h1 v-if="mostrarTitulo">
        {{ titulo }}
    </h1>

    <p v-show="mostrarParagrafo">
        {{ paragrafo }}
    </p>
</div>

<script>
    var app = new Vue({
        el: '#app',
        data: {
            titulo: 'Vue.js do jeito ninja',
            paragrafo: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
            mostrarTitulo: true,
            mostrarParagrafo: true,
        },
    });
</script>
```
    
  ##  v-cloak

    No espera una expresión

    Uso:

    Esta directiva permanecerá en el elemento hasta que la instancia Vue asociada termine su compilación. Combinada con reglas de CSS tal como [v-cloak] { display: none }, esta directiva puede ser utilizada para esconder mustache bindings no compilados hasta que la instancia de Vue este lista.

    Ejemplo:

    [v-cloak] {
      display: none;
    }

    <div v-cloak>
      {{ message }}
    </div>

    El <div> no será visible hasta que la compilación haya terminado.

    ejemplo:
    
    ```
    <div id="#app">
    <h1 v-if="mostrarTitulo">
        {{ titulo }}
    </h1>

    <p v-show="mostrarParagrafo">
        {{ paragrafo }}
    </p>
</div>

<script>
    var app = new Vue({
        el: '#app',
        data: {
            titulo: 'Vue.js do jeito ninja',
            paragrafo: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
            mostrarTitulo: true,
            mostrarParagrafo: true,
        },
    });
</script>
```
 
