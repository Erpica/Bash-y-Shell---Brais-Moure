# 03 - Gestión de archivos
## Directorios por defecto más típicos:
* /     Raíz del sistema.
* /home Directorios personales de los usuarios.
* /etc  Archivos de configuración del sistema.
* /bin  Programas básicos.
* /usr  Programas del usuario.
* /var  Datos variables del sistema (registros, logs, colas...).
* /tmp  Archivos temporales.

## Manipulación:
* touch
* mkdir
* cp
    - cp -r -> Se usa cuando sólo quieres el contenido, no una copia exacta.
    - cp -a -> Copia recursiva exacta.
* mv -> mover directorio o cambiar nombre a archivo
* rmdir -> eliminia un directorio vacío
* rm -> Elimina un archivo
    - rm -r -> Elimina un directorio de manera recusrsiva.
    - rm -ri -> Modo de eliminación recursiva con confirmación interactiva.

> [!CAUTION]
>
> ⚠️ El comando `rm` No se envía a la papelera. Cuidado con lo que se borra.
>
> ✋ La opción f (force) en rm -rf es muy peligrosa ya que no pide confirmación ni muestra errores si el directorio no existe.

## Wildcard (comodines):

\* ?

## Listados avanzados:
* tree
* find . -name "*.md"

[[◀️ Lección anterior](./02-FIRST-STEPS.md)] 
[[Inicio 🔼](../README.md)] [
[Siguiente lección ▶️](./05-ADVANCED-COMMANDS.md)]