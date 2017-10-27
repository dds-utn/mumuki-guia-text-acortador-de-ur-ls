Al utilizar redirecciones permanentes (como el `302`), le estamos diciendo al navegador que nunca más vuelva a ingresar a la URL accedida, sino a la que se está redirigiendo.   

Supongamos que María ingresó a `http://cortisimo.com/2bu3xJ3`, y el servidor respondió con un `301` apuntando a `https://wikipedia.org/`. Dado que es una redirección permanente, la próxima vez que ella entre a esa URL corta, el navegador deberá dirigirla directamente a la wiki, **sin pasar por los servidores de nuestro acortador**. 

Así, nuestros servidores recibirán menos pedidos. ¡Esto es mucho más barato! :moneybag: Notemos cómo un mero código HTTP puede cambiar drásticamente nuestra carga :sunglasses:.

Ahora bien, usar una redirección temporal también tiene sus beneficios: al volver siempre a nuestros servidores, podemos llevar estadísticas de uso que quizás le sean útiles a quien generó el enlace.  

