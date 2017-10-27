Al utilizar redirecciones permanentes (como el `302`), le estamos diciendo al navegador que nunca más ingrese a la URL accedida, sino a la que se está redirigiendo.   

Supongamos que María ingresó a `http://cortisimo.com/2bu3xJ3`, y el servidor respondió con un 301 apuntando a `https://wikipedia.org/`. Dado que es una redirección permanente, la próxima vez que ella entre a esa URL corta, el navegador deberá dirigirla directamente a la wiki, **sin pasar por los servidores de nuestro acortador**. 

¡Esto es mucho más barato, porque nuestros servidores recibirán menos pedidos! :moneybag: Notemos cómo un mero código HTTP puede cambiar drásticamente nuestra carga. 

Ahora bien, usar una redirección temporal también tiene sus beneficios: al volver siempre a nuestros servidores, podemos llevar estadísticas de uso que quizás le sean útiles a quien generó el enlace.  

