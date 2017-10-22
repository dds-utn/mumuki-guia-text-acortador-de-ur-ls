¡Pero no todo es color de rosa con las funciones de hash! 

Pensá que si el dominio de la función (en este caso, URLs largas) es más grande que su imagen (en este caso, URLs cortas)....



<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6c/Surjection.svg/200px-Surjection.svg.png" alt="" width="auto" height="auto">

...inevitablemente habrá colisiones: dos URLs largas diferentes que generen la misma URL corta. :confused: Matemáticamente hablando, decimos que una función de hash es _no inyectiva_, 

> Esto no es frecuente, porque el conjunto de enlaces cortos es muy grande. Por ejemplo, si sólo generamos enlaces de 7 caracteres usando numeros, mayúsculas y minúsculas, nos da un total de `(27*2 + 10)^7` posibilidades, que es un número bastante grande :stuck_out_tongue: 
> 
> Pero de vez en cuando puede haber colisiones. ¿Qué podemos hacer en este caso?

