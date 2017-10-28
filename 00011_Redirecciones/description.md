Si lo pensamos unos instantes, veremos que utilizar redirecciones es una opción natural. :leftwards_arrow_with_hook: 

Por ejemplo, cuando el usuario ingrese en su barra de navegación `http://cortisimo.com/2bu3xJ3`, nuestro servidor expandirá la URL y redirigirá apropiadamente. En código, esto se verá aproximadamente así: 

```java
class UrlController {
  Acortador acortador = new Acortador("http://cortisimo.com");
  
  // Recordemos que se corresponde con la ruta get("/:hash", urlsController::expandir);
  public void expandir(Request pedido, Response respuesta) {
    String expandida = acortador.expandir(pedido.queryParam("hash"));
    respuesta.redirect(expandida);
  }
}
```

> Ahora bien, existen muchos tipos de redirecciones, que se pueden agrupar en dos grandes categorías: permantes y temporales. 
> 
> Leé mas sobre éstos [acá](https://en.wikipedia.org/wiki/URL_redirection#HTTP_status_codes_3xx) y pensá ¿nos conviene usar un código `301` o un `302` (o `307`)? ¿Qué ventajas tendría una u otra opción?
> 
> Y no, no hay una única respuesta posible :stuck_out_tongue:



