# Ejercicios teoría

## Tema 1

### Ejercicio 1

Buscar información sobre las tareas o servicios web para los que se usan más los programas que comentamos al principio de la sesión:

  1. Apache: El servidor HTTP Apache es un servidor web HTTP de código abierto, para plataformas Unix (BSD, GNU/Linux, etc.), Microsoft Windows, Macintosh y otras, que implementa el protocolo HTTP/1.1. Es utilizado principalmente para servir páginas web.
  2. nginx: Es un servidor web/proxy inverso ligero de alto rendimiento y un proxy para protocolos de correo electrónico (IMAP/POP3). Originalmente fue creado para servir páginas web estáticas para sitios con mucho tráfico.
  3. thttpd: es un servidor web de código libre disponible para la mayoría de las variantes de Unix. 
Se caracteriza por ser simple, pequeño, portátil, rápido, y seguro, ya que utiliza los requerimientos mínimos de un servidor HTTP. Esto lo hace ideal para servir grandes volúmenes de información estática. 
  4. Cherokee: es un servidor web multiplataforma libre escrito en C. Su objetivo es ser rápido y completamente funcional sin dejar de ser liviano, comparado con otros servidores web. Puede usarse como un sistema embebido y soporta complementos para aumentar sus funcionalidades. 
  5. Node.js: es un entorno en tiempo de ejecución multiplataforma, de código abierto, para la capa del servidor (pero no limitándose a ello).
        
## Tema 2

### Ejercicio 1

Calcular la disponibilidad del sistema si tenemos dos réplicas de cada elemento (en total 3 elementos en cada subsistema).


<table>
<thead>
<tr>
<th>Componente</th>
<th>A<sub>n</sub></th>
<th>A<sub>n-1</sub></th>
<th>Resultado</th>
</tr>
</thead>
<tbody>
<tr>
<td>Web</td>
<td>0.9775</td>
<td>0.85</td>
<td>0.99662</td>
</tr>
<tr>
<td>Aplicación</td>
<td>0.99</td>
<td>0.9</td>
<td>0.999</td>
</tr>
<tr>
<td>Base de datos</td>
<td>0.999</td>
<td>0.9999</td>
<td>1</td>
</tr>
<tr>
<td>DNS</td>
<td>0.9996</td>
<td>0.98</td>
<td>0.99999</td>
</tr>
<tr>
<td>Cortafuegos</td>
<td>0.9775</td>
<td>0.85</td>
<td>0.99662</td>
</tr>
<tr>
<td>Switch</td>
<td>0.9999</td>
<td>0.99</td>
<td>1</td>
</tr>
<tr>
<td>Data Center</td>
<td>0.9999</td>
<td>0.9999</td>
<td>1</td>
</tr>
<tr>
<td>ISP</td>
<td>0.9975</td>
<td>0.95</td>
<td>0.99987</td>
</tr>
<tr>
<td>-</td>
<td>-</td>
<td><strong>Total</strong></td>
<td>0.99214</td>
</tr>
</tbody>
</table>

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

## Tema 7

### Ejercicio 7

Buscar información sobre los sistemas de ficheros en red más utilizados en la actualidad y comparar sus características. Hacer una lista de ventajas e inconvenientes de todos ellos, así como grandes sistemas en los que se utilicen.




