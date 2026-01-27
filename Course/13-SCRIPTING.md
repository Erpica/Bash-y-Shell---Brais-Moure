# 13 - SCRIPTING

## Archivo de texto que se ejecutará línea por línea secuencialmente. Debe ser ejecutable. Convenciones:
* Con extensión `.sh`
* Primera línea (shebang): `#!/bin/bash` 

## Algunas líneas dejemplo:
```
echo "Tu directorio actual es: $(pwd)"

name="Erpica"
echo "Hola $name"

a=5
b=3
let sum=a+b
echo "La suma es $sum"
sum2=$((a+b))
echo "La suma2 es $sum2"
```

* `let` es el comando que se usa para realizar operaciones aritméticas directamente sobre variables.
* `$(( ))` es más habitual usar expansión aritmética en Bash moderno.

## Lectura de datos
```
#!/bin/bash
echo "¿Cuál es tu nombre? "
read name
echo "Hola, $name"
read -p "¿Cuál es tu edad? " age
echo "Tu edad es $age"
read -s pass
echo "Tu contraseña es $pass"
```
* `read` → solicita datos y los almacena en la variable definida.
	* `read -p` → muestra el prompt en la misma línea.
	* `read -s` → entrada oculta para contraseñas.

```
#!/bin/bash
echo "El nombre del script es: $0"
echo "El primer parámetro es: $1"
echo "El segundo parámetro es: $2"
echo "Número de parámetros: $#"
echo "Todos los argumentos: $@"
```

Ejecución con argumentos: `./script.sh argumento1 argumento2`

* `$0` accede al nombre del script (*script.sh*).
* `$1` accede al argumento en la primera posición (*argumento1*).
* `$2` accede al argumento en la segunda posición (*argumento2*).
* `$#` accede al número total de parámetros (*2*).
* `$@` accede a todos los parámetros (*argumento1 argumento2*).

> [!NOTE] 
>  
> Script de ejemplo con parámetros: [params_script.sh](../Scripts/params_script.sh)
>

[[◀️ Lección anterior](./11-PROCESS.md)] 
[[Inicio 🔼](../README.md)] 
[[Siguiente lección ▶️](./15-LOGIC.md)]