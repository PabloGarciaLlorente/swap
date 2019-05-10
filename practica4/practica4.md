# Práctica 4
### Autores
Eugenio Alcántara García  
Pablo García Llorente

## Generar e instalar un certificado autofirmado
Lo primero que debemos hacer para generar un certificado SSL autofirmado en Ubuntu Server, es activando activando los SSL de Apache, generar los certificados y especifinado los ruta a los certificados en la confirguración. 

    $ a2enmod ssl
    $ service apache2 restart
    $ mkdir /etc/apache2/ssl
    $ openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/apache2/ssl/apache.key -out /etc/apache2/ssl/apache.crt

Una vez hayamos introducido una serie de datos que nos pedirá al ejecutar esa última ordern, procederemos a editar el archivo de configuración del sitio default-ssl. 

    $ nano /etc/apache2/sites-available/default-ssl
    
Y le agregaremos dos nuevos cerficiados debajo de la línea donde pone SSLEngine on. 
    
    SSLCertificateFile /etc/apache2/ssl/apache.crt 
    SSLCertificateKeyFile /etc/apache2/ssl/apache.key
    
Depués de haber añadido esos dos certificados, el archivo default-ssl quedaría como en la imagen de a continucación. 

![Archivo default-ssl](./imagenes/archivo_default_ssl.PNG)

Una vez guardado el archivo (siendo super usaurio), activamos el sitio default-ssl y reiniciamos apache.
        
    $ 2ensite default-ssl
    $ service apache2 reload