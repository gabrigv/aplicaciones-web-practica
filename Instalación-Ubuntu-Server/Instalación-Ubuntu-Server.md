# Instalación Ubuntu Server

## Errores

Este Error se soluciona dandole root a /sbin/vboxconfig (Necesitas comandos de administrador para esto)
![Captura Error Ubuntu Server](./CapturaError.png)

## Paso 1 Crear la red Host-only en VirtualBox

### Paso 1 Abre El Gestor De Redes
En virtualbox tienes que ir a archivo arriba a la izquierda y le das a herramientas y luego a red.

### Paso 2 Crea El Adaptador
Le das a crear y aparecera un adaptador nuevo llamado vboxnet0.

### Paso 3 Revisa la configuración IPv4
Comprueba que la direccion de la red es algo como 192.168.56.1/24 si no esta asi le das click-derecho, propiedades y las añades tu mismo.

### Paso 4 Servidor DHCP
Se puede dejar desactivado de momento.

### Paso 5 Cierra el gestor
Deberia de quedar algo asi

![Captura De La Configuracion De Red VirtualBox](./ConfRedVirtualBox.png)

## Paso 5 Instalar Ubuntu Server 24.04

### Paso 1 Idioma
![Captura De El Idioma](./UbuntuServerIdioma.png)

### Paso 2 Teclado
![Captura De Configuración Del Teclado](./UbuntuServerConfTeclado.png)

### Paso 3 Tipo De Instalación
![Captura De El Tipo De Configuración](./UbuntuServerTypeInst.png)

### Paso 4 Configuración De Red
![Captura De La Configuración De Red](./UbuntuServerNETConf.png)

### Paso 5 Proxy y Mirror
![Captura De La Configuración Del Proxy](./UbuntuServerProxy.png)

### Paso 6 Almacenamiento
Aqui tenemos que marcar la casilla que pone usar el disco completo.

### Paso 7 Perfil Del Usuario
![Captura Del Perfil Del Usuario](./UbuntuServerPflConf.png)

### Paso 8 Servidor SSH
![Captura De La Configuracion De SSH](./UbuntuServerSSHConf.png)

### Paso 9 Snaps Destacados
![Captura De Los Snaps Destacados](./UbuntuServerSnap.png)

### Paso 10 Fin De La Instalación
Ahora lo unico que hay que hacer es esperar a que termine y darle a Reboot Now.
