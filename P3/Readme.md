P3: Módulos de Apache
La actividad es individual, pero os podéis ayudar sin copiar.
Instrucciones de entrega:
Esta entrega se realizará mediante la plataforma Moodle y GitHub.
En el Moodle, habrá que subir un archivo .md con el siguiente nombre: DAW_
DAW_Apellido1_Apellido2_Nombre.md siguiendo el formato Markdown para explicar
los diferentes ejercicios.
En GitHub se tendrá que subir en el repositorio de la asignatura.
Se puede añadir imágenes y añadirlas en el documento.
Curso: CFGS Desarrollo de aplicaciones web
Módulo: M08 Despliegue de aplicaciones web
Nombre y apellidos: _________________________
Cualquier tipo de plagio o copia será penalizado siguiendo la normativa
de la escuela.
Fecha: 04/10/2023
Tipo: Actividad práctica



P3: Módulos de Apache

1. Añade en tu servidor el módulo mod_info y explique para que se utiliza este plugin.

El módulo mod_info es un módulo de Apache HTTP Server que proporciona información detallada sobre el servidor web y su configuración.
Este módulo se utiliza para obtener información de diagnóstico y estadísticas sobre el servidor Apache, lo que puede ser útil para los administradores del servidor web.

![1](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/058f61d2-e0d6-4554-8054-db80f1861b59)

2. Oculta la versión del sistema y sistema de apache.

![2](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/9ec63e1c-9bba-4c48-a84a-eb1208ccf577)

![3](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/20db958d-35b2-4cfa-af0b-f9f945c9cb38)

3. Crea una carpeta en la raíz del path del servidor con el nombre public y otra con el
nombre private. Permite que la carpeta public se visualice y el resto de las carpetas
que se creen, incluyendo private, no se muestren. A continuación, puede observar
cómo se debe de mostrar la carpeta public:

![4](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/56f92639-17fd-4fb4-8a3f-a4b59fe1421b)

![5](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/bee21f5b-c52e-456a-9906-4c18b8a697d5)

![6](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/c3202177-a780-4a9e-b8e9-8d5da4a5ac96)

4. Prueba de acceder poniendo www. delante de tu URL actual. ¿Funciona? En caso
negativo, haz que funcione mediante el módulo mod_rewrite. Investigue como utilizar
el archivo .htacess para implementarlo.

![7](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/2543b6c4-15b3-43ef-950e-7bb390afaafd)

![8](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/01984168-1a24-4593-b367-85396f8731bf)


5. Muestra los directorios de Apache con un tema diferente. Puedes utilizar
https://github.com/ramlmn/Apache-Directory-Listing u otra alternativa que te llame la
atención.
.


6. (Extra: 1 punto) Crea tu propio tema para el ejercicio anterior, sin dependencias
externas.
