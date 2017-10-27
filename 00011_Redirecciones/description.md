Si lo pensamos unos instantes, veremos que utilizar redirecciones es una opción natural. :leftwards_arrow_with_hook: 

Por ejemplo, cuando el usuario ingrese en su barra de navegación `http://cortisimo.com/2bu3xJ3`, nuestro servidor expandirá la URL y redirigirá a ésta. En código, esto se verá aproximadamente así: 

```java
class UrlController {
  Acortador acortador = new Acortador("http://cortisimo.com");
  
  // Recordemos que se corresponde con la ruta get("/:hash", urlsController::expandir);
  public void acortar(Request pedido, Response respuesta) {
    String expandida = acortador.expandir(pedido.queryParam("hash"));
    respuesta.redirect(expandida);
  }
}
```




