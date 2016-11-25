# Peticiones HTTP

Cuando nuestro navegador quiere acceder a una página web a través de HTTP (*scheme* = http), lo que hace es comunicarse con un servidor HTTP. Para ello descompone la URL en diferentes partes que le permiten conocer la dirección de la máquina (host) y la ruta (*path*) del recurso al que quiere acceder (o al que le va a enviar información), y envía un mensaje al servidor, lo que formalmente se conoce como una *petición*.

Algunas de las acciones que provocan que un navegador realice una petición HTTP son: escribir una URL en la barra de direcciones, pulsar un enlace, refrescar una pestaña o enviar un formulario.

Existen varios [tipos de peticiones](https://es.wikipedia.org/wiki/Hypertext_Transfer_Protocol#M.C3.A9todos_de_petici.C3.B3n), aunque nosotros en este curso trabajaremos con dos tipos:
* **GET**: para solicitar información.
* **POST**: para enviar información.

Los mensajes de respuesta del servidor pueden ser de [muchos tipos](https://es.wikipedia.org/wiki/Hypertext_Transfer_Protocol#C.C3.B3digos_de_respuesta), aunque nosotros nos encontraremos normalmente tres, que significan:
* **200**: que se ha encontrado correctamente el fichero/recurso.
* **403**: que no tenemos permiso para acceder al fichero/recurso.
* **404**: que el fichero/recurso que le hemos solicitado no se ha podido encontrar en el disco duro (puede ser porque no esté o porque la ruta es incorrecta).
 
El siguiente gráfico muestra un esquema simplificado que nos permite hacernos una idea sobre cómo funciona la comunicación entre ambos:

![Arquitectura](../images/client-server.png?token=aGhrYW9zOmNjZWEzYzUwLTdlNWItNGVjOC05MzA0LTkxZDdhMWUxOGZhOA%3D%3D)
