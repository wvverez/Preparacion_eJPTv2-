# Enumeración puertos abiertos

<img src="images/image.jpg" width="400" height="250">


Escaneo usado:
<pre> 
  <code> 
    nmap -p- --open -sS --min-rate 5000 -n -Pn (IP) -oN info_puertos
  </code> 
</pre> 

-p- : Escanea todos los puertos del 1 al 65535 

--open: Muestra solo los puertos que estéan abiertos 

-sS: Hace el escaneo más rápido y sigiloso 

--min-rate 5000 : Fuerza a nmap a que no vaya más lento que 5000 paquetes por segundo, hace el escaneo muy rápido

-n : Desactiva la resolución DNS, no intenta convertir ips en nombres de dominio

-Pn: Desactiva el host discovering, ya que suponemos que estean ya levantadas 

-oN : guarda el escaneo nmap en un archivo.


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
