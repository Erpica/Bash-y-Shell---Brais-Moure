# Administración del sistema
## Tipos de permiso / modo octal:
- Lectura: 
  * r / 4
- Escritura: 
  * w / 2
- Ejecución: 
  * x / 1
  
## Tipos de usuario:
- u: Propietario
- g: Grupo
- o: Otro
- a: Resto

## Ver permisos:
* En archivos:
  * `ls -l nombre_archivo`
  * `ls -ld nombre_directorio` 

# Anatomía de los permisos:
## Modo simbólico:
`-rwxrwxrwx`
* `-`  tipo de archivo
* `rwx`  permisos de usuario, grupo, resto

## Modo octal:
`777`

# Tipos de archivos:
* `-` archivo
* `d` directorio
* `l` enlace simbólico
* `b` dispositivo de bloque
* `c` dispositivo de carácter
* `s` socket
* `p` pipe

# Modificación de permisos:
`chmod`
* chmod [tipo_usuario][+/-][permiso] nombre_archivo/directorio
  * `chmod u+x nombre_archivo`
* chmod [permisos_octal] nombre_archivo/directorio
  * `chmod 753 nombre_archivo/directorio`
  * 
`chown`
* Cambiar el propietario:
  
    `chown [usuario] nombre_archivo/directorio`
* Cambiar el propietario y el grupo:
 
    `chown [usuario]:[grupo] nombre_archivo/directorio`


# Máscaras:
Son los permisos por defecto cuando creo un archivo.

`umask` -> Me dice la máscara actual
`umask 022` -> Le quito a la máscara 0 al propietario y 2 al grupo y al resto.

Se refiere a los permisos que tiene un archivo o una carpeta al ser creados. Los números se corresponden con los permisos que quito (excepto el primer cero que quiere decir que está en octal). Al crear un archivo partimos de un máximo de 666 y, en el caso de los directorios 777.


[[◀️ Lección anterior](./07-BASIC-EDITORS.md)] 
[[Inicio 🔼](../README.md)] 
[[Siguiente lección ▶️](./11-PROCESS.md)]



