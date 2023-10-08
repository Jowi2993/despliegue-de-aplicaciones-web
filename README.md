3.Analiza los headers de las peticiones cuando inicias sesión en el Moodle y comprende cómo se obtiene el token.
Para ello, necesitamos saber de dónde salen TODOS los datos sensibles que se envían

![headers](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/8a279bd4-a593-4940-b3ad-136a679d2227)


4. ¿A qué puerto se reciben normalmente las peticiones del protocolo HTTP?
¿A qué capa del modelo TCP/IP se encuentra el protocolo HTTP? ¿Y los protocolos TCP, UDP, e IP?

Las peticiones normalmente se suelen recibir en el puerto 80.
El protocolo HTTP se encuentra en la capa de aplicación del modelo OSI y en la capa de aplicación del modelo TCP/IP.
Los protocolos TCP, UDP e IP  se encuentran en diferentes capas del modelo TCP/IP:

5. ¿Cuál es el significado de la siguiente respuesta de un servidor?

HTTP/1.1 302 Found
Location: http://www.example.com/test/index2.php

Cuando un cliente recibe esta respuesta del servidor, debería seguir automáticamente la redirección y enviar una nueva solicitud al URL proporcionado 
para obtener el recurso deseado. La redirección "302 Found" se utiliza cuando un recurso se ha movido temporalmente a una nueva ubicación, 
y el cliente debe actualizar su enlace o URL.

6. Utilizando el filtro de captura para la interfaz de red de Wireshark, analiza la petición al host: www.google.com. Mostrando la cabecera IP, la dirección IP de tu ordenador y la del servidor. Comprueba que, poniendo esa IP en el navegador, accedas a Google.

![image](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/71689d84-d3db-4b79-9932-6aee26972e24)
![IP google](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/72cb5855-4fda-4271-82ba-622d356fca47)
![google](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/68accd3f-3155-4562-9eac-69f63be3e46b)
