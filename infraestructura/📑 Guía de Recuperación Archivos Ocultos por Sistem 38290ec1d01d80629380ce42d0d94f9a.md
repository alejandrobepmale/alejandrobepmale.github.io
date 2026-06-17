# 📑 Guía de Recuperación: Archivos Ocultos por Sistema (attrib)

Este procedimiento se utiliza cuando los archivos ocupan espacio en el disco y se puede acceder a ellos escribiendo la ruta manual, pero el Explorador de Windows no los muestra en la lista.

**1. Diagnóstico por Consola (CMD o PowerShell)**

Para verificar la existencia de carpetas ocultas antes de aplicar cambios, nos situamos en el directorio y listamos el contenido:

- **Comando:** `dir /a` (en CMD) o `ls -Force` (en PowerShell).

**2. Desocultar la Carpeta Raíz (Acción Inmediata)**

Si la carpeta principal está protegida como archivo de sistema, no dejará ver nada de su interior. Quitamos los atributos ocultos (`-h`) y de sistema (`-s`) directamente a la carpeta madre:

```jsx
attrib -h -s "I:\Respaldo"
```

Usa el código con precaución.

*(Nota: Asegurar la ortografía exacta de la ruta para evitar el error "No se encuentra el archivo").*

**3. Desocultar Contenido de Primer Nivel (Evita congelamientos)**

Para discos muy grandes (ej. 2 TB), ejecutar el comando recursivo (`/s`) puede demorar horas o congelar la consola. La mejor práctica es desocultar **solo el primer nivel de carpetas** para trabajar de inmediato:

```jsx
cd Respaldo
attrib -h -r -s /d *
```

Usa el código con precaución.

**4. Glosario de Parámetros Utilizados**

- `attrib`: Herramienta de Windows para modificar los atributos de archivos y carpetas.
- `h`: Quita el atributo de **Oculto** (Hidden).
- `s`: Quita el atributo de **Sistema** (System) que bloquea la visibilidad total.
- `r`: Quita el atributo de **Solo Lectura** (Read-only) para poder modificar el contenido.
- `/d`: Aplica el comando a las **carpetas** y directorios (no solo a los archivos individuales).
- : Comodín que indica "aplicar a **todo** el contenido actual". [[1](https://www.channelpartner.es/ticpymes/listado-de-comandos-de-windows/), [2](https://es.slideshare.net/slideshow/cmd-38068651/38068651), [3](https://sarreplec.caib.es/pluginfile.php/11770/mod_resource/content/8/DAM_SI03_Contenidos_Web/42_comandos_para_directorios_y_ficheros.html)]

---