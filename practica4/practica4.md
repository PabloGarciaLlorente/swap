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
