## COMANDOS AVANZADOS


# Leer archivos:

* cat
* less
* more
* head -n nº_de_líneas (por defecto, 10)
* tail -n nº_de_líneas (por defecto, 10)
* tail -f nombre_del_archivo -> va cargando en tiempo real si se modifica el archivo

# Búsquedas:
* grep -i "Word" file.txt (case insensitive con el -i)
* grep -r directorio (recursivamente en todos los archivos)
* wc archivo: (cuenta lineas, palabras y caracteres)
    - -w
    - -l
    - -c

# Redirecciones y pipes
> 
>>
<
| ->  cat holi.txt | grep "prueba" | wc

# Variables de entorno
* Local: 

    name="Erpica" (variable local, para esta sesión/pestaña)
echo $name -> Erpica

* Global:

export NOMBRE=


[[Lección anterior ▶️](./03-FILE-MANAGEMENT.md)]
[[Inicio 🔼](../README.md)] 
[[Siguiente lección ▶️](./07-BASIC-EDITORS.md)]

