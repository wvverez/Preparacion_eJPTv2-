# SERVICIOS Y VERSIONES NMAP

Escaneo base:
<pre>
  <code>
    nmap -p(puertos abiertos) -sCV -vvv -n -Pn (IP) -oN services_ports
  </code> 
</pre> 

-p(puertos) --> para indicar los puertos abiertos 

-sCV : Ejecuta los scripts por defecto de nmap y detecta Servicios y versiones

-vvv: Triple verbose, para que nos vaya mostrando la información a medida que la vaya encontrando

-n : Desactiva la resolución DNS 

-Pn : No realiza hostDiscovering 

-oN : Guarda el reporte en un archivo
