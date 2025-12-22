# Enumeración puertos abiertos

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
