# Instalación y configuración de NGINX

Entramos en https://nginx.org/en/download.html y seleccionamos la version que queramos. En mi caso, descargo la versión estable para windows 1.20.2

![image](https://user-images.githubusercontent.com/91744454/166659359-c5788965-13ff-4d9c-9204-ebc7b8bcb847.png)  
![image](https://user-images.githubusercontent.com/91744454/166659464-db5e161a-e234-42f5-bd55-adf81d20977a.png)


Una vez descargado, lo movemos a la carpeta C: y lo descomprimimos allí.

Las carpetas se verán así:  
![image](https://user-images.githubusercontent.com/91744454/166659523-881e6285-6267-44f8-a783-fa2321b7ae21.png)




Hacemos click en nginx.exe, ejecutando así el programa. Después de este click, ya estará corriendo. Esto podemos comprobarlo accediendo a la ruta ‘localhost’ en nuestro navegador.  

![image](https://user-images.githubusercontent.com/91744454/166661738-41e69f45-5251-4efb-b62f-b45b3fa549cb.png)


Después de comprobar que funciona, nos metemos en la carpeta “conf” y abrimos el archivo nginx.conf.  
![image](https://user-images.githubusercontent.com/91744454/166661922-279fe500-02d8-41b6-83ee-2354b8c7730e.png)  
![image](https://user-images.githubusercontent.com/91744454/166661956-777b48f3-580b-4e93-8a2a-0942a4341e61.png)



En este archivo se encuentra la configuración del host.  Podremos tanto ver como editar la configuración (es decir, los lugares donde nginx buscará los enlaces.   

![image](https://user-images.githubusercontent.com/91744454/166661998-bfe9d68d-9342-4819-bb57-6265e29508a0.png)



Vamos al final de todo, donde aparece “HTTPs server” e introducimos esta configuración.   
![image](https://user-images.githubusercontent.com/91744454/166662052-7eb3e6eb-814c-4724-9d0c-ca29503cd7e3.png)

![image](https://user-images.githubusercontent.com/91744454/166662199-192c3de5-8b31-42c3-ae57-3b96f8ca43a1.png)



Una vez lista la configuración, introducimos los archivos html que queramos mostrar con nginx. En mi caso he descargado tres páginas html en https://onehtmlpagechallenge.com y he creado un archivo índice adicional index.html el cual pusimos en la configuración previa, con el que poder acceder a estos. 
  

Abrimos nuestra consola de comandos, nos dirigimos a la carpeta de nginx y ejecutamos el comando `start nginx`.  
![image](https://user-images.githubusercontent.com/91744454/166662261-81a5ca57-641d-4f94-bfce-0075e1b948b4.png)





Una vez arrancado, accedemos a localhost desde nuestro navegador y aparecerá nuestra página de índice.  
![image](https://user-images.githubusercontent.com/91744454/166662495-494c878b-4fcd-4e74-9869-088896815860.png)

Y así, hemos configurado nginx para mostrar la página que queramos.
