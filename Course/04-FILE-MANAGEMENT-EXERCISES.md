1. Crea un directorio.

    `mkdir nombre_del_directorio`

2. Elimina el directorio que acabas de crear.

    `rm nombre_del_directorio`

3. Copia un archivo en el directorio actual y fuera de éste.

    ~~~
    cp /dir/nombre_del_archivo .
    cp nombre_del_archivo /home/erpica
    ~~~

4. Mueve un archivo del directorio actual.

    `mv ./nombre_del_archivo /home/erpica`

5. Cambia el nombre del archivo que acabas de mover.

    `mv hola.txt holi.txt`

6. Lista todos los archivos de un tipo usando un comodín.

    `find . "*.md"`

7. Elimina un directorio de manera recursiva (cuidado con lo que vas a borrar).

    `rm -r mydir`

8. Elimina todos los archivos de un mismo tipo (cuidado con lo que vas a borrar).

    `rm "*.md"`

9. Utiliza el comando tree.

    `tree`

10. Busca un archivo concreto en el directorio actual utilizando find.

    `find . "nombre_del_archivo.md"`