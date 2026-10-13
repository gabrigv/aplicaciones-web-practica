# Instalación de MariaDB en Ubuntu 24.04

## 1. Objetivos

Al terminar la práctica serás capaz de:
• Explicar qué es una base de datos y para qué la necesita WordPress.
• Instalar MariaDB sobre Ubuntu 24.04 y comprobar que funciona.
• Instalar PHP y comprobar que Apache lo ejecuta.
• Dejar el servidor (Linux, Apache, MariaDB y PHP) listo para instalar WordPress

## 2. Requisitos previos

- VM Ubuntu 24.04 y apache funcionando.
- Permisos sudo en la VM y conexion a internet.
- Repositorio de github con readme.md donde enlazar las practicas

## 3. Normas de la memoria

1. Crear el repositorio en github llamado practica-mariadb.md y enlazarlo a el readme.md
2. Para cada paso hay que poner:
   - El comando ejecutado.
   - La salida del comando en la terminal.
   - Captura de pantalla cuando lo indique
   - Explicacion de tus propias palabras de las preguntas y que hace.
3. En github hacer commits con mensajes precisos.
4. Responder a las pregutas en el documento

## 4. Antes de empezar: ¿qué es una base de datos?

Una base de datos es como un archivador donde un programa guarda su información. Una base de datos esta organizada en tablas como en una hoja de calculo, con columnas y filas.

### ¿Para qué necesitamos WordPress?

WordPress guarda en la base de datos todo lo que no son ficheros: 
