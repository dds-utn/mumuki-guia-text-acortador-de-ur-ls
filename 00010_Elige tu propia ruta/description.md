Ahora pensemos en las rutas de la aplicación. Necesitaremos rutas para...

 * ...mostrar la pantalla principal (la _home_);
 * ...acortar el enlace y redirigir a la página principal cuando presionemos el _call to action_ (el botón princial) `Acortar`;
 * ...expandir la url corta, dado su `hash`

> Suponiendo que nuestras URLs cortas fueran de la forma `https://cortisimo.com/abc1234d`, ¿cuáles de las siguientes rutas permitirían implementar el flujo de nuestra aplicación?
 > 
 > ```java
 > // Opción 1
 > get("/home", HomeController::show);
 > get("/:key", UrlsController::expandir);
 > get("/urls", UrlsController::acortar);
 > ```
>
 > ```java
 > // Opción 2 
 > get("/", HomeController::show);
 > get("/urls/:key", UrlsController::expandir);
 > post("/urls", UrlsController::acortar);
 > ```
 >
 > ```java
 > // Opción 3
 > get("/", HomeController::show);
 > get("/:key", UrlsController::expandir);
 > post("/urls", UrlsController::acortar);
 > ```
 >
