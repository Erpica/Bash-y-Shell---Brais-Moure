1. Muestra todo el contenido de un archivo.
cat nombre_archivo

2. Muestra el contenido paginado de un archivo.
less nombre_archivo

3. Muestra las 15 primeras líneas de un archivo.
head -n 15 nombre_archivo

4. Muestra las 15 últimas líneas de un archivo.
tail -n 15 nombre_archivo

5. Busca una palabra en un archivo.
cat nombre_archivo | grep "palabra"

6. Cuenta las líneas de un archivo.
wc -l nombre_archivo

7. Redirige una salida y guárdala en un archivo.
ls -a > archivo.txt

8. Añade una nueva salida al archivo anterior.
tree >> archivo.txt

9. Encadena 3 comandos.
cat nombre_archivo | grep "palabra" | wc -c

10. Crea una variable local y muéstrala.
nombre="Pica"
echo $nombre