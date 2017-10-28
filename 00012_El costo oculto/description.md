Al utilizar redirecciones permanentes (como el `301`), le estamos diciendo al navegador que nunca más vuelva a ingresar a la URL accedida, sino a la que se está redirigiendo.   

Supongamos que María ingresó a `http://cortisimo.com/2bu3xJ3`, y el servidor respondió con un `302` apuntando a `https://wikipedia.org/`. Dado que es una redirección permanente, la próxima vez que ella entre a esa URL corta, el navegador deberá dirigirla directamente a la wiki, **sin pasar por los servidores de nuestro acortador**. 

Así, nuestros servidores recibirán menos pedidos. ¡Esto es mucho más barato! :moneybag: Notemos cómo un mero código HTTP puede cambiar drásticamente nuestra carga :sunglasses:.

Ahora bien, usar una redirección temporal como el `302` también tiene sus beneficios: al volver siempre a nuestros servidores, podemos llevar estadísticas de uso que quizás le sean útiles a quien generó el enlace. Por ejemplo, podríamos llevar un contandor de cuántos clicks recibió un link. :mag:

> ¡Veamos qué hacen los que saben! Averiguá mediante `curl` qué código de redirección responde Bitly...
> 
> ```bash
> $ curl -i http://bit.ly/2hVRfWR
> HTTP/????
> Server: nginx
> Content-Type: text/html; charset=utf-8
> Connection: keep-alive
> etc...
> ```
> 
> ...e ingresá la primera línea del resultado a continuación.  
