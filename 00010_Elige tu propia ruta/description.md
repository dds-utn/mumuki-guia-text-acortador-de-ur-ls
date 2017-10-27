Ahora pensemos en las rutas de la aplicación. Necesitaremos rutas para...

 * ...mostrar la pantalla principal (la _home_);
 * ...acortar el enlace y redirigir a la página principal cuando presionemos el _call to action_ (el botón princial) `Acortar`;
 * ...expandir la url corta, dado su `hash`

> Suponiendo que nuestras URLs cortas fueran de la forma `https://cortisimo.com/abc1234d`, ¿cuáles de las siguientes rutas permitirían implementar el flujo de nuestra aplicación?
 > 
 > ```java
 > // Opción 1
 > get("/home", homeController::show);
 > get("/:hash", urlsController::expandir);
 > get("/urls", urlsController::acortar);
 > ```
>
 > ```java
 > // Opción 2 
 > get("/", homeController::show);
 > get("/urls/:hash", urlsController::expandir);
 > post("/urls", urlsController::acortar);
 > ```
 >
 > ```java
 > // Opción 3
 > get("/", homeController::show);
 > get("/:hash", urlsController::expandir);
 > post("/urls", urlsController::acortar);
 > ```
 >
