_¿Te acordás del hashing? ¡Volvió, en forma de función!_

Si en el ejercicio anterior pensante en una función de hash, ¡estás en lo correcto! Éstas nos permiten generar un código numérico a partir de una cadena de caracteres, y cumplen tanto las propiedades de unicidad como de existencia (bueno, pero eso mismo son funciones :stuck_out_tongue:).  

Existen muchas funciones de hash bien conocidas, como **MD5** y **SHA1** (ambas son también [_funciones de hash criptográficas_](https://en.wikipedia.org/wiki/Cryptographic_hash_function), pero eso lo dejamos para otro momento :innocent:), y son bastante fáciles de usar. 

Por ejemplo, en Ruby podemos calcular estos hashes de la siguiente forma: 

```ruby
Digest::MD5.hexdigest("Hola Mundo")    # representado en hexadecimal (base 16)
# => "d501194c987486789bb01b50dc1a0adb"
Digest::MD5.base64digest("Hola Mundo") # representado en base 64
# => "1QEZTJh0hnibsBtQ3BoK2w=="        # notá que se codifica usando números, letras y algunos símbolos
Digest::SHA1.hexdigest("Hola Mundo")
# => "48124d6dc3b2e693a207667c32ac672414913994"
# etc...
```

> ¡Probalo! Calculá el hash md5 de `'https://mumuki.io'` y `'https://en.wikipedia.org/wiki/Hash_function'` en _base 64_
