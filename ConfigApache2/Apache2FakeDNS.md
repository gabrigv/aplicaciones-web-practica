# Lo que haremos en esta practica es crear una pagina web con apache y que con una maquina virtual podamos entrar poniendo el nombre de la pagina

ssh gabriel@ip del servidor | para conectarnos al servidor

sudo su | para tener siempre el poder de root

cd /var/www | para meternos en el directorio de las paginas web

mkdir smr y cd smr  | para crear un nuevo directorio y meternos en el

mkdir web y mkdir intranet | para crear los 2 directorios de las webs

cd web y nano index.html | para crear el archivo html deberemos de escribir una linea de html

cd ../intranet y nano intranet.html | para crear el archivo html de intranet haremos lo mismo que la otra

sudo apt install apache2-utils -y | para instalar apache2 utils

sudo htpasswd -c /etc/apache2/.htpasswd alumno | esto sirve para poner la contraseña, en el directorio /etc/apache2/.htpasswd con el user alumno

