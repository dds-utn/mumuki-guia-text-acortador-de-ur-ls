¡Volvamos a nuestro flujo principal! :muscle:

Ahora que sabemos que estamos frente a una aplicación Web, necesitaremos desarrollar algunas rutas y pantallas. 

> Suponiendo que nos gustaría que nuestras URLs cortas fueran de la forma `https://miacortador.com/abcd12345`, ¿cuáles de las siguientes rutas permitirían implementar el flujo de nuestra aplicación?
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
> get("/:key", UrlsController::expandir);
> post("/urls", UrlsController::acortar);
> ```
>
> ```java
> // Opción 3 
> get("/", HomeController::show);
> get("/urls/:key", UrlsController::expandir);
> post("/urls", UrlsController::acortar);
> ```
> 
