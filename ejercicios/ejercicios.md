#Ejercicios teoría

##Tema 1

###Ejercicio 1

Buscar información sobre las tareas o servicios web para los que se usan más los programas que comentamos al principio de la sesión:

##Tema 2

### Ejercicio 1

Calcular la disponibilidad del sistema si tenemos dos réplicas de cada elemento (en total 3 elementos en cada subsistema).

### Ejercicio 2

Buscar frameworks y librerías para diferentes lenguajes que permitan hacer aplicaciones altamente disponibles con relativa facilidad.
Como ejemplo, examina PM2 https://github.com/Unitech/pm2 que sirve para administrar clústeres de NodeJS.

### Ejercicio 3

¿Cómo analizar el nivel de carga de cada uno de los subsistemas en el servidor?
Buscar herramientas y aprender a usarlas.
...¡o recordar cómo usarlas!

### Ejercicio 4

Buscar ejemplos de balanceadores software y hardware (productos comerciales).
Buscar productos comerciales para servidores de aplicaciones.
Buscar productos comerciales para servidores de almacenamiento.

## Tema 3

### Ejercicio 1

Buscar con qué órdenes de terminal o herramientas podemos configurar bajo Windows y bajo Linux el enrutamiento del tráfico de un servidor para pasar el
tráfico desde una subred a otra.

### Ejercicio 2

Buscar con qué órdenes de terminal o herramientas gráficas podemos configurar bajo Windows y bajo Linux el filtrado y bloqueo de paquetes.

## Tema 4

### Ejercicio 1



## Tema 5

### Ejercicio 1

Buscar información sobre cómo calcular el número de conexiones por segundo.

        netstat -an | grep :80 | sort
        netstat | grep http | wc -l
        
Para empezar, podéis revisar las siguientes webs:

    http://bit.ly/1ye4yHz
    http://bit.ly/1PkZbLJ
    http://bit.ly/2nGm3MR
    
### Ejercicio 2 

Revisar los análisis de tráfico que se ofrecen en:
http://bit.ly/1g0dkKj
Instalar wireshark y observar cómo fluye el tráfico de red en uno de los servidores web mientras se le hacen peticiones HTTP… o en la red de casa

### Ejercicio 3

Buscar información sobre características, funcionalidad, disponibilidad para diversos SO, etc de herramientas para monitorizar las prestaciones de un servidor.

Para empezar, podemos comenzar utilizando las clásicas de Linux:
         top
         vmstat
         netstat

## Tema 6

### Ejercicio 1

Aplicar con iptables una política de denegar todo el tráfico en una de las máquinas de prácticas. Comprobar el funcionamiento.

Aplicar con iptables una política de permitir todo el tráfico en una de las máquinas de prácticas.
Comprobar el funcionamiento.

### Ejercicio 2

Comprobar qué puertos tienen abiertos nuestras máquinas, su estado, y qué programa o demonio lo ocupa.

### Ejercicio 3

Buscar información acerca de los tipos de ataques más comunes en servidores web (p.ej. secuestros de sesión).
Detallar en qué consisten, y cómo se pueden evitar




