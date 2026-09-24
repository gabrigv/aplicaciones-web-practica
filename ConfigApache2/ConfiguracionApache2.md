# Configuracion Apache2 en terminal linux

Primero tienes que conectar la maquina ubuntu server a el host haciendo desde la terminal host ssh gabriel@192.168.56.10

Luego hemos instalado apache2 con "sudo apt-get install apache2"

Hemos hecho "systemctl status apache2" para ver que esta bien instalado y esta corriendo

La carpeta de apache es /etc/apache2

Entramos a la carpeta sites-available, de ahí entramos en el archivo 000-default.conf y vamos a la ruta en la que indica dónde está nuestra página.

Luego nos vamos a este directorio cd /var/www/html/ hacemos sudo nano index.html y hay podemos modificar nuestra propia pagina

# Deshabilitar antigua página y crear una nueva

1- El archivo 000-default.conf que está en sites-available lo duplicamos y lo llamamos smr.conf.

2- Editamos el archivo duplicado y donde está la ruta añadimos /smr.

3- Vamos a la ruta /var/www/html y con mkdir creamos la carpeta smr.

4- Dentro de la carpeta creamos con nano un fichero llamado index.html y añadimos lo que queramos que se vea en la web.

5- Volvemos donde está instalado Apache, entramos en sites-available y desactivamos el fichero antiguo con a2dissite 000-default.conf.

6- Metemos un systemctl reload apache2 y luego hacemos systemctl status apache2 para que se aplique el cambio y comprobar que va bien.

7- Ahora ponemos a2ensite smr.conf para habilitar la nueva página y metemos otra vez un reload y un status.

8- Entramos en el archivo smr.conf y cambiamos el VirtualHost al puerto 7654 y hacemos un reload.

9- Por último, modificamos el archivo ports.conf de Apache2, añadimos Listen 7654 y hacemos un reload para aplicar los cambios.
