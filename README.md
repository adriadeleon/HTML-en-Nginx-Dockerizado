# HTML-en-Nginx-Dockerizado

___
- Introducción
___
- ¿Que es Docker?

Docker es una plataforma de software que le permite crear, probar e implementar aplicaciones rápidamente. Docker empaqueta software en unidades estandarizadas llamadas contenedores que incluyen todo lo necesario para que el software se ejecute, incluidas bibliotecas, herramientas de sistema, código y tiempo de ejecución. Con Docker, puede implementar y ajustar la escala de aplicaciones rápidamente en cualquier entorno con la certeza de saber que su código se ejecutará.

La ejecución de Docker en AWS les ofrece a desarrolladores y administradores una manera muy confiable y económica de crear, enviar y ejecutar aplicaciones distribuidas en cualquier escala.

- ¿Que es Nginx?

NGINX es un servidor web open source de alta performance que ofrece el contenido estático de un sitio web de forma rápida y fácil de configurar. Ofrece recursos de equilibrio de carga, proxy inverso y streaming, además de gestionar miles de conexiones simultáneas. El resultado de sus aportes es una mayor velocidad y escalabilidad.

___
- Comienzo de la practica:
___

Para poder empezar con la practica debemos tener las herramientas suficientes para instalarlo todo, en este caso utilizaremos Docker y Nginx para poder realizar la práctica.

Para poder hacer que Nginx tenga nuestros propios archivos Front-End tendremos que crear con anterioridad la imagen del mismo, asi al tenerlo lo podremos implementar.

Para hacer esto debemos crear y editar el archivo **Dockerfile** que no contiene extensión en la carpeta que contenga el *Front-end*.

Dentro del archivo que modificaremos tenemos que escribir el siguiente codigo:
``
From nginx:latest
copy * /user/share/nginx/html/
ls (para visualizar que todo ha funcionado exactamente como deseamos)
``

Si ya tenemos este paso realizado solo nos queda ejecutar un comando, este comando se lanza desde la misma carpeta donde alojamos nuestro **Dockerfile**.

Una vez realizada la práctica debemos comprobar que funciona poniendo en el buscador del navegador web **localhost:8888**
![image](https://user-images.githubusercontent.com/98842240/169795968-35d30a7e-9b4d-47ea-bb21-63405f03e5de.png)

