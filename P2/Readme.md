P2: Administración de servidores web
La actividad es individual, pero os podéis ayudar sin copiar.
Comente todo el código para su correcta comprensión. Si quiere destacar algo, puede responder la actividad con los puntos que considere clave o destacables.
Instrucciones de entrega:
Esta entrega se realizará mediante la plataforma Moodle y GitHub.
En el Moodle, habrá que subir un archivo .md con el siguiente nombre: DAW_ DAW_Apellido1_Apellido2_Nombre.md siguiendo el formato Markdown para explicar los diferentes ejercicios.
En GitHub se tendrá que subir en el repositorio de la asignatura. Se puede añadir imágenes y añadirlas en el documento.
 

1.	Instale en una máquina virtual un sistema operativo con base Linux (se recomienda Debian o Ubuntu) e instale apache2.












2.	Explique con sus palabras que es una petición GET, POST, PUT y DELETE, remarcando sus diferencias.

GET: Se usa para obtener datos de un servidor web. Los datos se envían en la URL, y sirve para solicitudes de solo lectura. Para OBTENER.

POST: Sirve para enviar datos al servidor como por ejemplo al enviar un formulario en línea. Los datos se envían de forma segura en el cuerpo de la solicitud. Para ENVIAR.

PUT: Se utiliza para actualizar o crear recursos en el servidor. Los datos se envían en el cuerpo de la solicitud. Para ACTUALIZAR.

DELETE: Se usa para eliminar un recurso en el servidor sin necesidad de enviar datos en el cuerpo de la solicitud. Para ELIMINAR.











3.	Cambie del puerto 80 al puerto 4444 el servidor apache2. Muestra desde el navegador su funcionamiento adjuntando una captura de pantalla.












4.	Instale un certificado SSL y configure su Apache para servir contenido a través de HTTPS en el puerto 4444. Muestre desde el navegador cómo se muestra el sitio web como "seguro" (aunque sea un certificado autofirmado).













5.	¿Dónde se encuentran los ficheros de configuración de Apache2?
•	Ubicación principal.
Se encuentran en la carpeta de archivos etc.





•	Explora el archivo apache2.conf. Identifica las secciones principales y describe su propósito.
Me sale en blanco.









•	sites-available y sites-enabled: Explica la diferencia entre estos dos directorios y cómo funcionan juntos.
sites-available es como una carpeta donde guardas tus planes para sitios web, pero no están en línea todavía. Mientras que en sites-enabled pones un sello de aprobación en los planes que realmente quieres que estén en línea, y Apache se encarga de hacerlos visibles en la web. Es una forma organizada de decirle a Apache qué sitios deben estar activos y cuáles no.


•	mods-available y mods-enabled: Explica la diferencia entre estos dos directorios.
mods-available es como una lista de módulos de Apache que tienes disponibles, pero aún no los estás usando. Por otro lado, en mods-enabled, pones una marca en los módulos que realmente quieres usar en tu servidor Apache. Esto te permite activar o desactivar fácilmente diferentes características sin tener que meter mano en la configuración principal de Apache.









6.	¿Dónde se encuentran los ficheros de ejecución de Apache2?
•	Ubicación principal
Los archivos de ejecución de Apache2, que son parte de los scripts y programas necesarios para iniciar, detener, reiniciar y administrar el servidor web Apache2, suelen ubicarse en el directorio /usr/sbin/.
•	Control del servicio: Utiliza el binario de ejecución para iniciar, detener, recargar y reiniciar el servidor Apache2 explicando la diferencia entre cada uno de los comandos utilizados.
Para controlar el servidor web Apache2 en sistemas Debian, se utilizan los siguientes comandos con el binario apache2ctl: start para iniciar Apache2, stop para detenerlo, graceful para recargar la configuración sin detenerlo, y restart para detener y reiniciar el servidor. Estos comandos permiten gestionar el funcionamiento del servidor y aplicar cambios de configuración de manera efectiva.
•	Comprobación de sintaxis: Usa el binario de Apache para verificar la sintaxis de tu configuración. Esto es útil para asegurarse de que no haya errores antes de reiniciar el servidor.
.
7.	¿Dónde se encuentran los ficheros de monitorización de Apache2?
•	Ubicación principal
Los archivos de registro de Apache2, que se utilizan para la monitorización y el seguimiento de las actividades del servidor web Apache, suelen estar en el directorio /var/log/apache2/ en Debian.




•	error.log y access.log: Explica la diferencia entre estos dos archivos. Abre y revisa las entradas recientes en cada uno de ello. 




error.log registra errores y problemas del servidor. access.log registra solicitudes y tráfico del sitio web, como direcciones IP, fechas y recursos solicitados. Estos registros son esenciales para diagnosticar fallos y analizar el tráfico web.
•	Rotación de logs: Investiga cómo funciona la rotación de logs en Apache2.
¿Por qué es importante? ¿Cómo se configura?

La rotación de logs en Apache2 es un proceso importante para gestionar los archivos de registro de manera eficiente. Su importancia radica en prevenir que los archivos de registro crezcan indefinidamente y ocupen todo el espacio en disco, lo que podría hacer que el servidor falle. También facilita el mantenimiento y análisis de registros al dividirlos en archivos más pequeños.
La configuración de la rotación de logs en Apache2 se realiza mediante el módulo logrotate, que es una herramienta de gestión de registros en sistemas Unix y Linux.

•	Monitorización en tiempo real: Utiliza herramientas como tail -f para monitorear en tiempo real los accesos a tu servidor web y posibles errores.
La monitorización en tiempo real del servidor web Apache2 se puede realizar utilizando la herramienta tail -f en combinación con los archivos de registro apropiados.




•	Análisis de logs: Instala y usa herramientas como goaccess para analizar y obtener estadísticas visuales a partir de tus logs de Apache2.


8.	¿Qué es un Firewall? ¿Para qué sirve? ¿Por qué es necesario? Instale y configure un Firewall en la máquina virtual para que solo permita tráfico HTTP y HTTPS. Bloquee todo el resto de los puertos y demuestre su funcionamiento.
Un firewall es un sistema o dispositivo diseñado para filtrar y controlar el tráfico de red. Puede ser un software que se ejecuta en un servidor o un hardware dedicado que se coloca entre una red interna y una red externa. El firewall tiene varias funciones, las 3 más importantes son la protección contra amenazas, el control del acceso y la seguridad de red

9.	Explica con tus palabras las diferentes partes de una URL.
Una URL consta de varias partes. El Esquema establece el protocolo a utilizar, como "http://" o "https://". El Nombre de Dominio identifica el servidor, por ejemplo, "www.algo.com". La Ruta señala la ubicación del recurso en el servidor. Los Parámetros permiten enviar datos adicionales con la solicitud. El Fragmento apunta a una sección específica dentro del recurso. Todas estas partes trabajan juntas para localizar y acceder a recursos en la web.

10.	Explica el funcionamiento del protocolo HTTP con tus palabras.  
HTTP es un protocolo para la comunicación en la web. Los clientes envían solicitudes a servidores para obtener recursos. Los servidores procesan las solicitudes y envían respuestas con datos. La transferencia de datos puede ser de varios tipos. Luego, la conexión puede cerrarse o mantenerse abierta para solicitudes adicionales. HTTP es fundamental para la navegación y el acceso a contenido en la web.

11.	¿Qué es un archivo .htaccess? Proporcione un ejemplo de cómo se puede utilizar para reescribir URL o restringir el acceso a ciertas partes de su sitio web.
Un archivo .htaccess es un archivo de configuración utilizado en servidores web Apache para aplicar directivas de configuración específicas en un directorio o en una parte particular de un sitio web. Estas directivas permiten personalizar la configuración y el comportamiento del servidor web en un nivel local sin necesidad de modificar la configuración global de Apache. Los archivos .htaccess son muy útiles para realizar tareas como reescritura de URL, autenticación de usuarios, redirecciones, configuración de encabezados HTTP, entre otros. 

