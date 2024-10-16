---
layout: post
author: Flick
title: Hack The Box Writeups
---

Hola soy Flick, esta vez estaremos resolviendo la máquina **Validation**, esta maquina involucra vulnerabilidades, las cuales son las siguientes:

* Buffer overflow
* Cross side scripting
* Ddos 
* Google dorking
* XSS 

Iniciando con la fase de enumeración, no empezaremos con nmap si no con un script que simplifica a nmap y es mucho mejor: 

```python
#!/usr/bin/env python3 
n = int(input(¿Qué numero crees que a salido? ))
if n % 2 == 0:
    raise Exception("ERROR JAJA")
```

