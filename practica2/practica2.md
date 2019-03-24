# Práctica 2
### Autores
Eugenio Alcántara García  
Pablo García Llorente

## Preparación de las herramientas
Para poder abordar la práticas debemos de realizar la instalación de la herramienta Rsync sobre las máquinas virtuales creadas a lo largo de la práctica previa, para instalar Rsync simplemente abrimos la terminal y escribimos:

      $sudo apt-get install rsync 

Una vez hayamos seguido todos los pasos e instalado todos los paquetes necesario, podemos comenzar a realizar la práctica.  

## Cuestiones a resolver

### Hay que llevar a cabo las siguientes tareas:
1. #### Probar el funcionamiento de la copia de archivos por ssh
2. #### Clonado de una carpeta entre las dos máquinas
3. #### Configuración de ssh para acceder sin que solicite contraseña
4. #### Establecer una tarea en cron que se ejecute cada hora para mantener actualizado el contenido del directorio /var/www entre las dos máquinas

### 1.Probar el funcionamiento de la copia de archivos por ssh

Para probar el funcionamiento de la copia de archivos por ssh vamos a crear un archivo directamente en otro ordenador, que en nuestro caso sería otra máquina virtual, conectado mediante ssh, más específicamente, indicaremos al comando tar que queremos que use stdout como destino y mandar con una pipe la salida al ssh. Éste debe coger la salida del tar y escribirla en un fichero. La orden sería:

    $tar czf - | ssh 192.168.1.101 'cat > ~/tar.tgz'

Ejecución de la orden, al no indicar el directorio al cual se mandará el archivo, se creará en el directorio /home/usuario del usuario que se ha utilizado para conectar el ssh:

![](creadion de archivo ssh(maq1).png)
