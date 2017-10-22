¿Y si se corta la luz? ¿Y si el programa falla y se pierden los datos?

Cuando pensamos la arquitectura de una aplicación, debemos identificar qué datos podemos perder sin afectar su normal funcionamiento, y qué datos necesitamos persistir. Ante la duda de si persistir un dato o no, siempre nos podemos preguntar...

1. ¿...dejó ya de ser útil?
2. ...en caso de perderlo, ¿podemos recalcularlo a partir de otros datos disponibles?

Si la respuesta a ambas preguntas anteriores es **no**, entonces no hay duda: debe ser persistido.  

> ¿Que deberíamos hacer entonces con nuestro diccionario de enlaces?
