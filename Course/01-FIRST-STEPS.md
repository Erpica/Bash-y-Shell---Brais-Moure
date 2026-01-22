# PRIMEROS COMANDOS:
## Antes dos formas de escribir código en Markdown:
Para una línea, al principio cuatro espacios en blanco.

    Esto es código 

Si ya vamos a escribir más se pone con las virgulillas:
~~~
echo "Hola, BASH"
echo $SHELL
echo $0
pwd
ls
ls -l
ls -a
ls -lh
---
cd dir
cd dir/dir/dir
cd ..
cd ../../../
cd ~
cd - -> Va al directorio anterior
---
whoami
cal
date
uptime
hostname
uname
uname -a` Información del kernel/sistema.
clear
~~~

## Anatomía del comando

* `comando` es lo que quieres ejecutar (`ls`).
* `opciones` modifican el comportamiento (`-l`)
* `argumentos` son los datos sobre los que actúa (`archivo.txt`, `directorio/`)

~~~
python --help
python -h
man ls
~~~

[[◀️ Lección anterior](./00-CONFIGURATION.md)] 
[[Inicio 🔼](../README.md)] 
[[Siguiente lección ▶️](./03-FILE-MANAGEMENT.md)]