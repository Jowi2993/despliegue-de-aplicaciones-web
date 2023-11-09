1- Crea dos sitios web que compartirán IP y puerto, pero tendrán nombres DNS distintos
para acceder a ellos. El nombre del primer dominio será daw.gimbernat.eug.es y el
segundo tunombreyapellidos.gimbernat.eug.es, donde “tunombreyapellidos” contiene
la inicial de tu nombre, el primer apellido, y la inicial de tu segundo apellido. De esta
manera, si tu nombre es: Francisco Mesas Cervilla, el domino quedaría:
fmesasc.gimbernat.eug.es.
• En el primer caso, daw.gimbernat.eug.es tendrá su directorio base en
/var/www/daw/ conteniendo una página llamada index.html que ponga el
nombre de la clase como título con un archivo css para aplicarle estilos al título.
• En el segundo caso, fmesasc.gimbernat.eug.es tendrá su directorio base en
/var/www/fmesasc/ (el equivalente para vuestros nombres), conteniendo una
página llamada index.html que contenga vuestro currículum aplicándole un
estilo css para que se visualice correctamente.
Para ello, tendrás que crear un archivo de configuración (copiado de 000-default.conf)
para cada uno de los dominios. Recuerda que con a2ensite puedes crear los enlaces
simbólicos necesarios para añadir esta configuración a la ejecución de apache.

![1](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/3394b034-18f9-4484-a2bf-399f8a4f4767)

![2](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/d9596150-38e9-42c1-bfcd-8fda29aa3cfa)

![3](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/968a91eb-52ba-477d-887c-e2fde1b992b6)

![4](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/e748f828-0c27-4306-880d-0757a0dce10d)

![5](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/e15b7274-39e6-4c56-a516-0a61e2247c95)

![6](https://github.com/Jowi2993/despliegue-de-aplicaciones-web/assets/144775347/75601797-8db3-4ae1-9075-1ea3faab1f17)
