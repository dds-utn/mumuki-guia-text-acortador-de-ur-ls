_¿Te acordás del hashing? ¡Volvió, en forma de función!_

Si en el ejercicio anterior pensante en una función de hash, ¡estás en lo correcto! Éstas nos permiten generar un código numérico a partir de una cadena de caracteres, y cumplen tanto las propiedades de unicidad como de existencia (bueno, pero eso mismo son funciones :stuck_out_tongue:).  

Existen muchas funciones de hash bien conocidas, como **MD5** y **SHA1** (ambas son también [_funciones de hash criptográficas_](https://en.wikipedia.org/wiki/Cryptographic_hash_function), pero eso lo dejamos para otro momento :innocent:), y son bastante fáciles de usar. 

Por ejemplo, en Ruby podemos calcular estos hashes de la siguiente forma: 

```ruby
Digest::MD5.hexdigest("Hola Mundo")
Digest::SHA1.hexdigest("Hola Mundo")
```

> ¡Probalo! Calculá el hash md5 de `'https://mumuki.io'` y `'https://en.wikipedia.org/wiki/Hash_function'`
