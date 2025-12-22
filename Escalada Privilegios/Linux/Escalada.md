# 🔑Privileges

#### 😣Permisos débiles:
<pre>
  <code>
find / -not -type l -perm o+w
  </code>
  </pre>
  
#### 🕵️‍♂️SUID 

* [gtfobins](https://gtfobins.github.io/)

<pre>
  <code>
    find / -perm -4000 2>/dev/null 
  </code>
</pre>

#### 🗝️SUDO

<pre>
  <code>
    sudo -l
  </code>
</pre>

#### ⚔️CAPABILITIES
<pre>
  <code>
getcap -r / 2>/dev/null
  </code>
</pre>
